
# Setting Up Reverse Proxy

Before we can go further we have to create a [reverse proxy](https://grpc.io/blog/state-of-grpc-web/) in order for our front-end to make GRPC requests to our server. This is because it is mandatory to have a proxy for translating between gRPC-Web requests and gRPC HTTP/2 responses.

We will do this by using a proxy tool called [envoy](https://www.envoyproxy.io/docs/envoy/latest/start/install).

Below is a basic GRPC proxy. How it works is as follows:

1) Under listeners we setup a listener to port `8080`. This means any requests made on that port will be caught by our proxy.
2) Under HTTP filters we have setup some GRPC web filters as well as CORS
3) Finally under clusters we then setup a section for our server. This is running on port `9090` 

With this setup what will happen is the proxy will take all requests on `8080` and send them onto our server running `9090` and in doing so it would have converted it to the correct protocol needed.

```YAML
admin:
  access_log_path: /tmp/admin_access.log
  address:
    socket_address: { address: 0.0.0.0, port_value: 9901 }

static_resources:
  listeners:
    - name: listener_0
      address:
        socket_address: { address: 0.0.0.0, port_value: 8080 }
      filter_chains:
        - filters:
          - name: envoy.filters.network.http_connection_manager
            typed_config:
              "@type": type.googleapis.com/envoy.extensions.filters.network.http_connection_manager.v3.HttpConnectionManager
              codec_type: auto
              stat_prefix: ingress_http
              route_config:
                name: local_route
                virtual_hosts:
                  - name: local_service
                    domains: ["*"]
                    routes:
                      - match: { prefix: "/" }
                        route:
                          cluster: greeter_service
                          timeout: 0s
                          max_stream_duration:
                            grpc_timeout_header_max: 0s
                    cors:
                      allow_origin_string_match:
                        - prefix: "*"
                      allow_methods: GET, PUT, DELETE, POST, OPTIONS
                      allow_headers: keep-alive,user-agent,cache-control,content-type,content-transfer-encoding,custom-header-1,x-accept-content-transfer-encoding,x-accept-response-streaming,x-user-agent,x-grpc-web,grpc-timeout
                      max_age: "1728000"
                      expose_headers: custom-header-1,grpc-status,grpc-message
              http_filters:
                - name: envoy.filters.http.grpc_web
                  typed_config:
                    "@type": type.googleapis.com/envoy.extensions.filters.http.grpc_web.v3.GrpcWeb
                - name: envoy.filters.http.cors
                  typed_config:
                    "@type": type.googleapis.com/envoy.extensions.filters.http.cors.v3.Cors
                - name: envoy.filters.http.router
                  typed_config:
                    "@type": type.googleapis.com/envoy.extensions.filters.http.router.v3.Router
  clusters:
    - name: greeter_service
      connect_timeout: 0.25s
      type: logical_dns
      http2_protocol_options: {}
      lb_policy: round_robin
      # win/mac hosts: Use address: host.docker.internal instead of address: localhost in the line below
      load_assignment:
        cluster_name: cluster_0
        endpoints:
          - lb_endpoints:
            - endpoint:
                address:
                  socket_address:
                    address: 0.0.0.0
                    port_value: 9090
```

# Generating GRPC code

Before we can make requests details on server and frontend we need to go over how to generate the code using our protobuff files.

```proto
syntax = "proto3";

package user.service;

option go_package = "generated/user_service";

message GetGreetRequest {
}

message GetGreetResponse {
  string greet = 1;
}

service UserService {
  rpc GetGreet(GetGreetRequest) returns (GetGreetResponse);
}
```

Using the simple example above we can then generate our code to use on the back-end and front-end. 

First we generate some code for a Go server:

```shell
protoc -I . --go_out=./server --go-grpc_out=./server user.proto
```

Then we want to generate the front-end browser code:

**Prerequisites: make sure to install the [ts-proto](https://github.com/stephenh/ts-proto) package**

```sh
protoc --plugin=./node_modules/.bin/protoc-gen-ts_proto --ts_proto_opt=outputClientImpl=grpc-web --ts_proto_out=./client/generated user.proto
```

The above script will generate the front-end code that is ESM and [grpc-web](https://github.com/improbable-eng/grpc-web) compatible. By passing in the `--ts_proto_opt=outputClientImpl=grpc-web` we ensure that it generate with the correct implementation details.

## Setting up Go server:

Now that we have created our reverse proxy and generated our Go code we can then implement it. Below we take our generated user service and implement the GetGreet call and return the details required and specified in our `.proto` file.

```go
package main

import (
	"context"
	"fmt"
	"google.golang.org/grpc"
	pb "grpcserver/generated/user_service"
	"log"
	"net"
	"time"
)

const (
	listenAddress = "0.0.0.0:9090"
)

type userService struct {
	// NOTE: this has to be here to satisfy the interface, otherwise the compiler will complain
	pb.UnimplementedUserServiceServer
}

func (t *timeService) GetGreet(ctx context.Context, req *pb.GetGreetRequest) (*pb.GetGreetResponse, error) {
	log.Println("Greetings!")
	return &pb.GetGreetResponse{Greet: "Hello!"}, nil
}

func main() {
	log.Printf("Time service starting on %s", listenAddress)
	lis, err := net.Listen("tcp", listenAddress)
	if err != nil {
		log.Fatalf("failed to listen: %v", err)
	}
	s := grpc.NewServer()

	fmt.Println(lis, s)
	pb.RegisterTimeServiceServer(s, &timeService{})

	if err := s.Serve(lis); err != nil {
		log.Fatalf("failed to serve: %v", err)
	}
}
```


## Setting up the Client

The server is the easy part. Now we need to setup the front-end. Using your favorite framework we can then create a file that implements our GRPC communication. If you look at the way we generated our client code we needed to pass in the **grpc-web** option. This is important. Basically what this does is generates a communication client for the requests. There are other ways you can do this. However in this case we are working with improbable's  version. 

First you need to create the `GrpcWebImpl` then you can take your service `UserServiceClientImpl` and give it the RPC we just created and then after everything is up and running you can make requests!

```ts
import {grpc} from "@improbable-eng/grpc-web";
import {GrpcWebImpl, TimeServiceClientImpl} from "../generated/time";

const rpc = new GrpcWebImpl('http://localhost:8080', {
    debug: false,
    metadata: new grpc.Metadata({}),
});

const client = new UserServiceClientImpl(rpc);

console.log(await client.GetGreet({}));
console.log(await client.GetCurrentTime({}));
```

## Resources

Article on `ts-protoc` library:
https://blog.mechanicalrock.io/2022/04/08/getting-started-with-protobufs-and-typescript.html

Library for fully generating and using in client and backend:
https://github.com/bufbuild/connect-web

## Install of Plugins for Protoc

To see what protoc plugins or to put plugins for protoc go to: 

```sh
cd ~/.local
```
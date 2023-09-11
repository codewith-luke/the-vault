## Services

- Proxy Service (HTTP/GRPC)
- Registry service (TCP)
- Communication to external services ([[@RPC and GRPC]])
## Responsibility

- Handle registration of services
- Handle the subscription of services and updates to those services
- Proxy requests to the correct service in relation to the proxy service

Communication flow: [[Orchestrator Architecture]]
## How It Works

In order to not have to write a lot of the boilerplate for our CRUD logic for the proxy layer we are using a [code gen](https://github.com/deepmap/oapi-codegen) library based on the [Open API](https://www.openapis.org/) schema.

To understand how the Registry Service and Proxy Service work together make sure to checkout [[Orchestrator Architecture]] to get an understanding of how the basic flow would work.

To summarize:

1) Services register into the *registry service*. Services do not communicate directly to the *proxy service*.
	- Services that are not registered are considered dead, will return empty from the registry.
	- Services that do not exist after a registry dies will eventually be removed. This would be based on a heartbeat to check on the service.
2) HTTP requests will be fired at the proxy service layer. 
3) Fetch/Update the internal cache of available internal services
	- The proxy service will keep an internal cache of all available services. If a service changes or is removed, the registry will let the proxy know.
4) Proxy those requests out to relevant services over GRPC

## Proxy Endpoints

- /login - *POST*
- /logout - *POST*
- /register - *POST*
- /profile - *GET/PATCH*
- /profile/settings - *GET/PATCH*

```protobuf
package dsa;

message LoginRequest {
    // request data
}

message LoginResponse {
	// request data
}

message LogoutRequest {
    // request data
}

message LogoutResponse {
	// request data
}

message RegisterRequest {
	// request data
}

message RegisterResponse {
	// request data
}

service AuthService {
    rpc Login (LoginRequest) returns (LoginResponse) {}
    rpc Logout (LogoutRequest) returns (LogoutResponse) {}
    rpc Logout (RegisterRequest) returns (RegisterResponse) {}
}

service ProfileService {
    rpc Login (LoginRequest) returns (LoginResponse) {}
    rpc Logout (LogoutRequest) returns (LogoutResponse) {}
}
```

- /groups - *GET*
- /groups/new - *POST*
- /groups/:id - *GET/PATCH
- /groups/:id/members - *GET
- /groups/:id/messages - *GET/POST*
# References

- https://www.weave.works/blog/container-design-patterns-for-kubernetes/
- https://betterprogramming.pub/building-a-load-balancer-in-go-3da3c7c46f30
- https://medium.com/@leonardo5621_66451/building-a-load-balancer-in-go-1c68131dc0ef


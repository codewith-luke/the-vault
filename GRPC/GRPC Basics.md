### What is GRPC?

- [Go GRPC Tutorial](https://grpc.io/docs/languages/go/basics/)
### Generating With Protoc

**Prerequisites**
Make sure you have followed [these](https://grpc.io/docs/languages/go/quickstart/) steps to setup *Protoc*.
#### Generating

```sh
protoc --go_out=. --go_opt=paths=source_relative \
    --go-grpc_out=. --go-grpc_opt=paths=source_relative \
    {proto_path}
```
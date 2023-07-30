# droneshield-test-upstream

Place to store service contract `proto` and generated gRPC service code.

## To generate gRPC service code

```bash
# generate proto message & custom type
protoc --go_out=./svc ./proto/droneService.proto

# generate rpc methods & service client
protoc --go-grpc_out=./svc ./proto/droneService.proto
```
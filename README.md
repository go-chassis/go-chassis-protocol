# go-chassis-protocol


## How to use
Import the protocol client you want to use 

```go
import _ "github.com/go-chassis/go-chassis-protocol/client/grpc"
```
Import the protocol server you want to use and launch it by chassis.yaml
```go
import _ "github.com/go-chassis/go-chassis-protocol/server/grpc"
```

```yaml
cse:
  service:
    registry:
      address: http://127.0.0.1:30100 # If type is File then address will be the path of the file
  protocols:
    grpc:
      listenAddress: 127.0.0.1:5000
      advertiseAddress: 127.0.0.1:5000
```
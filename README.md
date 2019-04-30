Rundeck Go SDK
==============
Go SDK generated from an OpenApi 2.0 spec via Autorest.

> WARNING: The OpenApi spec and SDK are under heavy development. The spec, methods, interfaces, and project structure may change heavily between releases.


## Example Usage

```go
import "fmt"

import "github.com/rundeck/go-rundeck/rundeck"
import "github.com/rundeck/go-rundeck/rundeck/auth"

func main() {
    cl := rundeck.NewWithBaseURI("https://127.0.0.1:4440/api/26")   
    cl.Client.Authorizer = &auth.TokenAuthorizer{Token: "ABCDEFG"}  
    ctx := context.Background() 
    sysInfo, _ := cl.SystemInfoGet(ctx)

    fmt.Println(*sysInfo.System.Os.Name)
}
```

## Building

### Pre-requisites
[`DotNet Core SDK`](https://www.microsoft.com/net/download) - Required for the Autorest backend  
`Nodejs/npm` - Required for the Autorest frontend

### Quick Start
```
autorest autorest.md
```
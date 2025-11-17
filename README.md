Rundeck Go SDK
==============

[![Release](https://img.shields.io/github/v/release/rundeck/go-rundeck)](https://github.com/rundeck/go-rundeck/releases)
[![Go Reference](https://pkg.go.dev/badge/github.com/rundeck/go-rundeck/rundeck-v2.svg)](https://pkg.go.dev/github.com/rundeck/go-rundeck/rundeck-v2)
[![Go Report Card](https://goreportcard.com/badge/github.com/rundeck/go-rundeck)](https://goreportcard.com/report/github.com/rundeck/go-rundeck)

Go SDK for the Rundeck / Runbook Automation API, generated from OpenAPI specification.

## Installation

```bash
go get github.com/rundeck/go-rundeck/rundeck-v2@latest
```

Or pin to a specific version:

```bash
go get github.com/rundeck/go-rundeck/rundeck-v2@v1.0.0
```


## Example Usage

```go
import "fmt"

import "github.com/rundeck/go-rundeck/rundeck"
import "github.com/rundeck/go-rundeck/rundeck/auth"

func main() {
    cl := rundeck.NewRundeckWithBaseURI("https://127.0.0.1:4440/api/26")   
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

## Versioning and Releases

This repository uses semantic versioning. Releases are automated via GitHub Actions when version tags are pushed.

### For Maintainers

To create a new release:

```bash
git tag -a v1.0.0 -m "Release v1.0.0"
git push origin v1.0.0
```

See [RELEASING.md](RELEASING.md) for detailed release instructions.

### For Consumers

Use standard Go module versioning:

```go
// go.mod
require (
    github.com/rundeck/go-rundeck/rundeck-v2 v1.0.0
)
```

Or use pseudo-versions for unreleased commits:

```go
github.com/rundeck/go-rundeck/rundeck-v2 v0.0.0-20251115214811-7b8e53bdb31e
```

## SDK Structure

- **rundeck/** - Legacy SDK (AutoRest-based, deprecated)
- **rundeck-v2/** - Current SDK (OpenAPI Generator-based) ⭐

## Contributing

See [RELEASING.md](RELEASING.md) for information about the release process.
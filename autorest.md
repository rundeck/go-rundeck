Rundeck Go SDK
===================================
> see https://aka.ms/autorest

## Getting Started 
To build the SDKs for Rundeck, simply install AutoRest via `npm` (`npm install -g autorest`) and then run:
> `autorest autorest.md`

To see additional help and options, run:
> `autorest --help`

For other options on installation see [Installing AutoRest](https://aka.ms/autorest/install) on the AutoRest github page.

---

## Configuration 
The following are the settings for this using this API with AutoRest.

Defines the Open API spec file(s) to use for input:
```yaml
input-file:
- https://github.com/rundeck/rundeck-api-specs/blob/4f3b7f32eb6e961cc77a9c4f392398787528fd8d/rundeck/execution.yaml
- https://github.com/rundeck/rundeck-api-specs/blob/4f3b7f32eb6e961cc77a9c4f392398787528fd8d/rundeck/job.yaml
- https://github.com/rundeck/rundeck-api-specs/blob/4f3b7f32eb6e961cc77a9c4f392398787528fd8d/rundeck/metric.yaml
- https://github.com/rundeck/rundeck-api-specs/blob/4f3b7f32eb6e961cc77a9c4f392398787528fd8d/rundeck/project.yaml
- https://github.com/rundeck/rundeck-api-specs/blob/4f3b7f32eb6e961cc77a9c4f392398787528fd8d/rundeck/storage.yaml
- https://github.com/rundeck/rundeck-api-specs/blob/4f3b7f32eb6e961cc77a9c4f392398787528fd8d/rundeck/system.yaml
- https://github.com/rundeck/rundeck-api-specs/blob/4f3b7f32eb6e961cc77a9c4f392398787528fd8d/rundeck/user.yaml
```

Sets the generated TypeScript code output directory:
```yaml
go:
  output-folder: rundeck
  namespace: rundeck
  user-agent: Rundeck-SDK-For-Go/version 
  enum-types: true
```

Add credential provider parameter to client constructor:
```yaml
add-credentials: true
```

## TypeScript settings:
```yaml $(go)
use:
- '@microsoft.azure/autorest.go@2.1.131'
```
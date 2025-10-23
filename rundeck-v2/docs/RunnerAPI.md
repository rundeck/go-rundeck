# \RunnerAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CheckPing**](RunnerAPI.md#CheckPing) | **Get** /runnerManagement/checkPing/{token} | Check Runner Ping
[**CreateNoEphemeralReplica**](RunnerAPI.md#CreateNoEphemeralReplica) | **Post** /runnerManagement/runner/{runnerId}/replicas | Create a Runner Replica in no-ephemeral mode
[**CreateProjectNoEphemeralReplica**](RunnerAPI.md#CreateProjectNoEphemeralReplica) | **Post** /project/{project}/runnerManagement/runner/{runnerId}/replicas | Create a Runner Replica without ephemeral mode at project context
[**CreateProjectRunner**](RunnerAPI.md#CreateProjectRunner) | **Post** /project/{project}/runnerManagement/runners | Create a Runner at Project Context
[**CreateRunner**](RunnerAPI.md#CreateRunner) | **Post** /runnerManagement/runners | Create a Runner
[**DeleteProjectRunner**](RunnerAPI.md#DeleteProjectRunner) | **Delete** /project/{project}/runnerManagement/runner/{runnerId} | Delete Runner
[**DeleteProjectRunnerReplica**](RunnerAPI.md#DeleteProjectRunnerReplica) | **Delete** /project/{project}/runnerManagement/runner/{runnerId}/replica/{replicaId} | Delete Runner Replica at Project Context
[**DeleteRunner**](RunnerAPI.md#DeleteRunner) | **Delete** /runnerManagement/runner/{runnerId} | Delete Runner
[**DeleteRunnerReplica**](RunnerAPI.md#DeleteRunnerReplica) | **Delete** /runnerManagement/runner/{runnerId}/replica/{replicaId} | Delete Runner Replica
[**DownloadRunner**](RunnerAPI.md#DownloadRunner) | **Get** /runnerManagement/download/{token} | Download Runner
[**GetRunnerKey**](RunnerAPI.md#GetRunnerKey) | **Get** /runnerManagement/runner/{id}/keys | Get Runner Storage Keys
[**ListProjectAssociatedTags**](RunnerAPI.md#ListProjectAssociatedTags) | **Get** /runnerManagement/tags | List all Tags associated to a project
[**ListProjectRunners**](RunnerAPI.md#ListProjectRunners) | **Get** /project/{project}/runnerManagement/runners | List Runners at project context
[**ListProjectRunnersReplicas**](RunnerAPI.md#ListProjectRunnersReplicas) | **Get** /project/{project}/runnerManagement/runner/{runnerId}/replicas | List Runner Replicas at Project Context
[**ListRunnerTags**](RunnerAPI.md#ListRunnerTags) | **Get** /runnerManagement/runner/{id}/tags | List Runner Tags
[**ListRunners**](RunnerAPI.md#ListRunners) | **Get** /runnerManagement/runners | List Runners
[**ListRunnersReplicas**](RunnerAPI.md#ListRunnersReplicas) | **Get** /runnerManagement/runner/{runnerId}/replicas | List Runner Replicas
[**PingProjectRunner**](RunnerAPI.md#PingProjectRunner) | **Post** /project/{project}/runnerManagement/runner/{id}/ping | Ping a Runner at Project Context
[**PingRunner**](RunnerAPI.md#PingRunner) | **Post** /runnerManagement/runner/{id}/ping | Ping a Runner
[**ProjectCheckPing**](RunnerAPI.md#ProjectCheckPing) | **Get** /project/{project}/runnerManagement/checkPing/{token} | Check Runner Ping at Project Context
[**ProjectContextRunnerConfig**](RunnerAPI.md#ProjectContextRunnerConfig) | **Get** /project/{project}/runnerManagement/config | Get Project Context Runner Configuration
[**ProjectDownloadRunner**](RunnerAPI.md#ProjectDownloadRunner) | **Get** /project/{project}/runnerManagement/download/{token} | Download Runner at Project Context
[**ProjectRunnerInfo**](RunnerAPI.md#ProjectRunnerInfo) | **Get** /project/{project}/runnerManagement/runner/{runnerId} | Get Runner Info at Project Context
[**ProjectUi**](RunnerAPI.md#ProjectUi) | **Get** /project/{project}/runnerManagement/ui | Get UI info for runner management at project context
[**RegenerateProjectRunnerCreds**](RunnerAPI.md#RegenerateProjectRunnerCreds) | **Post** /project/{project}/runnerManagement/runner/{id}/regenerateCreds | Regenerate Runner Creds at Project context
[**RegenerateRunnerCreds**](RunnerAPI.md#RegenerateRunnerCreds) | **Post** /runnerManagement/runner/{id}/regenerateCreds | Regenerate Runner Creds
[**RemoveProjectAssociation**](RunnerAPI.md#RemoveProjectAssociation) | **Post** /project/{project}/runnerManagement/runner/{runnerId}/removeProjectAssociation | Remove Project Association From the Runner
[**RunnerInfo**](RunnerAPI.md#RunnerInfo) | **Get** /runnerManagement/runner/{runnerId} | Get Runner Info
[**SaveProjectContextRunnerConfig**](RunnerAPI.md#SaveProjectContextRunnerConfig) | **Post** /project/{project}/runnerManagement/config | Save Project Context Runner Config
[**SaveProjectRunner**](RunnerAPI.md#SaveProjectRunner) | **Post** /project/{project}/runnerManagement/runner/{runnerId} | Update Runner Definition  at Project context
[**SaveProjectRunnerNodeDispatchSettings**](RunnerAPI.md#SaveProjectRunnerNodeDispatchSettings) | **Post** /project/{project}/runnerManagement/nodeDispatch/config | Update Runner Node Dispatch at project context
[**SaveRunner**](RunnerAPI.md#SaveRunner) | **Post** /runnerManagement/runner/{runnerId} | Update Runner Definition
[**SearchTags**](RunnerAPI.md#SearchTags) | **Get** /runnerTag/searchTags | Search Runner Tags by a keyword
[**StartupOperation**](RunnerAPI.md#StartupOperation) | **Get** /runner/startup | Runner: Init agent process to register replicas [Enterprise Runner]
[**Ui**](RunnerAPI.md#Ui) | **Get** /runnerManagement/ui | Get UI info for runner management



## CheckPing

> PingResponse CheckPing(ctx, token).Execute()

Check Runner Ping



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	token := "token_example" // string | Ping Token

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.CheckPing(context.Background(), token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.CheckPing``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CheckPing`: PingResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.CheckPing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**token** | **string** | Ping Token | 

### Other Parameters

Other parameters are passed through a pointer to a apiCheckPingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**PingResponse**](PingResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateNoEphemeralReplica

> NewRunnerReplicaResponse CreateNoEphemeralReplica(ctx, runnerId).Execute()

Create a Runner Replica in no-ephemeral mode



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	runnerId := "runnerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.CreateNoEphemeralReplica(context.Background(), runnerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.CreateNoEphemeralReplica``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateNoEphemeralReplica`: NewRunnerReplicaResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.CreateNoEphemeralReplica`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**runnerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateNoEphemeralReplicaRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**NewRunnerReplicaResponse**](NewRunnerReplicaResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateProjectNoEphemeralReplica

> NewRunnerReplicaResponse CreateProjectNoEphemeralReplica(ctx, project, runnerId).Execute()

Create a Runner Replica without ephemeral mode at project context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	runnerId := "runnerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.CreateProjectNoEphemeralReplica(context.Background(), project, runnerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.CreateProjectNoEphemeralReplica``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateProjectNoEphemeralReplica`: NewRunnerReplicaResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.CreateProjectNoEphemeralReplica`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 
**runnerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateProjectNoEphemeralReplicaRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**NewRunnerReplicaResponse**](NewRunnerReplicaResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateProjectRunner

> NewRunnerResponse CreateProjectRunner(ctx, project).CreateProjectRunnerRequest(createProjectRunnerRequest).Execute()

Create a Runner at Project Context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	createProjectRunnerRequest := *openapiclient.NewCreateProjectRunnerRequest("Name_example", "Description_example") // CreateProjectRunnerRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.CreateProjectRunner(context.Background(), project).CreateProjectRunnerRequest(createProjectRunnerRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.CreateProjectRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateProjectRunner`: NewRunnerResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.CreateProjectRunner`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateProjectRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createProjectRunnerRequest** | [**CreateProjectRunnerRequest**](CreateProjectRunnerRequest.md) |  | 

### Return type

[**NewRunnerResponse**](NewRunnerResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateRunner

> NewRunnerResponse CreateRunner(ctx).CreateProjectRunnerRequest(createProjectRunnerRequest).Execute()

Create a Runner



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	createProjectRunnerRequest := *openapiclient.NewCreateProjectRunnerRequest("Name_example", "Description_example") // CreateProjectRunnerRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.CreateRunner(context.Background()).CreateProjectRunnerRequest(createProjectRunnerRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.CreateRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRunner`: NewRunnerResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.CreateRunner`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createProjectRunnerRequest** | [**CreateProjectRunnerRequest**](CreateProjectRunnerRequest.md) |  | 

### Return type

[**NewRunnerResponse**](NewRunnerResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteProjectRunner

> DeleteProjectRunner(ctx, project, runnerId).Execute()

Delete Runner



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	runnerId := "runnerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RunnerAPI.DeleteProjectRunner(context.Background(), project, runnerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.DeleteProjectRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 
**runnerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteProjectRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteProjectRunnerReplica

> DeleteProjectRunnerReplica(ctx, project, runnerId, replicaId).Execute()

Delete Runner Replica at Project Context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	runnerId := "runnerId_example" // string | 
	replicaId := "replicaId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RunnerAPI.DeleteProjectRunnerReplica(context.Background(), project, runnerId, replicaId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.DeleteProjectRunnerReplica``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 
**runnerId** | **string** |  | 
**replicaId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteProjectRunnerReplicaRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteRunner

> DeleteRunner(ctx, runnerId).Execute()

Delete Runner



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	runnerId := "runnerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RunnerAPI.DeleteRunner(context.Background(), runnerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.DeleteRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**runnerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteRunnerReplica

> DeleteRunnerReplica(ctx, runnerId, replicaId).Execute()

Delete Runner Replica



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	runnerId := "runnerId_example" // string | 
	replicaId := "replicaId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RunnerAPI.DeleteRunnerReplica(context.Background(), runnerId, replicaId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.DeleteRunnerReplica``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**runnerId** | **string** |  | 
**replicaId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteRunnerReplicaRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DownloadRunner

> DownloadRunner(ctx, token).Execute()

Download Runner



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	token := "token_example" // string | Download Token

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RunnerAPI.DownloadRunner(context.Background(), token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.DownloadRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**token** | **string** | Download Token | 

### Other Parameters

Other parameters are passed through a pointer to a apiDownloadRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/java-archive

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetRunnerKey

> TagCountResponse GetRunnerKey(ctx, id).Path(path).Refresh(refresh).Execute()

Get Runner Storage Keys



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	id := "id_example" // string | runner id
	path := "path_example" // string | key path (optional)
	refresh := true // bool | key path (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.GetRunnerKey(context.Background(), id).Path(path).Refresh(refresh).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.GetRunnerKey``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRunnerKey`: TagCountResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.GetRunnerKey`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | runner id | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRunnerKeyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **path** | **string** | key path | 
 **refresh** | **bool** | key path | 

### Return type

[**TagCountResponse**](TagCountResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListProjectAssociatedTags

> TagCountResponse ListProjectAssociatedTags(ctx).Project(project).Execute()

List all Tags associated to a project



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | Project Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ListProjectAssociatedTags(context.Background()).Project(project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ListProjectAssociatedTags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListProjectAssociatedTags`: TagCountResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ListProjectAssociatedTags`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListProjectAssociatedTagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | **string** | Project Name | 

### Return type

[**TagCountResponse**](TagCountResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListProjectRunners

> RunnerList ListProjectRunners(ctx, project).Tags(tags).LocalOnly(localOnly).Filter(filter).Status(status).Execute()

List Runners at project context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	tags := "tags_example" // string | List of tags (optional)
	localOnly := true // bool | Include local runner only (optional)
	filter := "filter_example" // string | Use filter string (optional)
	status := "status_example" // string | Filter by runner status (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ListProjectRunners(context.Background(), project).Tags(tags).LocalOnly(localOnly).Filter(filter).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ListProjectRunners``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListProjectRunners`: RunnerList
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ListProjectRunners`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListProjectRunnersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **tags** | **string** | List of tags | 
 **localOnly** | **bool** | Include local runner only | 
 **filter** | **string** | Use filter string | 
 **status** | **string** | Filter by runner status | 

### Return type

[**RunnerList**](RunnerList.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListProjectRunnersReplicas

> RunnerReplicaList ListProjectRunnersReplicas(ctx, project, runnerId).Execute()

List Runner Replicas at Project Context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	runnerId := "runnerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ListProjectRunnersReplicas(context.Background(), project, runnerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ListProjectRunnersReplicas``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListProjectRunnersReplicas`: RunnerReplicaList
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ListProjectRunnersReplicas`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 
**runnerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListProjectRunnersReplicasRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**RunnerReplicaList**](RunnerReplicaList.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRunnerTags

> []string ListRunnerTags(ctx, id).Execute()

List Runner Tags



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	id := "id_example" // string | Runner ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ListRunnerTags(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ListRunnerTags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRunnerTags`: []string
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ListRunnerTags`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Runner ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiListRunnerTagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**[]string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRunners

> RunnerList ListRunners(ctx).Tags(tags).LocalOnly(localOnly).Filter(filter).Status(status).Execute()

List Runners



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	tags := "tags_example" // string | List of tags (optional)
	localOnly := true // bool | Include local runner only (optional)
	filter := "filter_example" // string | Use filter string (optional)
	status := "status_example" // string | Filter by runner status (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ListRunners(context.Background()).Tags(tags).LocalOnly(localOnly).Filter(filter).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ListRunners``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRunners`: RunnerList
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ListRunners`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListRunnersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tags** | **string** | List of tags | 
 **localOnly** | **bool** | Include local runner only | 
 **filter** | **string** | Use filter string | 
 **status** | **string** | Filter by runner status | 

### Return type

[**RunnerList**](RunnerList.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRunnersReplicas

> RunnerReplicaList ListRunnersReplicas(ctx, runnerId).Execute()

List Runner Replicas



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	runnerId := "runnerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ListRunnersReplicas(context.Background(), runnerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ListRunnersReplicas``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRunnersReplicas`: RunnerReplicaList
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ListRunnersReplicas`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**runnerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListRunnersReplicasRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RunnerReplicaList**](RunnerReplicaList.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PingProjectRunner

> PingTokenResponse PingProjectRunner(ctx, id, project).Execute()

Ping a Runner at Project Context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	id := "id_example" // string | Runner ID
	project := "project_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.PingProjectRunner(context.Background(), id, project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.PingProjectRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PingProjectRunner`: PingTokenResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.PingProjectRunner`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Runner ID | 
**project** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPingProjectRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**PingTokenResponse**](PingTokenResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PingRunner

> PingTokenResponse PingRunner(ctx, id).Execute()

Ping a Runner



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	id := "id_example" // string | Runner ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.PingRunner(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.PingRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PingRunner`: PingTokenResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.PingRunner`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Runner ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiPingRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**PingTokenResponse**](PingTokenResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ProjectCheckPing

> PingResponse ProjectCheckPing(ctx, token, project).Execute()

Check Runner Ping at Project Context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	token := "token_example" // string | Ping Token
	project := "project_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ProjectCheckPing(context.Background(), token, project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ProjectCheckPing``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ProjectCheckPing`: PingResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ProjectCheckPing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**token** | **string** | Ping Token | 
**project** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiProjectCheckPingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**PingResponse**](PingResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ProjectContextRunnerConfig

> ProjectContextRunnerConfig ProjectContextRunnerConfig(ctx, project).Execute()

Get Project Context Runner Configuration



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | Project Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ProjectContextRunnerConfig(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ProjectContextRunnerConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ProjectContextRunnerConfig`: ProjectContextRunnerConfig
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ProjectContextRunnerConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiProjectContextRunnerConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ProjectContextRunnerConfig**](ProjectContextRunnerConfig.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ProjectDownloadRunner

> ProjectDownloadRunner(ctx, token, project).Execute()

Download Runner at Project Context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	token := "token_example" // string | Download Token
	project := "project_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RunnerAPI.ProjectDownloadRunner(context.Background(), token, project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ProjectDownloadRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**token** | **string** | Download Token | 
**project** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiProjectDownloadRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/java-archive

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ProjectRunnerInfo

> RunnerInfo ProjectRunnerInfo(ctx, runnerId, project).Execute()

Get Runner Info at Project Context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	runnerId := "runnerId_example" // string | Runner ID
	project := "project_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ProjectRunnerInfo(context.Background(), runnerId, project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ProjectRunnerInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ProjectRunnerInfo`: RunnerInfo
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ProjectRunnerInfo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**runnerId** | **string** | Runner ID | 
**project** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiProjectRunnerInfoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**RunnerInfo**](RunnerInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ProjectUi

> UiData ProjectUi(ctx, project).Execute()

Get UI info for runner management at project context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.ProjectUi(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.ProjectUi``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ProjectUi`: UiData
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.ProjectUi`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiProjectUiRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**UiData**](UiData.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegenerateProjectRunnerCreds

> RegenRunnerCredResponse RegenerateProjectRunnerCreds(ctx, project, id).Execute()

Regenerate Runner Creds at Project context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.RegenerateProjectRunnerCreds(context.Background(), project, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.RegenerateProjectRunnerCreds``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegenerateProjectRunnerCreds`: RegenRunnerCredResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.RegenerateProjectRunnerCreds`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRegenerateProjectRunnerCredsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**RegenRunnerCredResponse**](RegenRunnerCredResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegenerateRunnerCreds

> RegenRunnerCredResponse RegenerateRunnerCreds(ctx, id).Execute()

Regenerate Runner Creds



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.RegenerateRunnerCreds(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.RegenerateRunnerCreds``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegenerateRunnerCreds`: RegenRunnerCredResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.RegenerateRunnerCreds`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRegenerateRunnerCredsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RegenRunnerCredResponse**](RegenRunnerCredResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveProjectAssociation

> RunnerInfo RemoveProjectAssociation(ctx, project, runnerId).UpdateRunnerRequest(updateRunnerRequest).Execute()

Remove Project Association From the Runner



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	runnerId := "runnerId_example" // string | 
	updateRunnerRequest := *openapiclient.NewUpdateRunnerRequest("RunnerId_example") // UpdateRunnerRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.RemoveProjectAssociation(context.Background(), project, runnerId).UpdateRunnerRequest(updateRunnerRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.RemoveProjectAssociation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RemoveProjectAssociation`: RunnerInfo
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.RemoveProjectAssociation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 
**runnerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveProjectAssociationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateRunnerRequest** | [**UpdateRunnerRequest**](UpdateRunnerRequest.md) |  | 

### Return type

[**RunnerInfo**](RunnerInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RunnerInfo

> RunnerInfo RunnerInfo(ctx, runnerId).Execute()

Get Runner Info



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	runnerId := "runnerId_example" // string | Runner ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.RunnerInfo(context.Background(), runnerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.RunnerInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RunnerInfo`: RunnerInfo
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.RunnerInfo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**runnerId** | **string** | Runner ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiRunnerInfoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RunnerInfo**](RunnerInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SaveProjectContextRunnerConfig

> ProjectContextRunnerConfig SaveProjectContextRunnerConfig(ctx, project).SaveProjectContextRunnerConfigRequest(saveProjectContextRunnerConfigRequest).Execute()

Save Project Context Runner Config



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | Project Name
	saveProjectContextRunnerConfigRequest := *openapiclient.NewSaveProjectContextRunnerConfigRequest() // SaveProjectContextRunnerConfigRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.SaveProjectContextRunnerConfig(context.Background(), project).SaveProjectContextRunnerConfigRequest(saveProjectContextRunnerConfigRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.SaveProjectContextRunnerConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SaveProjectContextRunnerConfig`: ProjectContextRunnerConfig
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.SaveProjectContextRunnerConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiSaveProjectContextRunnerConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **saveProjectContextRunnerConfigRequest** | [**SaveProjectContextRunnerConfigRequest**](SaveProjectContextRunnerConfigRequest.md) |  | 

### Return type

[**ProjectContextRunnerConfig**](ProjectContextRunnerConfig.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SaveProjectRunner

> RunnerInfo SaveProjectRunner(ctx, project, runnerId).SaveProjectRunnerRequest(saveProjectRunnerRequest).Execute()

Update Runner Definition  at Project context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	runnerId := "runnerId_example" // string | 
	saveProjectRunnerRequest := *openapiclient.NewSaveProjectRunnerRequest("RunnerId_example") // SaveProjectRunnerRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.SaveProjectRunner(context.Background(), project, runnerId).SaveProjectRunnerRequest(saveProjectRunnerRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.SaveProjectRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SaveProjectRunner`: RunnerInfo
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.SaveProjectRunner`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 
**runnerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSaveProjectRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **saveProjectRunnerRequest** | [**SaveProjectRunnerRequest**](SaveProjectRunnerRequest.md) |  | 

### Return type

[**RunnerInfo**](RunnerInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SaveProjectRunnerNodeDispatchSettings

> RunnerInfo SaveProjectRunnerNodeDispatchSettings(ctx, project).SaveProjectRunnerNodeDispatchSettingsRequest(saveProjectRunnerNodeDispatchSettingsRequest).Execute()

Update Runner Node Dispatch at project context



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	project := "project_example" // string | 
	saveProjectRunnerNodeDispatchSettingsRequest := *openapiclient.NewSaveProjectRunnerNodeDispatchSettingsRequest("RunnerId_example") // SaveProjectRunnerNodeDispatchSettingsRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.SaveProjectRunnerNodeDispatchSettings(context.Background(), project).SaveProjectRunnerNodeDispatchSettingsRequest(saveProjectRunnerNodeDispatchSettingsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.SaveProjectRunnerNodeDispatchSettings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SaveProjectRunnerNodeDispatchSettings`: RunnerInfo
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.SaveProjectRunnerNodeDispatchSettings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSaveProjectRunnerNodeDispatchSettingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **saveProjectRunnerNodeDispatchSettingsRequest** | [**SaveProjectRunnerNodeDispatchSettingsRequest**](SaveProjectRunnerNodeDispatchSettingsRequest.md) |  | 

### Return type

[**RunnerInfo**](RunnerInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SaveRunner

> RunnerInfo SaveRunner(ctx, runnerId).SaveProjectRunnerRequest(saveProjectRunnerRequest).Execute()

Update Runner Definition



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	runnerId := "runnerId_example" // string | 
	saveProjectRunnerRequest := *openapiclient.NewSaveProjectRunnerRequest("RunnerId_example") // SaveProjectRunnerRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.SaveRunner(context.Background(), runnerId).SaveProjectRunnerRequest(saveProjectRunnerRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.SaveRunner``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SaveRunner`: RunnerInfo
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.SaveRunner`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**runnerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSaveRunnerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **saveProjectRunnerRequest** | [**SaveProjectRunnerRequest**](SaveProjectRunnerRequest.md) |  | 

### Return type

[**RunnerInfo**](RunnerInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SearchTags

> []string SearchTags(ctx).Keyword(keyword).Offset(offset).Limit(limit).Execute()

Search Runner Tags by a keyword



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	keyword := "keyword_example" // string | Keyword (optional)
	offset := int32(56) // int32 | Offset from the start of the result set. Used for pagination. (optional)
	limit := int32(56) // int32 | Limit the size of the returned result set. Used for pagination. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.SearchTags(context.Background()).Keyword(keyword).Offset(offset).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.SearchTags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchTags`: []string
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.SearchTags`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSearchTagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **keyword** | **string** | Keyword | 
 **offset** | **int32** | Offset from the start of the result set. Used for pagination. | 
 **limit** | **int32** | Limit the size of the returned result set. Used for pagination. | 

### Return type

**[]string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StartupOperation

> StartUpResponse StartupOperation(ctx).Execute()

Runner: Init agent process to register replicas [Enterprise Runner]



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.StartupOperation(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.StartupOperation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StartupOperation`: StartUpResponse
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.StartupOperation`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiStartupOperationRequest struct via the builder pattern


### Return type

[**StartUpResponse**](StartUpResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Ui

> UiData Ui(ctx).Execute()

Get UI info for runner management



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RunnerAPI.Ui(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RunnerAPI.Ui``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Ui`: UiData
	fmt.Fprintf(os.Stdout, "Response from `RunnerAPI.Ui`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiUiRequest struct via the builder pattern


### Return type

[**UiData**](UiData.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


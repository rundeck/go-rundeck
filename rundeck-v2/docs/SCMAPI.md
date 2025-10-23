# \SCMAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiJobActionInput**](SCMAPI.md#ApiJobActionInput) | **Get** /job/{id}/scm/{integration}/action/{actionId}/input | Get Job SCM Action Input Fields
[**ApiJobActionPerform**](SCMAPI.md#ApiJobActionPerform) | **Post** /job/{id}/scm/{integration}/action/{actionId} | Perform Job SCM Action
[**ApiJobDiff**](SCMAPI.md#ApiJobDiff) | **Get** /job/{id}/scm/{integration}/diff | Get Job SCM Diff
[**ApiJobStatus**](SCMAPI.md#ApiJobStatus) | **Get** /job/{id}/scm/{integration}/status | Get Job SCM Status
[**ApiPluginInput**](SCMAPI.md#ApiPluginInput) | **Get** /project/{project}/scm/{integration}/plugin/{type}/input | Get SCM Plugin Input Fields
[**ApiPlugins**](SCMAPI.md#ApiPlugins) | **Get** /project/{project}/scm/{integration}/plugins | List SCM Plugins
[**ApiProjectActionInput**](SCMAPI.md#ApiProjectActionInput) | **Get** /project/{project}/scm/{integration}/action/{actionId}/input | Get Project SCM Action Input Fields
[**ApiProjectActionPerform**](SCMAPI.md#ApiProjectActionPerform) | **Post** /project/{project}/scm/{integration}/action/{actionId} | Perform Project SCM Action
[**ApiProjectConfig**](SCMAPI.md#ApiProjectConfig) | **Get** /project/{project}/scm/{integration}/config | Get Project SCM Config
[**ApiProjectDisable**](SCMAPI.md#ApiProjectDisable) | **Post** /project/{project}/scm/{integration}/plugin/{type}/disable | Disable SCM Plugin for a Project
[**ApiProjectEnable**](SCMAPI.md#ApiProjectEnable) | **Post** /project/{project}/scm/{integration}/plugin/{type}/enable | Enable SCM Plugin for a Project
[**ApiProjectSetup**](SCMAPI.md#ApiProjectSetup) | **Post** /project/{project}/scm/{integration}/plugin/{type}/setup | Setup SCM Plugin for a Project
[**ApiProjectStatus**](SCMAPI.md#ApiProjectStatus) | **Get** /project/{project}/scm/{integration}/status | Get Project SCM Status
[**ApiProjectToggleSCM**](SCMAPI.md#ApiProjectToggleSCM) | **Post** /project/{project}/scm/toggle | Toggle SCM for a Project



## ApiJobActionInput

> ScmActionInput ApiJobActionInput(ctx, id, integration, actionId).Execute()

Get Job SCM Action Input Fields



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	id := "id_example" // string | Job ID
	integration := "integration_example" // string | SCM integration type
	actionId := "actionId_example" // string | Action Name/ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiJobActionInput(context.Background(), id, integration, actionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiJobActionInput``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobActionInput`: ScmActionInput
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiJobActionInput`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 
**integration** | **string** | SCM integration type | 
**actionId** | **string** | Action Name/ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobActionInputRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ScmActionInput**](ScmActionInput.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobActionPerform

> ScmActionResult ApiJobActionPerform(ctx, id, integration, actionId).Body(body).Execute()

Perform Job SCM Action



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	id := "id_example" // string | Job ID
	integration := "integration_example" // string | SCM integration type
	actionId := "actionId_example" // string | Action Name/ID
	body := map[string]interface{}{ ... } // map[string]interface{} | SCM Action Input Request.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiJobActionPerform(context.Background(), id, integration, actionId).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiJobActionPerform``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobActionPerform`: ScmActionResult
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiJobActionPerform`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 
**integration** | **string** | SCM integration type | 
**actionId** | **string** | Action Name/ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobActionPerformRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | **map[string]interface{}** | SCM Action Input Request. | 

### Return type

[**ScmActionResult**](ScmActionResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobDiff

> ScmJobDiff ApiJobDiff(ctx, id, integration).Execute()

Get Job SCM Diff



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	id := "id_example" // string | Job ID
	integration := "integration_example" // string | SCM integration type

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiJobDiff(context.Background(), id, integration).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiJobDiff``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobDiff`: ScmJobDiff
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiJobDiff`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 
**integration** | **string** | SCM integration type | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobDiffRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ScmJobDiff**](ScmJobDiff.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobStatus

> ScmJobStatus ApiJobStatus(ctx, id, integration).Execute()

Get Job SCM Status



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	id := "id_example" // string | Job ID
	integration := "integration_example" // string | SCM integration type

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiJobStatus(context.Background(), id, integration).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiJobStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobStatus`: ScmJobStatus
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiJobStatus`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 
**integration** | **string** | SCM integration type | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobStatusRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ScmJobStatus**](ScmJobStatus.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiPluginInput

> ScmPluginSetupInput ApiPluginInput(ctx, project, integration, type_).Execute()

Get SCM Plugin Input Fields



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	integration := "integration_example" // string | Integration Name
	type_ := "type__example" // string | Plugin Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiPluginInput(context.Background(), project, integration, type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiPluginInput``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiPluginInput`: ScmPluginSetupInput
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiPluginInput`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**integration** | **string** | Integration Name | 
**type_** | **string** | Plugin Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiPluginInputRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ScmPluginSetupInput**](ScmPluginSetupInput.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiPlugins

> ScmPluginList ApiPlugins(ctx, project, integration).Execute()

List SCM Plugins



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	integration := "integration_example" // string | Integration Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiPlugins(context.Background(), project, integration).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiPlugins``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiPlugins`: ScmPluginList
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiPlugins`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**integration** | **string** | Integration Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiPluginsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ScmPluginList**](ScmPluginList.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectActionInput

> ScmActionInput ApiProjectActionInput(ctx, project, integration, actionId).Execute()

Get Project SCM Action Input Fields



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	integration := "integration_example" // string | Integration Name
	actionId := "actionId_example" // string | Action ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiProjectActionInput(context.Background(), project, integration, actionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiProjectActionInput``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectActionInput`: ScmActionInput
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiProjectActionInput`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**integration** | **string** | Integration Name | 
**actionId** | **string** | Action ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectActionInputRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ScmActionInput**](ScmActionInput.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectActionPerform

> ScmActionResult ApiProjectActionPerform(ctx, project, integration, actionId).ScmAction(scmAction).Execute()

Perform Project SCM Action



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	integration := "integration_example" // string | Integration Name
	actionId := "actionId_example" // string | Action ID
	scmAction := *openapiclient.NewScmAction() // ScmAction | Perform Action Request

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiProjectActionPerform(context.Background(), project, integration, actionId).ScmAction(scmAction).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiProjectActionPerform``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectActionPerform`: ScmActionResult
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiProjectActionPerform`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**integration** | **string** | Integration Name | 
**actionId** | **string** | Action ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectActionPerformRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **scmAction** | [**ScmAction**](ScmAction.md) | Perform Action Request | 

### Return type

[**ScmActionResult**](ScmActionResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectConfig

> ScmProjectPluginConfig ApiProjectConfig(ctx, project, integration).Execute()

Get Project SCM Config



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	integration := "integration_example" // string | Integration Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiProjectConfig(context.Background(), project, integration).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiProjectConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectConfig`: ScmProjectPluginConfig
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiProjectConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**integration** | **string** | Integration Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ScmProjectPluginConfig**](ScmProjectPluginConfig.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectDisable

> ScmActionResult ApiProjectDisable(ctx, project, integration, type_).Execute()

Disable SCM Plugin for a Project



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	integration := "integration_example" // string | Integration Name
	type_ := "type__example" // string | Plugin Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiProjectDisable(context.Background(), project, integration, type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiProjectDisable``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectDisable`: ScmActionResult
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiProjectDisable`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**integration** | **string** | Integration Name | 
**type_** | **string** | Plugin Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectDisableRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ScmActionResult**](ScmActionResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectEnable

> ScmActionResult ApiProjectEnable(ctx, project, integration, type_).Execute()

Enable SCM Plugin for a Project



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	integration := "integration_example" // string | Integration Name
	type_ := "type__example" // string | Plugin Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiProjectEnable(context.Background(), project, integration, type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiProjectEnable``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectEnable`: ScmActionResult
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiProjectEnable`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**integration** | **string** | Integration Name | 
**type_** | **string** | Plugin Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectEnableRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ScmActionResult**](ScmActionResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectSetup

> ScmActionResult ApiProjectSetup(ctx, project, integration, type_).Body(body).Execute()

Setup SCM Plugin for a Project



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	integration := "integration_example" // string | Integration Name
	type_ := "type__example" // string | Plugin Name
	body := map[string]interface{}{ ... } // map[string]interface{} | Configuration values for the plugin. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiProjectSetup(context.Background(), project, integration, type_).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiProjectSetup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectSetup`: ScmActionResult
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiProjectSetup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**integration** | **string** | Integration Name | 
**type_** | **string** | Plugin Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectSetupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | **map[string]interface{}** | Configuration values for the plugin. | 

### Return type

[**ScmActionResult**](ScmActionResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectStatus

> ScmProjectStatus ApiProjectStatus(ctx, project, integration).Execute()

Get Project SCM Status



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	integration := "integration_example" // string | Integration Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiProjectStatus(context.Background(), project, integration).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiProjectStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectStatus`: ScmProjectStatus
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiProjectStatus`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**integration** | **string** | Integration Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectStatusRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ScmProjectStatus**](ScmProjectStatus.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectToggleSCM

> ScmToggleResponse ApiProjectToggleSCM(ctx, project).ScmToggleRequest(scmToggleRequest).Execute()

Toggle SCM for a Project



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	project := "project_example" // string | Project Name
	scmToggleRequest := *openapiclient.NewScmToggleRequest() // ScmToggleRequest | Configuration values for the plugin. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SCMAPI.ApiProjectToggleSCM(context.Background(), project).ScmToggleRequest(scmToggleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SCMAPI.ApiProjectToggleSCM``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectToggleSCM`: ScmToggleResponse
	fmt.Fprintf(os.Stdout, "Response from `SCMAPI.ApiProjectToggleSCM`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectToggleSCMRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **scmToggleRequest** | [**ScmToggleRequest**](ScmToggleRequest.md) | Configuration values for the plugin. | 

### Return type

[**ScmToggleResponse**](ScmToggleResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


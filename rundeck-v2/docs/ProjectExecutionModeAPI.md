# \ProjectExecutionModeAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiProjectDisableLater**](ProjectExecutionModeAPI.md#ApiProjectDisableLater) | **Post** /project/{project}/disable/later | Disable Project executions or schedules after a duration of time
[**ApiProjectEnableLater**](ProjectExecutionModeAPI.md#ApiProjectEnableLater) | **Post** /project/{project}/enable/later | Enable Project executions or schedules after a duration of time



## ApiProjectDisableLater

> ModeLaterResponse ApiProjectDisableLater(ctx, project).ProjectModeLaterRequest(projectModeLaterRequest).Execute()

Disable Project executions or schedules after a duration of time



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
	project := "project_example" // string | project name
	projectModeLaterRequest := *openapiclient.NewProjectModeLaterRequest() // ProjectModeLaterRequest | Disable Schedule or Executions. Specify the `type` to enable, and a `value` with a time duration expression. The request must contain a `value` with a \"Time duration expression\". (See request schema for syntax.) 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectExecutionModeAPI.ApiProjectDisableLater(context.Background(), project).ProjectModeLaterRequest(projectModeLaterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectExecutionModeAPI.ApiProjectDisableLater``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectDisableLater`: ModeLaterResponse
	fmt.Fprintf(os.Stdout, "Response from `ProjectExecutionModeAPI.ApiProjectDisableLater`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | project name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectDisableLaterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **projectModeLaterRequest** | [**ProjectModeLaterRequest**](ProjectModeLaterRequest.md) | Disable Schedule or Executions. Specify the &#x60;type&#x60; to enable, and a &#x60;value&#x60; with a time duration expression. The request must contain a &#x60;value&#x60; with a \&quot;Time duration expression\&quot;. (See request schema for syntax.)  | 

### Return type

[**ModeLaterResponse**](ModeLaterResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectEnableLater

> ModeLaterResponse ApiProjectEnableLater(ctx, project).ProjectModeLaterRequest(projectModeLaterRequest).Execute()

Enable Project executions or schedules after a duration of time



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
	project := "project_example" // string | project name
	projectModeLaterRequest := *openapiclient.NewProjectModeLaterRequest() // ProjectModeLaterRequest | Enable Schedule or Executions. Specify the `type` to enable, and a `value` with a time duration expression. The request must contain a `value` with a \"Time duration expression\". (See request schema for syntax.) 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectExecutionModeAPI.ApiProjectEnableLater(context.Background(), project).ProjectModeLaterRequest(projectModeLaterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectExecutionModeAPI.ApiProjectEnableLater``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectEnableLater`: ModeLaterResponse
	fmt.Fprintf(os.Stdout, "Response from `ProjectExecutionModeAPI.ApiProjectEnableLater`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | project name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectEnableLaterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **projectModeLaterRequest** | [**ProjectModeLaterRequest**](ProjectModeLaterRequest.md) | Enable Schedule or Executions. Specify the &#x60;type&#x60; to enable, and a &#x60;value&#x60; with a time duration expression. The request must contain a &#x60;value&#x60; with a \&quot;Time duration expression\&quot;. (See request schema for syntax.)  | 

### Return type

[**ModeLaterResponse**](ModeLaterResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


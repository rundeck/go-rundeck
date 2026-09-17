# \ExecutionModeAPI

All URIs are relative to *https://localhost:4440/api/59*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiExecutionModeLaterActive**](ExecutionModeAPI.md#ApiExecutionModeLaterActive) | **Post** /system/executions/enable/later | Enable System executions after a duration of time
[**ApiExecutionModeLaterPassive**](ExecutionModeAPI.md#ApiExecutionModeLaterPassive) | **Post** /system/executions/disable/later | Disable System executions after a duration of time
[**ApiProjectDisableLater**](ExecutionModeAPI.md#ApiProjectDisableLater) | **Post** /project/{project}/disable/later | Disable Project executions or schedules after a duration of time
[**ApiProjectEnableLater**](ExecutionModeAPI.md#ApiProjectEnableLater) | **Post** /project/{project}/enable/later | Enable Project executions or schedules after a duration of time



## ApiExecutionModeLaterActive

> ModeLaterResponse ApiExecutionModeLaterActive(ctx).ApiExecutionModeLaterPassiveRequest(apiExecutionModeLaterPassiveRequest).Execute()

Enable System executions after a duration of time



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
	apiExecutionModeLaterPassiveRequest := *openapiclient.NewApiExecutionModeLaterPassiveRequest() // ApiExecutionModeLaterPassiveRequest | Enable Executions. Specify a `value` with a time duration expression. (See request schema for syntax.) 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ExecutionModeAPI.ApiExecutionModeLaterActive(context.Background()).ApiExecutionModeLaterPassiveRequest(apiExecutionModeLaterPassiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ExecutionModeAPI.ApiExecutionModeLaterActive``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionModeLaterActive`: ModeLaterResponse
	fmt.Fprintf(os.Stdout, "Response from `ExecutionModeAPI.ApiExecutionModeLaterActive`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionModeLaterActiveRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiExecutionModeLaterPassiveRequest** | [**ApiExecutionModeLaterPassiveRequest**](ApiExecutionModeLaterPassiveRequest.md) | Enable Executions. Specify a &#x60;value&#x60; with a time duration expression. (See request schema for syntax.)  | 

### Return type

[**ModeLaterResponse**](ModeLaterResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionModeLaterPassive

> ModeLaterResponse ApiExecutionModeLaterPassive(ctx).ApiExecutionModeLaterPassiveRequest(apiExecutionModeLaterPassiveRequest).Execute()

Disable System executions after a duration of time



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
	apiExecutionModeLaterPassiveRequest := *openapiclient.NewApiExecutionModeLaterPassiveRequest() // ApiExecutionModeLaterPassiveRequest | Disable Executions. Specify a `value` with a time duration expression. (See request schema for syntax.) 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ExecutionModeAPI.ApiExecutionModeLaterPassive(context.Background()).ApiExecutionModeLaterPassiveRequest(apiExecutionModeLaterPassiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ExecutionModeAPI.ApiExecutionModeLaterPassive``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionModeLaterPassive`: ModeLaterResponse
	fmt.Fprintf(os.Stdout, "Response from `ExecutionModeAPI.ApiExecutionModeLaterPassive`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionModeLaterPassiveRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiExecutionModeLaterPassiveRequest** | [**ApiExecutionModeLaterPassiveRequest**](ApiExecutionModeLaterPassiveRequest.md) | Disable Executions. Specify a &#x60;value&#x60; with a time duration expression. (See request schema for syntax.)  | 

### Return type

[**ModeLaterResponse**](ModeLaterResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectDisableLater

> ModeLaterResponse ApiProjectDisableLater(ctx, project).ApiProjectDisableLaterRequest(apiProjectDisableLaterRequest).Execute()

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
	apiProjectDisableLaterRequest := *openapiclient.NewApiProjectDisableLaterRequest() // ApiProjectDisableLaterRequest | Disable Schedule or Executions. Specify the `type` to enable, and a `value` with a time duration expression. The request must contain a `value` with a \"Time duration expression\". (See request schema for syntax.) 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ExecutionModeAPI.ApiProjectDisableLater(context.Background(), project).ApiProjectDisableLaterRequest(apiProjectDisableLaterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ExecutionModeAPI.ApiProjectDisableLater``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectDisableLater`: ModeLaterResponse
	fmt.Fprintf(os.Stdout, "Response from `ExecutionModeAPI.ApiProjectDisableLater`: %v\n", resp)
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

 **apiProjectDisableLaterRequest** | [**ApiProjectDisableLaterRequest**](ApiProjectDisableLaterRequest.md) | Disable Schedule or Executions. Specify the &#x60;type&#x60; to enable, and a &#x60;value&#x60; with a time duration expression. The request must contain a &#x60;value&#x60; with a \&quot;Time duration expression\&quot;. (See request schema for syntax.)  | 

### Return type

[**ModeLaterResponse**](ModeLaterResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectEnableLater

> ModeLaterResponse ApiProjectEnableLater(ctx, project).ApiProjectDisableLaterRequest(apiProjectDisableLaterRequest).Execute()

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
	apiProjectDisableLaterRequest := *openapiclient.NewApiProjectDisableLaterRequest() // ApiProjectDisableLaterRequest | Enable Schedule or Executions. Specify the `type` to enable, and a `value` with a time duration expression. The request must contain a `value` with a \"Time duration expression\". (See request schema for syntax.) 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ExecutionModeAPI.ApiProjectEnableLater(context.Background(), project).ApiProjectDisableLaterRequest(apiProjectDisableLaterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ExecutionModeAPI.ApiProjectEnableLater``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectEnableLater`: ModeLaterResponse
	fmt.Fprintf(os.Stdout, "Response from `ExecutionModeAPI.ApiProjectEnableLater`: %v\n", resp)
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

 **apiProjectDisableLaterRequest** | [**ApiProjectDisableLaterRequest**](ApiProjectDisableLaterRequest.md) | Enable Schedule or Executions. Specify the &#x60;type&#x60; to enable, and a &#x60;value&#x60; with a time duration expression. The request must contain a &#x60;value&#x60; with a \&quot;Time duration expression\&quot;. (See request schema for syntax.)  | 

### Return type

[**ModeLaterResponse**](ModeLaterResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


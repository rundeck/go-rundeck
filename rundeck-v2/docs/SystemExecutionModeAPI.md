# \SystemExecutionModeAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiExecutionModeLaterActive**](SystemExecutionModeAPI.md#ApiExecutionModeLaterActive) | **Post** /system/executions/enable/later | Enable System executions after a duration of time
[**ApiExecutionModeLaterPassive**](SystemExecutionModeAPI.md#ApiExecutionModeLaterPassive) | **Post** /system/executions/disable/later | Disable System executions after a duration of time



## ApiExecutionModeLaterActive

> ModeLaterResponse ApiExecutionModeLaterActive(ctx).ModeLaterRequest(modeLaterRequest).Execute()

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
	modeLaterRequest := *openapiclient.NewModeLaterRequest() // ModeLaterRequest | Enable Executions. Specify a `value` with a time duration expression. (See request schema for syntax.) 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemExecutionModeAPI.ApiExecutionModeLaterActive(context.Background()).ModeLaterRequest(modeLaterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemExecutionModeAPI.ApiExecutionModeLaterActive``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionModeLaterActive`: ModeLaterResponse
	fmt.Fprintf(os.Stdout, "Response from `SystemExecutionModeAPI.ApiExecutionModeLaterActive`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionModeLaterActiveRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **modeLaterRequest** | [**ModeLaterRequest**](ModeLaterRequest.md) | Enable Executions. Specify a &#x60;value&#x60; with a time duration expression. (See request schema for syntax.)  | 

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


## ApiExecutionModeLaterPassive

> ModeLaterResponse ApiExecutionModeLaterPassive(ctx).ModeLaterRequest(modeLaterRequest).Execute()

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
	modeLaterRequest := *openapiclient.NewModeLaterRequest() // ModeLaterRequest | Disable Executions. Specify a `value` with a time duration expression. (See request schema for syntax.) 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemExecutionModeAPI.ApiExecutionModeLaterPassive(context.Background()).ModeLaterRequest(modeLaterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemExecutionModeAPI.ApiExecutionModeLaterPassive``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionModeLaterPassive`: ModeLaterResponse
	fmt.Fprintf(os.Stdout, "Response from `SystemExecutionModeAPI.ApiExecutionModeLaterPassive`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionModeLaterPassiveRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **modeLaterRequest** | [**ModeLaterRequest**](ModeLaterRequest.md) | Disable Executions. Specify a &#x60;value&#x60; with a time duration expression. (See request schema for syntax.)  | 

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


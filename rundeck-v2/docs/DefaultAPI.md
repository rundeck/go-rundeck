# \DefaultAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiValidateOption**](DefaultAPI.md#ApiValidateOption) | **Post** /project/{project}/jobs/validateOption | Validate an option



## ApiValidateOption

> OptionValidateResponse ApiValidateOption(ctx, project).JobWasScheduled(jobWasScheduled).ApiValidateOptionRequest(apiValidateOptionRequest).Execute()

Validate an option



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
	project := "project_example" // string | Project name
	jobWasScheduled := true // bool | True if job was scheduled
	apiValidateOptionRequest := *openapiclient.NewApiValidateOptionRequest() // ApiValidateOptionRequest | Option validation request (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultAPI.ApiValidateOption(context.Background(), project).JobWasScheduled(jobWasScheduled).ApiValidateOptionRequest(apiValidateOptionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultAPI.ApiValidateOption``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiValidateOption`: OptionValidateResponse
	fmt.Fprintf(os.Stdout, "Response from `DefaultAPI.ApiValidateOption`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiValidateOptionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **jobWasScheduled** | **bool** | True if job was scheduled | 
 **apiValidateOptionRequest** | [**ApiValidateOptionRequest**](ApiValidateOptionRequest.md) | Option validation request | 

### Return type

[**OptionValidateResponse**](OptionValidateResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


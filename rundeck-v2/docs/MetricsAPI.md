# \MetricsAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiMetrics**](MetricsAPI.md#ApiMetrics) | **Get** /metrics/{name} | Get Rundeck metrics



## ApiMetrics

> LinkListResponse ApiMetrics(ctx, name).Execute()

Get Rundeck metrics



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
	name := "name_example" // string | Metric name, or blank to receive list of metrics

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MetricsAPI.ApiMetrics(context.Background(), name).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetricsAPI.ApiMetrics``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiMetrics`: LinkListResponse
	fmt.Fprintf(os.Stdout, "Response from `MetricsAPI.ApiMetrics`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** | Metric name, or blank to receive list of metrics | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiMetricsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**LinkListResponse**](LinkListResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


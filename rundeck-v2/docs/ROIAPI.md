# \ROIAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetRoiMetricsDataApi**](ROIAPI.md#GetRoiMetricsDataApi) | **Get** /execution/{id}/roimetrics/data | INCUBATING: ROI Metrics Data [Enterprise]
[**GetRoiMetricsDataAvailability**](ROIAPI.md#GetRoiMetricsDataAvailability) | **Get** /execution/{id}/roimetrics/available | INCUBATING: ROI Metrics Data Available [Enterprise]



## GetRoiMetricsDataApi

> GetRoiMetricsDataApi(ctx, id).Wait(wait).Execute()

INCUBATING: ROI Metrics Data [Enterprise]



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
	id := "id_example" // string | Execution ID
	wait := true // bool | if true and the data is not immediately available, the response will wait until the data is retrieved, or a timeout occurs. Otherwise the response may return 202 status if data must be retrieved first. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ROIAPI.GetRoiMetricsDataApi(context.Background(), id).Wait(wait).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ROIAPI.GetRoiMetricsDataApi``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRoiMetricsDataApiRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **wait** | **bool** | if true and the data is not immediately available, the response will wait until the data is retrieved, or a timeout occurs. Otherwise the response may return 202 status if data must be retrieved first. | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetRoiMetricsDataAvailability

> RoiMetricsControllerDataAvailableResponse GetRoiMetricsDataAvailability(ctx, id).Execute()

INCUBATING: ROI Metrics Data Available [Enterprise]



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
	id := "id_example" // string | Execution ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ROIAPI.GetRoiMetricsDataAvailability(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ROIAPI.GetRoiMetricsDataAvailability``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRoiMetricsDataAvailability`: RoiMetricsControllerDataAvailableResponse
	fmt.Fprintf(os.Stdout, "Response from `ROIAPI.GetRoiMetricsDataAvailability`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRoiMetricsDataAvailabilityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RoiMetricsControllerDataAvailableResponse**](RoiMetricsControllerDataAvailableResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


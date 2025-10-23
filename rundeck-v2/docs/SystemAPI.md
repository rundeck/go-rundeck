# \SystemAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiExecutionModeActive**](SystemAPI.md#ApiExecutionModeActive) | **Post** /system/executions/enable | Set Execution Mode Active
[**ApiExecutionModePassive**](SystemAPI.md#ApiExecutionModePassive) | **Post** /system/executions/disable | Set Execution Mode Passive
[**ApiExecutionModeStatus**](SystemAPI.md#ApiExecutionModeStatus) | **Get** /system/executions/status | Get Current Execution Mode
[**ApiSystemInfo**](SystemAPI.md#ApiSystemInfo) | **Get** /system/info | Get Rundeck server information and stats
[**FeatureQuery**](SystemAPI.md#FeatureQuery) | **Get** /feature/{featureName} | Get Rundeck System Feature Status
[**FeatureQueryAll**](SystemAPI.md#FeatureQueryAll) | **Get** /feature | List all System Feature on/off Status
[**GetDataset**](SystemAPI.md#GetDataset) | **Get** /enterprise/system-report/datasets/{dataset} | Get System Report Dataset by Name
[**ListDatasets**](SystemAPI.md#ListDatasets) | **Get** /enterprise/system-report/datasets | List System Report Datasets



## ApiExecutionModeActive

> ExecutionModeResult ApiExecutionModeActive(ctx).Execute()

Set Execution Mode Active



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemAPI.ApiExecutionModeActive(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemAPI.ApiExecutionModeActive``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionModeActive`: ExecutionModeResult
	fmt.Fprintf(os.Stdout, "Response from `SystemAPI.ApiExecutionModeActive`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionModeActiveRequest struct via the builder pattern


### Return type

[**ExecutionModeResult**](ExecutionModeResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionModePassive

> ExecutionModeResult ApiExecutionModePassive(ctx).Execute()

Set Execution Mode Passive



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemAPI.ApiExecutionModePassive(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemAPI.ApiExecutionModePassive``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionModePassive`: ExecutionModeResult
	fmt.Fprintf(os.Stdout, "Response from `SystemAPI.ApiExecutionModePassive`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionModePassiveRequest struct via the builder pattern


### Return type

[**ExecutionModeResult**](ExecutionModeResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionModeStatus

> ExecutionModeResult ApiExecutionModeStatus(ctx).PassiveAs503(passiveAs503).Execute()

Get Current Execution Mode



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
	passiveAs503 := true // bool | if true, return 503 response when execution mode is passive. Since: v36 (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemAPI.ApiExecutionModeStatus(context.Background()).PassiveAs503(passiveAs503).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemAPI.ApiExecutionModeStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionModeStatus`: ExecutionModeResult
	fmt.Fprintf(os.Stdout, "Response from `SystemAPI.ApiExecutionModeStatus`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionModeStatusRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passiveAs503** | **bool** | if true, return 503 response when execution mode is passive. Since: v36 | 

### Return type

[**ExecutionModeResult**](ExecutionModeResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSystemInfo

> SystemInfoModel ApiSystemInfo(ctx).Execute()

Get Rundeck server information and stats



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemAPI.ApiSystemInfo(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemAPI.ApiSystemInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSystemInfo`: SystemInfoModel
	fmt.Fprintf(os.Stdout, "Response from `SystemAPI.ApiSystemInfo`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiSystemInfoRequest struct via the builder pattern


### Return type

[**SystemInfoModel**](SystemInfoModel.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FeatureQuery

> FeatureEnabledResult FeatureQuery(ctx, featureName).Execute()

Get Rundeck System Feature Status



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
	featureName := "featureName_example" // string | Feature name without the `feature.` prefix, or blank to receive list of all system features

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemAPI.FeatureQuery(context.Background(), featureName).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemAPI.FeatureQuery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FeatureQuery`: FeatureEnabledResult
	fmt.Fprintf(os.Stdout, "Response from `SystemAPI.FeatureQuery`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**featureName** | **string** | Feature name without the &#x60;feature.&#x60; prefix, or blank to receive list of all system features | 

### Other Parameters

Other parameters are passed through a pointer to a apiFeatureQueryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**FeatureEnabledResult**](FeatureEnabledResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FeatureQueryAll

> []FeatureEnabledResult FeatureQueryAll(ctx).Execute()

List all System Feature on/off Status



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemAPI.FeatureQueryAll(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemAPI.FeatureQueryAll``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FeatureQueryAll`: []FeatureEnabledResult
	fmt.Fprintf(os.Stdout, "Response from `SystemAPI.FeatureQueryAll`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiFeatureQueryAllRequest struct via the builder pattern


### Return type

[**[]FeatureEnabledResult**](FeatureEnabledResult.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDataset

> []DataSet GetDataset(ctx, dataset).Execute()

Get System Report Dataset by Name



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
	dataset := "dataset_example" // string | Dataset Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemAPI.GetDataset(context.Background(), dataset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemAPI.GetDataset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDataset`: []DataSet
	fmt.Fprintf(os.Stdout, "Response from `SystemAPI.GetDataset`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dataset** | **string** | Dataset Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDatasetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]DataSet**](DataSet.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDatasets

> []SystemReportItem ListDatasets(ctx).Execute()

List System Report Datasets



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemAPI.ListDatasets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemAPI.ListDatasets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDatasets`: []SystemReportItem
	fmt.Fprintf(os.Stdout, "Response from `SystemAPI.ListDatasets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListDatasetsRequest struct via the builder pattern


### Return type

[**[]SystemReportItem**](SystemReportItem.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


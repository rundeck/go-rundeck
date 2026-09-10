# \MetricsAPI

All URIs are relative to *https://localhost:4440/api/59*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiMetricsHealthcheckDocs**](MetricsAPI.md#ApiMetricsHealthcheckDocs) | **Get** /metrics/healthcheck | Get healthcheck results
[**ApiMetricsListDocs**](MetricsAPI.md#ApiMetricsListDocs) | **Get** /metrics | List available metrics
[**ApiMetricsMetricsDocs**](MetricsAPI.md#ApiMetricsMetricsDocs) | **Get** /metrics/metrics | Get metrics data
[**ApiMetricsPingDocs**](MetricsAPI.md#ApiMetricsPingDocs) | **Get** /metrics/ping | Ping metrics endpoint
[**ApiMetricsThreadsDocs**](MetricsAPI.md#ApiMetricsThreadsDocs) | **Get** /metrics/threads | Get thread dump



## ApiMetricsHealthcheckDocs

> map[string]interface{} ApiMetricsHealthcheckDocs(ctx).Execute()

Get healthcheck results



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
	resp, r, err := apiClient.MetricsAPI.ApiMetricsHealthcheckDocs(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetricsAPI.ApiMetricsHealthcheckDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiMetricsHealthcheckDocs`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MetricsAPI.ApiMetricsHealthcheckDocs`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiMetricsHealthcheckDocsRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiMetricsListDocs

> LinkListResponse ApiMetricsListDocs(ctx).Execute()

List available metrics



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
	resp, r, err := apiClient.MetricsAPI.ApiMetricsListDocs(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetricsAPI.ApiMetricsListDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiMetricsListDocs`: LinkListResponse
	fmt.Fprintf(os.Stdout, "Response from `MetricsAPI.ApiMetricsListDocs`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiMetricsListDocsRequest struct via the builder pattern


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


## ApiMetricsMetricsDocs

> map[string]interface{} ApiMetricsMetricsDocs(ctx).Execute()

Get metrics data



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
	resp, r, err := apiClient.MetricsAPI.ApiMetricsMetricsDocs(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetricsAPI.ApiMetricsMetricsDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiMetricsMetricsDocs`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MetricsAPI.ApiMetricsMetricsDocs`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiMetricsMetricsDocsRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiMetricsPingDocs

> string ApiMetricsPingDocs(ctx).Execute()

Ping metrics endpoint



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
	resp, r, err := apiClient.MetricsAPI.ApiMetricsPingDocs(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetricsAPI.ApiMetricsPingDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiMetricsPingDocs`: string
	fmt.Fprintf(os.Stdout, "Response from `MetricsAPI.ApiMetricsPingDocs`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiMetricsPingDocsRequest struct via the builder pattern


### Return type

**string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiMetricsThreadsDocs

> string ApiMetricsThreadsDocs(ctx).Execute()

Get thread dump



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
	resp, r, err := apiClient.MetricsAPI.ApiMetricsThreadsDocs(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetricsAPI.ApiMetricsThreadsDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiMetricsThreadsDocs`: string
	fmt.Fprintf(os.Stdout, "Response from `MetricsAPI.ApiMetricsThreadsDocs`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiMetricsThreadsDocsRequest struct via the builder pattern


### Return type

**string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


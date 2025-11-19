# \HealthAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiNodeHealth**](HealthAPI.md#ApiNodeHealth) | **Get** /project/{project}/healthcheck/status | Get Node Healthcheck Status [Enterprise]
[**ApiNodeHealthAll**](HealthAPI.md#ApiNodeHealthAll) | **Get** /project/{project}/healthcheck/status/all | Get Node Healthcheck Status for All Nodes [Enterprise]
[**ApiProjectHasHealthStatusEnhancer**](HealthAPI.md#ApiProjectHasHealthStatusEnhancer) | **Get** /project/{project}/healthcheck/enhancer | Check Health Status Node Enhancer is Configured [Enterprise]
[**ApiRefreshHealthCheck**](HealthAPI.md#ApiRefreshHealthCheck) | **Post** /project/{project}/healthcheck/refresh | Refresh Node Healthcheck Status [Enterprise]
[**ApiRefreshHealthCheckAll**](HealthAPI.md#ApiRefreshHealthCheckAll) | **Post** /project/{project}/healthcheck/refresh/all | Refresh All Project Node Healthchecks [Enterprise]



## ApiNodeHealth

> map[string]interface{} ApiNodeHealth(ctx, project).Node(node).Execute()

Get Node Healthcheck Status [Enterprise]



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
	node := "node_example" // string | Node Name
	project := "project_example" // string | Project Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.HealthAPI.ApiNodeHealth(context.Background(), project).Node(node).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HealthAPI.ApiNodeHealth``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiNodeHealth`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `HealthAPI.ApiNodeHealth`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiNodeHealthRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **node** | **string** | Node Name | 


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


## ApiNodeHealthAll

> []map[string]interface{} ApiNodeHealthAll(ctx, project).IncludeChecks(includeChecks).Execute()

Get Node Healthcheck Status for All Nodes [Enterprise]



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
	includeChecks := true // bool | Include Checks (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.HealthAPI.ApiNodeHealthAll(context.Background(), project).IncludeChecks(includeChecks).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HealthAPI.ApiNodeHealthAll``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiNodeHealthAll`: []map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `HealthAPI.ApiNodeHealthAll`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiNodeHealthAllRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **includeChecks** | **bool** | Include Checks | 

### Return type

**[]map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectHasHealthStatusEnhancer

> map[string]interface{} ApiProjectHasHealthStatusEnhancer(ctx, project).Execute()

Check Health Status Node Enhancer is Configured [Enterprise]



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
	resp, r, err := apiClient.HealthAPI.ApiProjectHasHealthStatusEnhancer(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HealthAPI.ApiProjectHasHealthStatusEnhancer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectHasHealthStatusEnhancer`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `HealthAPI.ApiProjectHasHealthStatusEnhancer`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectHasHealthStatusEnhancerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


## ApiRefreshHealthCheck

> map[string]interface{} ApiRefreshHealthCheck(ctx, project).Node(node).Body(body).Execute()

Refresh Node Healthcheck Status [Enterprise]



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
	node := "node_example" // string | Node Name (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} | Node List Request (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.HealthAPI.ApiRefreshHealthCheck(context.Background(), project).Node(node).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HealthAPI.ApiRefreshHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiRefreshHealthCheck`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `HealthAPI.ApiRefreshHealthCheck`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiRefreshHealthCheckRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **node** | **string** | Node Name | 
 **body** | **map[string]interface{}** | Node List Request | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiRefreshHealthCheckAll

> map[string]interface{} ApiRefreshHealthCheckAll(ctx, project).Execute()

Refresh All Project Node Healthchecks [Enterprise]



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
	resp, r, err := apiClient.HealthAPI.ApiRefreshHealthCheckAll(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HealthAPI.ApiRefreshHealthCheckAll``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiRefreshHealthCheckAll`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `HealthAPI.ApiRefreshHealthCheckAll`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiRefreshHealthCheckAllRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


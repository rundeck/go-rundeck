# \ClusterAPI

All URIs are relative to *https://localhost:4440/api/59*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiJobClusterTakeoverSchedule**](ClusterAPI.md#ApiJobClusterTakeoverSchedule) | **Put** /scheduler/takeover | Takeover Schedule in Cluster Mode
[**ApiToggle**](ClusterAPI.md#ApiToggle) | **Post** /enterprise/cluster/executions/disable | Set Execution Mode for a Cluster Member [Enterprise]
[**ApiToggle1**](ClusterAPI.md#ApiToggle1) | **Post** /enterprise/cluster/executions/enable | Set Execution Mode for a Cluster Member [Enterprise]



## ApiJobClusterTakeoverSchedule

> map[string]interface{} ApiJobClusterTakeoverSchedule(ctx).Body(body).Execute()

Takeover Schedule in Cluster Mode



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
	body := map[string]interface{}{ ... } // map[string]interface{} | Takeover Request.  * optional `server` entry, with one of these required entries:     * `uuid` server UUID to take over from     * `all` value of `true` to take over from all servers * optional `project` entry, specifying a project name * optional `job` entry, with required entry:     * `id` Job UUID * optional `jobs` array, each object has:     * `id` Job UUID     * (Since: v32) 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ClusterAPI.ApiJobClusterTakeoverSchedule(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ClusterAPI.ApiJobClusterTakeoverSchedule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobClusterTakeoverSchedule`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ClusterAPI.ApiJobClusterTakeoverSchedule`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiJobClusterTakeoverScheduleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **map[string]interface{}** | Takeover Request.  * optional &#x60;server&#x60; entry, with one of these required entries:     * &#x60;uuid&#x60; server UUID to take over from     * &#x60;all&#x60; value of &#x60;true&#x60; to take over from all servers * optional &#x60;project&#x60; entry, specifying a project name * optional &#x60;job&#x60; entry, with required entry:     * &#x60;id&#x60; Job UUID * optional &#x60;jobs&#x60; array, each object has:     * &#x60;id&#x60; Job UUID     * (Since: v32)  | 

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


## ApiToggle

> map[string]interface{} ApiToggle(ctx).Uuid(uuid).Execute()

Set Execution Mode for a Cluster Member [Enterprise]



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
	uuid := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | UUID of Member

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ClusterAPI.ApiToggle(context.Background()).Uuid(uuid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ClusterAPI.ApiToggle``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiToggle`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ClusterAPI.ApiToggle`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiToggleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **string** | UUID of Member | 

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


## ApiToggle1

> map[string]interface{} ApiToggle1(ctx).Uuid(uuid).Execute()

Set Execution Mode for a Cluster Member [Enterprise]



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
	uuid := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | UUID of Member

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ClusterAPI.ApiToggle1(context.Background()).Uuid(uuid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ClusterAPI.ApiToggle1``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiToggle1`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ClusterAPI.ApiToggle1`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiToggle1Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **string** | UUID of Member | 

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


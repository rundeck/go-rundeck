# \SchedulerAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiJobClusterTakeoverSchedule**](SchedulerAPI.md#ApiJobClusterTakeoverSchedule) | **Put** /scheduler/takeover | Takeover Schedule in Cluster Mode



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
	resp, r, err := apiClient.SchedulerAPI.ApiJobClusterTakeoverSchedule(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SchedulerAPI.ApiJobClusterTakeoverSchedule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobClusterTakeoverSchedule`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `SchedulerAPI.ApiJobClusterTakeoverSchedule`: %v\n", resp)
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

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


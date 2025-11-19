# \LogStorageAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiLogstorageInfo**](LogStorageAPI.md#ApiLogstorageInfo) | **Get** /system/logstorage | Log Storage Info
[**ApiLogstorageListIncompleteExecutions**](LogStorageAPI.md#ApiLogstorageListIncompleteExecutions) | **Get** /system/logstorage/incomplete | List Executions with Incomplete Log Storage
[**ApiResumeIncompleteLogstorage**](LogStorageAPI.md#ApiResumeIncompleteLogstorage) | **Post** /system/logstorage/incomplete/resume | Resume Incomplete Log Storage



## ApiLogstorageInfo

> map[string]interface{} ApiLogstorageInfo(ctx).Execute()

Log Storage Info



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
	resp, r, err := apiClient.LogStorageAPI.ApiLogstorageInfo(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LogStorageAPI.ApiLogstorageInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiLogstorageInfo`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `LogStorageAPI.ApiLogstorageInfo`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiLogstorageInfoRequest struct via the builder pattern


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


## ApiLogstorageListIncompleteExecutions

> map[string]interface{} ApiLogstorageListIncompleteExecutions(ctx).Query(query).Execute()

List Executions with Incomplete Log Storage



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
	query := *openapiclient.NewBaseQuery() // BaseQuery |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LogStorageAPI.ApiLogstorageListIncompleteExecutions(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LogStorageAPI.ApiLogstorageListIncompleteExecutions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiLogstorageListIncompleteExecutions`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `LogStorageAPI.ApiLogstorageListIncompleteExecutions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiLogstorageListIncompleteExecutionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | [**BaseQuery**](BaseQuery.md) |  | 

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


## ApiResumeIncompleteLogstorage

> map[string]interface{} ApiResumeIncompleteLogstorage(ctx).Execute()

Resume Incomplete Log Storage



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
	resp, r, err := apiClient.LogStorageAPI.ApiResumeIncompleteLogstorage(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LogStorageAPI.ApiResumeIncompleteLogstorage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiResumeIncompleteLogstorage`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `LogStorageAPI.ApiResumeIncompleteLogstorage`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiResumeIncompleteLogstorageRequest struct via the builder pattern


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


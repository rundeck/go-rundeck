# \JobsAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiExecutionDataAvailable**](JobsAPI.md#ApiExecutionDataAvailable) | **Get** /execution/{id}/result/dataAvailable | Check Execution Result Data Availability [Enterprise]
[**ApiExecutionDataExport**](JobsAPI.md#ApiExecutionDataExport) | **Get** /execution/{id}/result/data | Get Execution Result Data [Enterprise]
[**ApiFlipExecutionDisabled**](JobsAPI.md#ApiFlipExecutionDisabled) | **Post** /job/{id}/execution/disable | Disable Executions for a Job
[**ApiFlipExecutionDisabledBulk**](JobsAPI.md#ApiFlipExecutionDisabledBulk) | **Post** /jobs/execution/disable | Bulk Toggle Job Execution Disabled
[**ApiFlipExecutionEnabled**](JobsAPI.md#ApiFlipExecutionEnabled) | **Post** /job/{id}/execution/enable | Enable Executions for a Job
[**ApiFlipExecutionEnabledBulk**](JobsAPI.md#ApiFlipExecutionEnabledBulk) | **Post** /jobs/execution/enable | Bulk Toggle Job Execution Enabled
[**ApiFlipScheduleDisabled**](JobsAPI.md#ApiFlipScheduleDisabled) | **Post** /job/{id}/schedule/disable | Disable Schedule for a Job
[**ApiFlipScheduleDisabledBulk**](JobsAPI.md#ApiFlipScheduleDisabledBulk) | **Post** /jobs/schedule/disable | Bulk Toggle Job Schedule Disabled
[**ApiFlipScheduleEnabled**](JobsAPI.md#ApiFlipScheduleEnabled) | **Post** /job/{id}/schedule/enable | Enable Schedule for a Job
[**ApiFlipScheduleEnabledBulk**](JobsAPI.md#ApiFlipScheduleEnabledBulk) | **Post** /jobs/schedule/enable | Bulk Toggle Job Schedule Enabled
[**ApiJobBrowse**](JobsAPI.md#ApiJobBrowse) | **Post** /project/{project}/jobs/browse | Project Job Group browse
[**ApiJobBrowseGetDocs**](JobsAPI.md#ApiJobBrowseGetDocs) | **Get** /project/{project}/jobs/browse | Browse jobs at a path
[**ApiJobDelete**](JobsAPI.md#ApiJobDelete) | **Delete** /job/{id} | Deleting a Job Definition
[**ApiJobDeleteBulk**](JobsAPI.md#ApiJobDeleteBulk) | **Post** /jobs/delete | Bulk Job Delete
[**ApiJobDeleteBulkDocs2**](JobsAPI.md#ApiJobDeleteBulkDocs2) | **Delete** /jobs/delete | Bulk Job Delete
[**ApiJobDetail**](JobsAPI.md#ApiJobDetail) | **Get** /job/{id}/info | Get Job Metadata
[**ApiJobExecutions**](JobsAPI.md#ApiJobExecutions) | **Get** /job/{id}/executions | Getting Executions for a Job
[**ApiJobExecutionsDelete**](JobsAPI.md#ApiJobExecutionsDelete) | **Delete** /job/{id}/executions | Delete all Executions for a Job
[**ApiJobExport**](JobsAPI.md#ApiJobExport) | **Get** /job/{id} | Getting a Job Definition
[**ApiJobFileInfo**](JobsAPI.md#ApiJobFileInfo) | **Get** /jobs/file/{id} | Get Info About an Uploaded File
[**ApiJobFileMultiUpload**](JobsAPI.md#ApiJobFileMultiUpload) | **Post** /job/{id}/input/file | Upload Multiple Files for Job Options
[**ApiJobFileUpload**](JobsAPI.md#ApiJobFileUpload) | **Post** /job/{id}/input/file/{optionName} | Upload a File for a Job Option
[**ApiJobForecast**](JobsAPI.md#ApiJobForecast) | **Get** /job/{id}/forecast | Get Job Forecast
[**ApiJobMeta**](JobsAPI.md#ApiJobMeta) | **Get** /job/{id}/meta | Get Job UI Metadata
[**ApiJobRetry**](JobsAPI.md#ApiJobRetry) | **Post** /job/{id}/retry/{executionId} | Retry a Job based on execution
[**ApiJobRun**](JobsAPI.md#ApiJobRun) | **Post** /job/{id}/executions | Running a Job
[**ApiJobRun1**](JobsAPI.md#ApiJobRun1) | **Post** /job/{id}/run | Running a Job
[**ApiJobWorkflow**](JobsAPI.md#ApiJobWorkflow) | **Get** /job/{id}/workflow | Get Job Workflow
[**ApiJobsExportv14**](JobsAPI.md#ApiJobsExportv14) | **Get** /project/{project}/jobs/export | Export Jobs
[**ApiJobsImportv14**](JobsAPI.md#ApiJobsImportv14) | **Post** /project/{project}/jobs/import | Import Job definitions
[**ApiJobsImportv14_0**](JobsAPI.md#ApiJobsImportv14_0) | **Post** /project/{project}/jobs/import | Import Job definitions
[**ApiJobsListv2**](JobsAPI.md#ApiJobsListv2) | **Get** /project/{project}/jobs | Listing Jobs
[**ApiListAllJobsInProject**](JobsAPI.md#ApiListAllJobsInProject) | **Get** /project/{project}/listAllJobs | List all Jobs in Summarized Form [Enterprise]
[**ApiSchedulerListJobs**](JobsAPI.md#ApiSchedulerListJobs) | **Get** /scheduler/server/{uuid}/jobs | List Scheduled Jobs For a Cluster Server
[**ApiSchedulerListJobsCurrentDocs**](JobsAPI.md#ApiSchedulerListJobsCurrentDocs) | **Get** /scheduler/jobs | List Scheduled Jobs For this Cluster Server



## ApiExecutionDataAvailable

> ResultDataAvailableResponse ApiExecutionDataAvailable(ctx, id).Execute()

Check Execution Result Data Availability [Enterprise]



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
	id := "id_example" // string | Execution ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiExecutionDataAvailable(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiExecutionDataAvailable``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionDataAvailable`: ResultDataAvailableResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiExecutionDataAvailable`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionDataAvailableRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ResultDataAvailableResponse**](ResultDataAvailableResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionDataExport

> ApiExecutionDataExport(ctx, id).Wait(wait).Execute()

Get Execution Result Data [Enterprise]



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
	id := "id_example" // string | Execution ID
	wait := true // bool | if true and the data is not immediately available, the response will wait until the data is retrieved, or a timeout occurs. Otherwise the response may return 202 status if data must be retrieved first. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.JobsAPI.ApiExecutionDataExport(context.Background(), id).Wait(wait).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiExecutionDataExport``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiExecutionDataExportRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **wait** | **bool** | if true and the data is not immediately available, the response will wait until the data is retrieved, or a timeout occurs. Otherwise the response may return 202 status if data must be retrieved first. | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiFlipExecutionDisabled

> map[string]interface{} ApiFlipExecutionDisabled(ctx, id).Execute()

Disable Executions for a Job



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
	id := "id_example" // string | Job ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiFlipExecutionDisabled(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiFlipExecutionDisabled``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiFlipExecutionDisabled`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiFlipExecutionDisabled`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiFlipExecutionDisabledRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiFlipExecutionDisabledBulk

> map[string]interface{} ApiFlipExecutionDisabledBulk(ctx).Ids(ids).Idlist(idlist).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()

Bulk Toggle Job Execution Disabled



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
	ids := []string{"Inner_example"} // []string | The Job IDs to delete, can be specified multiple times (optional)
	idlist := "idlist_example" // string | The Job IDs to delete as a single comma-separated string. (optional)
	apiBulkJobDeleteRequest := *openapiclient.NewApiBulkJobDeleteRequest() // ApiBulkJobDeleteRequest | request (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiFlipExecutionDisabledBulk(context.Background()).Ids(ids).Idlist(idlist).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiFlipExecutionDisabledBulk``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiFlipExecutionDisabledBulk`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiFlipExecutionDisabledBulk`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiFlipExecutionDisabledBulkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **[]string** | The Job IDs to delete, can be specified multiple times | 
 **idlist** | **string** | The Job IDs to delete as a single comma-separated string. | 
 **apiBulkJobDeleteRequest** | [**ApiBulkJobDeleteRequest**](ApiBulkJobDeleteRequest.md) | request | 

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


## ApiFlipExecutionEnabled

> map[string]interface{} ApiFlipExecutionEnabled(ctx, id).Execute()

Enable Executions for a Job



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
	id := "id_example" // string | Job ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiFlipExecutionEnabled(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiFlipExecutionEnabled``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiFlipExecutionEnabled`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiFlipExecutionEnabled`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiFlipExecutionEnabledRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiFlipExecutionEnabledBulk

> map[string]interface{} ApiFlipExecutionEnabledBulk(ctx).Ids(ids).Idlist(idlist).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()

Bulk Toggle Job Execution Enabled



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
	ids := []string{"Inner_example"} // []string | The Job IDs to delete, can be specified multiple times (optional)
	idlist := "idlist_example" // string | The Job IDs to delete as a single comma-separated string. (optional)
	apiBulkJobDeleteRequest := *openapiclient.NewApiBulkJobDeleteRequest() // ApiBulkJobDeleteRequest | Bulk ID request (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiFlipExecutionEnabledBulk(context.Background()).Ids(ids).Idlist(idlist).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiFlipExecutionEnabledBulk``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiFlipExecutionEnabledBulk`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiFlipExecutionEnabledBulk`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiFlipExecutionEnabledBulkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **[]string** | The Job IDs to delete, can be specified multiple times | 
 **idlist** | **string** | The Job IDs to delete as a single comma-separated string. | 
 **apiBulkJobDeleteRequest** | [**ApiBulkJobDeleteRequest**](ApiBulkJobDeleteRequest.md) | Bulk ID request | 

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


## ApiFlipScheduleDisabled

> map[string]interface{} ApiFlipScheduleDisabled(ctx, id).Execute()

Disable Schedule for a Job



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
	id := "id_example" // string | Job ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiFlipScheduleDisabled(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiFlipScheduleDisabled``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiFlipScheduleDisabled`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiFlipScheduleDisabled`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiFlipScheduleDisabledRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiFlipScheduleDisabledBulk

> map[string]interface{} ApiFlipScheduleDisabledBulk(ctx).Ids(ids).Idlist(idlist).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()

Bulk Toggle Job Schedule Disabled



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
	ids := []string{"Inner_example"} // []string | The Job IDs to delete, can be specified multiple times (optional)
	idlist := "idlist_example" // string | The Job IDs to delete as a single comma-separated string. (optional)
	apiBulkJobDeleteRequest := *openapiclient.NewApiBulkJobDeleteRequest() // ApiBulkJobDeleteRequest | Bulk ID request (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiFlipScheduleDisabledBulk(context.Background()).Ids(ids).Idlist(idlist).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiFlipScheduleDisabledBulk``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiFlipScheduleDisabledBulk`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiFlipScheduleDisabledBulk`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiFlipScheduleDisabledBulkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **[]string** | The Job IDs to delete, can be specified multiple times | 
 **idlist** | **string** | The Job IDs to delete as a single comma-separated string. | 
 **apiBulkJobDeleteRequest** | [**ApiBulkJobDeleteRequest**](ApiBulkJobDeleteRequest.md) | Bulk ID request | 

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


## ApiFlipScheduleEnabled

> map[string]interface{} ApiFlipScheduleEnabled(ctx, id).Execute()

Enable Schedule for a Job



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
	id := "id_example" // string | Job ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiFlipScheduleEnabled(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiFlipScheduleEnabled``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiFlipScheduleEnabled`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiFlipScheduleEnabled`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiFlipScheduleEnabledRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiFlipScheduleEnabledBulk

> map[string]interface{} ApiFlipScheduleEnabledBulk(ctx).Ids(ids).Idlist(idlist).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()

Bulk Toggle Job Schedule Enabled



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
	ids := []string{"Inner_example"} // []string | The Job IDs to delete, can be specified multiple times (optional)
	idlist := "idlist_example" // string | The Job IDs to delete as a single comma-separated string. (optional)
	apiBulkJobDeleteRequest := *openapiclient.NewApiBulkJobDeleteRequest() // ApiBulkJobDeleteRequest | Bulk ID request (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiFlipScheduleEnabledBulk(context.Background()).Ids(ids).Idlist(idlist).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiFlipScheduleEnabledBulk``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiFlipScheduleEnabledBulk`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiFlipScheduleEnabledBulk`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiFlipScheduleEnabledBulkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **[]string** | The Job IDs to delete, can be specified multiple times | 
 **idlist** | **string** | The Job IDs to delete as a single comma-separated string. | 
 **apiBulkJobDeleteRequest** | [**ApiBulkJobDeleteRequest**](ApiBulkJobDeleteRequest.md) | Bulk ID request | 

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


## ApiJobBrowse

> JobBrowseResponse ApiJobBrowse(ctx, project).Path(path).Meta(meta).Breakpoint(breakpoint).Max(max).RdJobQueryInput(rdJobQueryInput).Execute()

Project Job Group browse



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
	project := "project_example" // string | Project name
	path := "path_example" // string | Group path root, or blank for the root
	meta := "meta_example" // string | Comma-separated list of metadata items to include, or \"*\" for all
	breakpoint := int32(56) // int32 | Breakpoint, max number of jobs to load with metadata, if more results than the  breakpoint are available, no metadata will be loaded
	max := int32(56) // int32 | Since v54: Maximum number of jobs to retrieve. If not specified, all jobs will be returned.
	rdJobQueryInput := *openapiclient.NewRdJobQueryInput() // RdJobQueryInput | Query parameters (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobBrowse(context.Background(), project).Path(path).Meta(meta).Breakpoint(breakpoint).Max(max).RdJobQueryInput(rdJobQueryInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobBrowse``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobBrowse`: JobBrowseResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobBrowse`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobBrowseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **path** | **string** | Group path root, or blank for the root | 
 **meta** | **string** | Comma-separated list of metadata items to include, or \&quot;*\&quot; for all | 
 **breakpoint** | **int32** | Breakpoint, max number of jobs to load with metadata, if more results than the  breakpoint are available, no metadata will be loaded | 
 **max** | **int32** | Since v54: Maximum number of jobs to retrieve. If not specified, all jobs will be returned. | 
 **rdJobQueryInput** | [**RdJobQueryInput**](RdJobQueryInput.md) | Query parameters | 

### Return type

[**JobBrowseResponse**](JobBrowseResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobBrowseGetDocs

> JobBrowseResponse ApiJobBrowseGetDocs(ctx, project).Path(path).Meta(meta).Breakpoint(breakpoint).Execute()

Browse jobs at a path



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
	project := "project_example" // string | Project name
	path := "path_example" // string | Group path root, or blank for the root
	meta := "meta_example" // string | Comma-separated list of metadata items to include, or \"*\" for all
	breakpoint := int32(56) // int32 | Breakpoint, max number of jobs to load with metadata, if more results than the  breakpoint are available, no metadata will be loaded

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobBrowseGetDocs(context.Background(), project).Path(path).Meta(meta).Breakpoint(breakpoint).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobBrowseGetDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobBrowseGetDocs`: JobBrowseResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobBrowseGetDocs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobBrowseGetDocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **path** | **string** | Group path root, or blank for the root | 
 **meta** | **string** | Comma-separated list of metadata items to include, or \&quot;*\&quot; for all | 
 **breakpoint** | **int32** | Breakpoint, max number of jobs to load with metadata, if more results than the  breakpoint are available, no metadata will be loaded | 

### Return type

[**JobBrowseResponse**](JobBrowseResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobDelete

> map[string]interface{} ApiJobDelete(ctx, id).Execute()

Deleting a Job Definition



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
	id := "id_example" // string | Job ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobDelete(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobDelete`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobDeleteBulk

> DeleteBulkResponse ApiJobDeleteBulk(ctx).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()

Bulk Job Delete



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
	apiBulkJobDeleteRequest := *openapiclient.NewApiBulkJobDeleteRequest() // ApiBulkJobDeleteRequest | Bulk ID request (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobDeleteBulk(context.Background()).ApiBulkJobDeleteRequest(apiBulkJobDeleteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobDeleteBulk``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobDeleteBulk`: DeleteBulkResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobDeleteBulk`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiJobDeleteBulkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiBulkJobDeleteRequest** | [**ApiBulkJobDeleteRequest**](ApiBulkJobDeleteRequest.md) | Bulk ID request | 

### Return type

[**DeleteBulkResponse**](DeleteBulkResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobDeleteBulkDocs2

> DeleteBulkResponse ApiJobDeleteBulkDocs2(ctx).Ids(ids).Idlist(idlist).Execute()

Bulk Job Delete



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
	ids := []string{"Inner_example"} // []string | The Job IDs to delete, can be specified multiple times (optional)
	idlist := "idlist_example" // string | The Job IDs to delete as a single comma-separated string. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobDeleteBulkDocs2(context.Background()).Ids(ids).Idlist(idlist).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobDeleteBulkDocs2``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobDeleteBulkDocs2`: DeleteBulkResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobDeleteBulkDocs2`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiJobDeleteBulkDocs2Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **[]string** | The Job IDs to delete, can be specified multiple times | 
 **idlist** | **string** | The Job IDs to delete as a single comma-separated string. | 

### Return type

[**DeleteBulkResponse**](DeleteBulkResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobDetail

> JobInfo ApiJobDetail(ctx, id).Execute()

Get Job Metadata



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
	id := "id_example" // string | Job ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobDetail(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobDetail`: JobInfo
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**JobInfo**](JobInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobExecutions

> []map[string]interface{} ApiJobExecutions(ctx, id).Status(status).Max(max).Offset(offset).IncludeJobRef(includeJobRef).Execute()

Getting Executions for a Job



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
	id := "id_example" // string | Job ID
	status := "status_example" // string | the status of executions you want to be returned.  Must be  one of \"succeeded\", \"failed\", \"aborted\", or \"running\".  If this parameter is blank or unset, include all executions. (optional)
	max := int32(56) // int32 | indicate the maximum number of results to return. If  unspecified, all results will be returned (optional)
	offset := int32(56) // int32 | indicate the 0-indexed offset for the first result to  return. (optional)
	includeJobRef := true // bool | if true, include executions from the job reference in the results. Default is false.  Requires API version 50 or later. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobExecutions(context.Background(), id).Status(status).Max(max).Offset(offset).IncludeJobRef(includeJobRef).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobExecutions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobExecutions`: []map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobExecutions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobExecutionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **status** | **string** | the status of executions you want to be returned.  Must be  one of \&quot;succeeded\&quot;, \&quot;failed\&quot;, \&quot;aborted\&quot;, or \&quot;running\&quot;.  If this parameter is blank or unset, include all executions. | 
 **max** | **int32** | indicate the maximum number of results to return. If  unspecified, all results will be returned | 
 **offset** | **int32** | indicate the 0-indexed offset for the first result to  return. | 
 **includeJobRef** | **bool** | if true, include executions from the job reference in the results. Default is false.  Requires API version 50 or later. | 

### Return type

**[]map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobExecutionsDelete

> DeleteBulkResponse ApiJobExecutionsDelete(ctx, id).Execute()

Delete all Executions for a Job



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
	id := "id_example" // string | Job ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobExecutionsDelete(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobExecutionsDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobExecutionsDelete`: DeleteBulkResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobExecutionsDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobExecutionsDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DeleteBulkResponse**](DeleteBulkResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobExport

> map[string]interface{} ApiJobExport(ctx, id).Format(format).Execute()

Getting a Job Definition



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
	id := "id_example" // string | Job ID
	format := "format_example" // string | can be \"yaml\" or \"json\" (API v44+) to specify the output format (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobExport(context.Background(), id).Format(format).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobExport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobExport`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobExport`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobExportRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **format** | **string** | can be \&quot;yaml\&quot; or \&quot;json\&quot; (API v44+) to specify the output format | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/yaml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobFileInfo

> JobFileInfo ApiJobFileInfo(ctx, id).Execute()

Get Info About an Uploaded File



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
	id := "id_example" // string | File ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobFileInfo(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobFileInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobFileInfo`: JobFileInfo
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobFileInfo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | File ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobFileInfoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**JobFileInfo**](JobFileInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobFileMultiUpload

> JobFileUpload ApiJobFileMultiUpload(ctx, id).Execute()

Upload Multiple Files for Job Options



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
	id := "id_example" // string | Job ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobFileMultiUpload(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobFileMultiUpload``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobFileMultiUpload`: JobFileUpload
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobFileMultiUpload`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobFileMultiUploadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**JobFileUpload**](JobFileUpload.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobFileUpload

> JobFileUpload ApiJobFileUpload(ctx, id, optionName).FileName(fileName).Execute()

Upload a File for a Job Option



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
	id := "id_example" // string | Job ID
	optionName := "optionName_example" // string | For a single file/option value, specify the option name either as a query parameter or as part of the URL path
	fileName := "fileName_example" // string | Specify the original file name (optional) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobFileUpload(context.Background(), id, optionName).FileName(fileName).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobFileUpload``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobFileUpload`: JobFileUpload
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobFileUpload`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 
**optionName** | **string** | For a single file/option value, specify the option name either as a query parameter or as part of the URL path | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobFileUploadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fileName** | **string** | Specify the original file name (optional) | 

### Return type

[**JobFileUpload**](JobFileUpload.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/octet-stream
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobForecast

> JobInfo ApiJobForecast(ctx, id).Time(time).Past(past).Max(max).Execute()

Get Job Forecast



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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Job ID
	time := "time_example" // string | Time range to forecast.   Format is a string like `2d1h4n5s` using the following characters for time units: * `s` second * `n` minute * `h` hour * `d` day * `w` week * `m` month * `y` year  (optional)
	past := true // bool | Whether to return results in the past. default: false (optional)
	max := int32(56) // int32 | Maximum number of results to return (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobForecast(context.Background(), id).Time(time).Past(past).Max(max).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobForecast``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobForecast`: JobInfo
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobForecast`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobForecastRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **time** | **string** | Time range to forecast.   Format is a string like &#x60;2d1h4n5s&#x60; using the following characters for time units: * &#x60;s&#x60; second * &#x60;n&#x60; minute * &#x60;h&#x60; hour * &#x60;d&#x60; day * &#x60;w&#x60; week * &#x60;m&#x60; month * &#x60;y&#x60; year  | 
 **past** | **bool** | Whether to return results in the past. default: false | 
 **max** | **int32** | Maximum number of results to return | 

### Return type

[**JobInfo**](JobInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobMeta

> []ItemMeta ApiJobMeta(ctx, id).Meta(meta).Execute()

Get Job UI Metadata



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
	id := "id_example" // string | Job ID
	meta := "meta_example" // string | Comma-separated list of metadata item names to include, or \"*\" for all (default)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobMeta(context.Background(), id).Meta(meta).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobMeta``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobMeta`: []ItemMeta
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobMeta`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobMetaRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **meta** | **string** | Comma-separated list of metadata item names to include, or \&quot;*\&quot; for all (default) | 

### Return type

[**[]ItemMeta**](ItemMeta.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobRetry

> ApiJobRetry(ctx, id, executionId).FailedNodes(failedNodes).ArgString(argString).Loglevel(loglevel).AsUser(asUser).Filter(filter).RunAtTime(runAtTime).OptionOPTNAME(optionOPTNAME).MetaKEY(metaKEY).Body(body).Execute()

Retry a Job based on execution



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	id := "id_example" // string | Job ID
	executionId := "executionId_example" // string | Execution ID
	failedNodes := true // bool | `false` to run on the same nodes as the original execution, `true`or empty to run only on failed nodes. (optional)
	argString := "argString_example" // string | argument string to pass to the job, of the form: `-opt value -opt2 value ...`. (optional)
	loglevel := "loglevel_example" // string | argument specifying the loglevel to use (optional)
	asUser := "asUser_example" // string | specifies a username identifying the user who ran the job. Requires `runAs` permission. (optional)
	filter := "filter_example" // string | can be a node filter string. (optional)
	runAtTime := time.Now() // time.Time | Specify a time to run the job (Since: v18).  This is a ISO-8601 date and time stamp with timezone, with optional milliseconds., e.g. `2016-11-23T12:20:55-0800` or `2016-11-23T12:20:55.123-0800` (optional)
	optionOPTNAME := "optionOPTNAME_example" // string | Option value for option named `OPTNAME`. If any `option.OPTNAME` parameters are specified, the `argString` value is ignored (Since: v18). (optional)
	metaKEY := "metaKEY_example" // string | Additional metadata keyd by `KEY`. (Since: v32). (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} | Parameters can be specified in the request body, instead of as query parameters.  (**API v18** or later): The `options` entry can contain a map of option name -> value, in which case the `argString` is ignored. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.JobsAPI.ApiJobRetry(context.Background(), id, executionId).FailedNodes(failedNodes).ArgString(argString).Loglevel(loglevel).AsUser(asUser).Filter(filter).RunAtTime(runAtTime).OptionOPTNAME(optionOPTNAME).MetaKEY(metaKEY).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobRetry``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 
**executionId** | **string** | Execution ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobRetryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **failedNodes** | **bool** | &#x60;false&#x60; to run on the same nodes as the original execution, &#x60;true&#x60;or empty to run only on failed nodes. | 
 **argString** | **string** | argument string to pass to the job, of the form: &#x60;-opt value -opt2 value ...&#x60;. | 
 **loglevel** | **string** | argument specifying the loglevel to use | 
 **asUser** | **string** | specifies a username identifying the user who ran the job. Requires &#x60;runAs&#x60; permission. | 
 **filter** | **string** | can be a node filter string. | 
 **runAtTime** | **time.Time** | Specify a time to run the job (Since: v18).  This is a ISO-8601 date and time stamp with timezone, with optional milliseconds., e.g. &#x60;2016-11-23T12:20:55-0800&#x60; or &#x60;2016-11-23T12:20:55.123-0800&#x60; | 
 **optionOPTNAME** | **string** | Option value for option named &#x60;OPTNAME&#x60;. If any &#x60;option.OPTNAME&#x60; parameters are specified, the &#x60;argString&#x60; value is ignored (Since: v18). | 
 **metaKEY** | **string** | Additional metadata keyd by &#x60;KEY&#x60;. (Since: v32). | 
 **body** | **map[string]interface{}** | Parameters can be specified in the request body, instead of as query parameters.  (**API v18** or later): The &#x60;options&#x60; entry can contain a map of option name -&gt; value, in which case the &#x60;argString&#x60; is ignored. | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobRun

> ApiJobRun(ctx, id).ArgString(argString).Loglevel(loglevel).AsUser(asUser).Filter(filter).RunAtTime(runAtTime).OptionOPTNAME(optionOPTNAME).MetaKEY(metaKEY).Body(body).Execute()

Running a Job



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	id := "id_example" // string | Job ID
	argString := "argString_example" // string | argument string to pass to the job, of the form: `-opt value -opt2 value ...`. (optional)
	loglevel := "loglevel_example" // string | argument specifying the loglevel to use (optional)
	asUser := "asUser_example" // string | specifies a username identifying the user who ran the job. Requires `runAs` permission. (optional)
	filter := "filter_example" // string | can be a node filter string. (optional)
	runAtTime := time.Now() // time.Time | Specify a time to run the job (Since: v18).  This is a ISO-8601 date and time stamp with timezone, with optional milliseconds., e.g. `2016-11-23T12:20:55-0800` or `2016-11-23T12:20:55.123-0800` (optional)
	optionOPTNAME := "optionOPTNAME_example" // string | Option value for option named `OPTNAME`. If any `option.OPTNAME` parameters are specified, the `argString` value is ignored (Since: v18). (optional)
	metaKEY := "metaKEY_example" // string | Additional metadata keyd by `KEY`. (Since: v32). (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} | Parameters can be specified in the request body, instead of as query parameters.  (**API v18** or later): The `options` entry can contain a map of option name -> value, in which case the `argString` is ignored. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.JobsAPI.ApiJobRun(context.Background(), id).ArgString(argString).Loglevel(loglevel).AsUser(asUser).Filter(filter).RunAtTime(runAtTime).OptionOPTNAME(optionOPTNAME).MetaKEY(metaKEY).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobRun``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobRunRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **argString** | **string** | argument string to pass to the job, of the form: &#x60;-opt value -opt2 value ...&#x60;. | 
 **loglevel** | **string** | argument specifying the loglevel to use | 
 **asUser** | **string** | specifies a username identifying the user who ran the job. Requires &#x60;runAs&#x60; permission. | 
 **filter** | **string** | can be a node filter string. | 
 **runAtTime** | **time.Time** | Specify a time to run the job (Since: v18).  This is a ISO-8601 date and time stamp with timezone, with optional milliseconds., e.g. &#x60;2016-11-23T12:20:55-0800&#x60; or &#x60;2016-11-23T12:20:55.123-0800&#x60; | 
 **optionOPTNAME** | **string** | Option value for option named &#x60;OPTNAME&#x60;. If any &#x60;option.OPTNAME&#x60; parameters are specified, the &#x60;argString&#x60; value is ignored (Since: v18). | 
 **metaKEY** | **string** | Additional metadata keyd by &#x60;KEY&#x60;. (Since: v32). | 
 **body** | **map[string]interface{}** | Parameters can be specified in the request body, instead of as query parameters.  (**API v18** or later): The &#x60;options&#x60; entry can contain a map of option name -&gt; value, in which case the &#x60;argString&#x60; is ignored. | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobRun1

> ApiJobRun1(ctx, id).ArgString(argString).Loglevel(loglevel).AsUser(asUser).Filter(filter).RunAtTime(runAtTime).OptionOPTNAME(optionOPTNAME).MetaKEY(metaKEY).Body(body).Execute()

Running a Job



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/rundeck/go-rundeck"
)

func main() {
	id := "id_example" // string | Job ID
	argString := "argString_example" // string | argument string to pass to the job, of the form: `-opt value -opt2 value ...`. (optional)
	loglevel := "loglevel_example" // string | argument specifying the loglevel to use (optional)
	asUser := "asUser_example" // string | specifies a username identifying the user who ran the job. Requires `runAs` permission. (optional)
	filter := "filter_example" // string | can be a node filter string. (optional)
	runAtTime := time.Now() // time.Time | Specify a time to run the job (Since: v18).  This is a ISO-8601 date and time stamp with timezone, with optional milliseconds., e.g. `2016-11-23T12:20:55-0800` or `2016-11-23T12:20:55.123-0800` (optional)
	optionOPTNAME := "optionOPTNAME_example" // string | Option value for option named `OPTNAME`. If any `option.OPTNAME` parameters are specified, the `argString` value is ignored (Since: v18). (optional)
	metaKEY := "metaKEY_example" // string | Additional metadata keyd by `KEY`. (Since: v32). (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} | Parameters can be specified in the request body, instead of as query parameters.  (**API v18** or later): The `options` entry can contain a map of option name -> value, in which case the `argString` is ignored. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.JobsAPI.ApiJobRun1(context.Background(), id).ArgString(argString).Loglevel(loglevel).AsUser(asUser).Filter(filter).RunAtTime(runAtTime).OptionOPTNAME(optionOPTNAME).MetaKEY(metaKEY).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobRun1``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobRun1Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **argString** | **string** | argument string to pass to the job, of the form: &#x60;-opt value -opt2 value ...&#x60;. | 
 **loglevel** | **string** | argument specifying the loglevel to use | 
 **asUser** | **string** | specifies a username identifying the user who ran the job. Requires &#x60;runAs&#x60; permission. | 
 **filter** | **string** | can be a node filter string. | 
 **runAtTime** | **time.Time** | Specify a time to run the job (Since: v18).  This is a ISO-8601 date and time stamp with timezone, with optional milliseconds., e.g. &#x60;2016-11-23T12:20:55-0800&#x60; or &#x60;2016-11-23T12:20:55.123-0800&#x60; | 
 **optionOPTNAME** | **string** | Option value for option named &#x60;OPTNAME&#x60;. If any &#x60;option.OPTNAME&#x60; parameters are specified, the &#x60;argString&#x60; value is ignored (Since: v18). | 
 **metaKEY** | **string** | Additional metadata keyd by &#x60;KEY&#x60;. (Since: v32). | 
 **body** | **map[string]interface{}** | Parameters can be specified in the request body, instead of as query parameters.  (**API v18** or later): The &#x60;options&#x60; entry can contain a map of option name -&gt; value, in which case the &#x60;argString&#x60; is ignored. | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobWorkflow

> map[string]interface{} ApiJobWorkflow(ctx, id).Execute()

Get Job Workflow



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
	id := "id_example" // string | Job ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobWorkflow(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobWorkflow``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobWorkflow`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobWorkflow`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Job ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobWorkflowRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobsExportv14

> map[string]interface{} ApiJobsExportv14(ctx, project).Idlist(idlist).GroupPath(groupPath).JobFilter(jobFilter).Format(format).JobExactFilter(jobExactFilter).ProjFilter(projFilter).GroupPathExact(groupPathExact).DescFilter(descFilter).LoglevelFilter(loglevelFilter).ScheduledFilter(scheduledFilter).ScheduleEnabledFilter(scheduleEnabledFilter).ExecutionEnabledFilter(executionEnabledFilter).ServerNodeUUIDFilter(serverNodeUUIDFilter).DaysAhead(daysAhead).RunJobLaterFilter(runJobLaterFilter).PaginatedRequired(paginatedRequired).Execute()

Export Jobs



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
	project := "project_example" // string | Project Name
	idlist := "idlist_example" // string | A comma-separated list of Job IDs to export (optional)
	groupPath := "groupPath_example" // string | specify a group or partial group path to include all jobs within that group path. (optional)
	jobFilter := "jobFilter_example" // string | specify a filter for the job Name (optional)
	format := "format_example" // string | can be \"yaml\" or \"json\" (API v44+) to specify the output format (optional)
	jobExactFilter := "jobExactFilter_example" // string |  (optional)
	projFilter := "projFilter_example" // string |  (optional)
	groupPathExact := "groupPathExact_example" // string |  (optional)
	descFilter := "descFilter_example" // string |  (optional)
	loglevelFilter := "loglevelFilter_example" // string |  (optional)
	scheduledFilter := true // bool |  (optional)
	scheduleEnabledFilter := true // bool |  (optional)
	executionEnabledFilter := true // bool |  (optional)
	serverNodeUUIDFilter := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string |  (optional)
	daysAhead := int32(56) // int32 |  (optional)
	runJobLaterFilter := true // bool |  (optional)
	paginatedRequired := true // bool |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobsExportv14(context.Background(), project).Idlist(idlist).GroupPath(groupPath).JobFilter(jobFilter).Format(format).JobExactFilter(jobExactFilter).ProjFilter(projFilter).GroupPathExact(groupPathExact).DescFilter(descFilter).LoglevelFilter(loglevelFilter).ScheduledFilter(scheduledFilter).ScheduleEnabledFilter(scheduleEnabledFilter).ExecutionEnabledFilter(executionEnabledFilter).ServerNodeUUIDFilter(serverNodeUUIDFilter).DaysAhead(daysAhead).RunJobLaterFilter(runJobLaterFilter).PaginatedRequired(paginatedRequired).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobsExportv14``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobsExportv14`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobsExportv14`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobsExportv14Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **idlist** | **string** | A comma-separated list of Job IDs to export | 
 **groupPath** | **string** | specify a group or partial group path to include all jobs within that group path. | 
 **jobFilter** | **string** | specify a filter for the job Name | 
 **format** | **string** | can be \&quot;yaml\&quot; or \&quot;json\&quot; (API v44+) to specify the output format | 
 **jobExactFilter** | **string** |  | 
 **projFilter** | **string** |  | 
 **groupPathExact** | **string** |  | 
 **descFilter** | **string** |  | 
 **loglevelFilter** | **string** |  | 
 **scheduledFilter** | **bool** |  | 
 **scheduleEnabledFilter** | **bool** |  | 
 **executionEnabledFilter** | **bool** |  | 
 **serverNodeUUIDFilter** | **string** |  | 
 **daysAhead** | **int32** |  | 
 **runJobLaterFilter** | **bool** |  | 
 **paginatedRequired** | **bool** |  | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/yaml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobsImportv14

> ApiJobsImportv14(ctx, project).Fileformat(fileformat).DupeOption(dupeOption).UuidOption(uuidOption).Execute()

Import Job definitions



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
	project := "project_example" // string | Project Name
	fileformat := "fileformat_example" // string | Input file format, to specify the input format, if multipart of form input is sent. (optional)
	dupeOption := "dupeOption_example" // string | A value to indicate the behavior when importing jobs which already exist.  Value can be \"skip\", \"create\", or \"update\". Default is \"create\". (optional)
	uuidOption := "uuidOption_example" // string | Whether to preserve or remove UUIDs from the imported jobs:  *  `preserve`: Preserve the UUIDs in imported jobs.  This may cause the import to fail if the UUID is already used. (Default value). *  `remove`: Remove the UUIDs from imported jobs. Allows update/create to succeed without conflict on UUID.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.JobsAPI.ApiJobsImportv14(context.Background(), project).Fileformat(fileformat).DupeOption(dupeOption).UuidOption(uuidOption).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobsImportv14``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobsImportv14Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fileformat** | **string** | Input file format, to specify the input format, if multipart of form input is sent. | 
 **dupeOption** | **string** | A value to indicate the behavior when importing jobs which already exist.  Value can be \&quot;skip\&quot;, \&quot;create\&quot;, or \&quot;update\&quot;. Default is \&quot;create\&quot;. | 
 **uuidOption** | **string** | Whether to preserve or remove UUIDs from the imported jobs:  *  &#x60;preserve&#x60;: Preserve the UUIDs in imported jobs.  This may cause the import to fail if the UUID is already used. (Default value). *  &#x60;remove&#x60;: Remove the UUIDs from imported jobs. Allows update/create to succeed without conflict on UUID.  | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded, multipart/form-data, application/json, text/yaml
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobsImportv14_0

> ApiJobsImportv14_0(ctx, project).Fileformat(fileformat).DupeOption(dupeOption).UuidOption(uuidOption).Execute()

Import Job definitions



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
	project := "project_example" // string | Project Name
	fileformat := "fileformat_example" // string | Input file format, to specify the input format, if multipart of form input is sent. (optional)
	dupeOption := "dupeOption_example" // string | A value to indicate the behavior when importing jobs which already exist.  Value can be \"skip\", \"create\", or \"update\". Default is \"create\". (optional)
	uuidOption := "uuidOption_example" // string | Whether to preserve or remove UUIDs from the imported jobs:  *  `preserve`: Preserve the UUIDs in imported jobs.  This may cause the import to fail if the UUID is already used. (Default value). *  `remove`: Remove the UUIDs from imported jobs. Allows update/create to succeed without conflict on UUID.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.JobsAPI.ApiJobsImportv14_0(context.Background(), project).Fileformat(fileformat).DupeOption(dupeOption).UuidOption(uuidOption).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobsImportv14_0``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobsImportv14_1Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fileformat** | **string** | Input file format, to specify the input format, if multipart of form input is sent. | 
 **dupeOption** | **string** | A value to indicate the behavior when importing jobs which already exist.  Value can be \&quot;skip\&quot;, \&quot;create\&quot;, or \&quot;update\&quot;. Default is \&quot;create\&quot;. | 
 **uuidOption** | **string** | Whether to preserve or remove UUIDs from the imported jobs:  *  &#x60;preserve&#x60;: Preserve the UUIDs in imported jobs.  This may cause the import to fail if the UUID is already used. (Default value). *  &#x60;remove&#x60;: Remove the UUIDs from imported jobs. Allows update/create to succeed without conflict on UUID.  | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded, multipart/form-data, application/json, text/yaml
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiJobsListv2

> []JobInfo ApiJobsListv2(ctx, project).Max(max).Offset(offset).Tags(tags).JobFilter(jobFilter).JobExactFilter(jobExactFilter).ProjFilter(projFilter).GroupPath(groupPath).GroupPathExact(groupPathExact).DescFilter(descFilter).LoglevelFilter(loglevelFilter).Idlist(idlist).ScheduledFilter(scheduledFilter).ScheduleEnabledFilter(scheduleEnabledFilter).ExecutionEnabledFilter(executionEnabledFilter).ServerNodeUUIDFilter(serverNodeUUIDFilter).DaysAhead(daysAhead).RunJobLaterFilter(runJobLaterFilter).PaginatedRequired(paginatedRequired).Execute()

Listing Jobs



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
	project := "project_example" // string | Project Name
	max := int32(56) // int32 | limit the maximum amount of results to be received. (optional)
	offset := int32(56) // int32 | use in conjunction with `max` to paginate the result set. (optional)
	tags := int32(56) // int32 | specify a tag or comma separated list of tags to list Jobs that have matching tags. (e.g. `tags=tag1,tag2`) (optional)
	jobFilter := "jobFilter_example" // string |  (optional)
	jobExactFilter := "jobExactFilter_example" // string |  (optional)
	projFilter := "projFilter_example" // string |  (optional)
	groupPath := "groupPath_example" // string |  (optional)
	groupPathExact := "groupPathExact_example" // string |  (optional)
	descFilter := "descFilter_example" // string |  (optional)
	loglevelFilter := "loglevelFilter_example" // string |  (optional)
	idlist := "idlist_example" // string |  (optional)
	scheduledFilter := true // bool |  (optional)
	scheduleEnabledFilter := true // bool |  (optional)
	executionEnabledFilter := true // bool |  (optional)
	serverNodeUUIDFilter := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string |  (optional)
	daysAhead := int32(56) // int32 |  (optional)
	runJobLaterFilter := true // bool |  (optional)
	paginatedRequired := true // bool |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiJobsListv2(context.Background(), project).Max(max).Offset(offset).Tags(tags).JobFilter(jobFilter).JobExactFilter(jobExactFilter).ProjFilter(projFilter).GroupPath(groupPath).GroupPathExact(groupPathExact).DescFilter(descFilter).LoglevelFilter(loglevelFilter).Idlist(idlist).ScheduledFilter(scheduledFilter).ScheduleEnabledFilter(scheduleEnabledFilter).ExecutionEnabledFilter(executionEnabledFilter).ServerNodeUUIDFilter(serverNodeUUIDFilter).DaysAhead(daysAhead).RunJobLaterFilter(runJobLaterFilter).PaginatedRequired(paginatedRequired).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiJobsListv2``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiJobsListv2`: []JobInfo
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiJobsListv2`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiJobsListv2Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **max** | **int32** | limit the maximum amount of results to be received. | 
 **offset** | **int32** | use in conjunction with &#x60;max&#x60; to paginate the result set. | 
 **tags** | **int32** | specify a tag or comma separated list of tags to list Jobs that have matching tags. (e.g. &#x60;tags&#x3D;tag1,tag2&#x60;) | 
 **jobFilter** | **string** |  | 
 **jobExactFilter** | **string** |  | 
 **projFilter** | **string** |  | 
 **groupPath** | **string** |  | 
 **groupPathExact** | **string** |  | 
 **descFilter** | **string** |  | 
 **loglevelFilter** | **string** |  | 
 **idlist** | **string** |  | 
 **scheduledFilter** | **bool** |  | 
 **scheduleEnabledFilter** | **bool** |  | 
 **executionEnabledFilter** | **bool** |  | 
 **serverNodeUUIDFilter** | **string** |  | 
 **daysAhead** | **int32** |  | 
 **runJobLaterFilter** | **bool** |  | 
 **paginatedRequired** | **bool** |  | 

### Return type

[**[]JobInfo**](JobInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiListAllJobsInProject

> []map[string]interface{} ApiListAllJobsInProject(ctx, project).Execute()

List all Jobs in Summarized Form [Enterprise]



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
	project := "project_example" // string | Project Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiListAllJobsInProject(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiListAllJobsInProject``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiListAllJobsInProject`: []map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiListAllJobsInProject`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiListAllJobsInProjectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**[]map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSchedulerListJobs

> []JobInfo ApiSchedulerListJobs(ctx, uuid).Execute()

List Scheduled Jobs For a Cluster Server



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
	uuid := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Server UUID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.ApiSchedulerListJobs(context.Background(), uuid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiSchedulerListJobs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSchedulerListJobs`: []JobInfo
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiSchedulerListJobs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**uuid** | **string** | Server UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSchedulerListJobsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]JobInfo**](JobInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSchedulerListJobsCurrentDocs

> []JobInfo ApiSchedulerListJobsCurrentDocs(ctx).Execute()

List Scheduled Jobs For this Cluster Server



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
	resp, r, err := apiClient.JobsAPI.ApiSchedulerListJobsCurrentDocs(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ApiSchedulerListJobsCurrentDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSchedulerListJobsCurrentDocs`: []JobInfo
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ApiSchedulerListJobsCurrentDocs`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiSchedulerListJobsCurrentDocsRequest struct via the builder pattern


### Return type

[**[]JobInfo**](JobInfo.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


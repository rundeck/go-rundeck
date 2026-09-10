# \JobExecutionsAPI

All URIs are relative to *https://localhost:4440/api/59*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiExecution**](JobExecutionsAPI.md#ApiExecution) | **Get** /execution/{id} | Execution Info
[**ApiExecutionAbort**](JobExecutionsAPI.md#ApiExecutionAbort) | **Post** /execution/{id}/abort | Aborting Executions
[**ApiExecutionDelete**](JobExecutionsAPI.md#ApiExecutionDelete) | **Delete** /execution/{id} | Delete an Execution
[**ApiExecutionDeleteBulk**](JobExecutionsAPI.md#ApiExecutionDeleteBulk) | **Post** /executions/delete | Bulk Delete Executions
[**ApiExecutionInputFiles**](JobExecutionsAPI.md#ApiExecutionInputFiles) | **Get** /execution/{id}/input/files | List Input Files for an Execution
[**ApiExecutionMetricsDocs**](JobExecutionsAPI.md#ApiExecutionMetricsDocs) | **Get** /executions/metrics | Execution Query Metrics
[**ApiExecutionMetricsProjectDocs**](JobExecutionsAPI.md#ApiExecutionMetricsProjectDocs) | **Get** /project/{project}/executions/metrics | Execution Query Metrics
[**ApiExecutionOutput**](JobExecutionsAPI.md#ApiExecutionOutput) | **Get** /execution/{id}/output | Execution Output
[**ApiExecutionOutputNodeFilter**](JobExecutionsAPI.md#ApiExecutionOutputNodeFilter) | **Get** /execution/{id}/output/node/{nodename} | Execution Output For Node
[**ApiExecutionOutputNodeStepFilter**](JobExecutionsAPI.md#ApiExecutionOutputNodeStepFilter) | **Get** /execution/{id}/output/node/{nodename}/step/{stepctx} | Execution Output For Node and Step
[**ApiExecutionOutputStepFilter**](JobExecutionsAPI.md#ApiExecutionOutputStepFilter) | **Get** /execution/{id}/output/step/{stepctx} | Execution Output For Step
[**ApiExecutionState**](JobExecutionsAPI.md#ApiExecutionState) | **Get** /execution/{id}/state | Execution State
[**ApiExecutionStateOutput**](JobExecutionsAPI.md#ApiExecutionStateOutput) | **Get** /execution/{id}/output/state | Execution Output with State
[**ApiExecutionsQueryv14Docs**](JobExecutionsAPI.md#ApiExecutionsQueryv14Docs) | **Get** /project/{project}/executions | Execution Query
[**ApiExecutionsRunningv14**](JobExecutionsAPI.md#ApiExecutionsRunningv14) | **Get** /project/{project}/executions/running | Listing Running Executions
[**ApiHomeSummary**](JobExecutionsAPI.md#ApiHomeSummary) | **Get** /home/summary | Summary of executions and projects



## ApiExecution

> ApiExecution(ctx, id).Execute()

Execution Info



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
	r, err := apiClient.JobExecutionsAPI.ApiExecution(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecution``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiExecutionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


## ApiExecutionAbort

> ApiExecutionAbort(ctx, id).AsUser(asUser).ForceIncomplete(forceIncomplete).Execute()

Aborting Executions



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
	asUser := "asUser_example" // string | Specifies a username identifying the user who aborted the execution. Requires `runAs` actiion authorization. (optional)
	forceIncomplete := true // bool | if `true`, forces a running execution to be marked as \"incomplete\". (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.JobExecutionsAPI.ApiExecutionAbort(context.Background(), id).AsUser(asUser).ForceIncomplete(forceIncomplete).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionAbort``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiExecutionAbortRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **asUser** | **string** | Specifies a username identifying the user who aborted the execution. Requires &#x60;runAs&#x60; actiion authorization. | 
 **forceIncomplete** | **bool** | if &#x60;true&#x60;, forces a running execution to be marked as \&quot;incomplete\&quot;. | 

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


## ApiExecutionDelete

> ApiExecutionDelete(ctx, id).Execute()

Delete an Execution



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
	r, err := apiClient.JobExecutionsAPI.ApiExecutionDelete(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionDelete``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiExecutionDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionDeleteBulk

> DeleteBulkResponse ApiExecutionDeleteBulk(ctx).Ids(ids).ApiExecutionDeleteBulkRequest(apiExecutionDeleteBulkRequest).Execute()

Bulk Delete Executions



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
	ids := "ids_example" // string | comma separated list of IDs (optional)
	apiExecutionDeleteBulkRequest := openapiclient.apiExecutionDeleteBulk_request{DeleteBulkRequest: openapiclient.NewDeleteBulkRequest()} // ApiExecutionDeleteBulkRequest | Delete Bulk IDs request. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionDeleteBulk(context.Background()).Ids(ids).ApiExecutionDeleteBulkRequest(apiExecutionDeleteBulkRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionDeleteBulk``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionDeleteBulk`: DeleteBulkResponse
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionDeleteBulk`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionDeleteBulkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **string** | comma separated list of IDs | 
 **apiExecutionDeleteBulkRequest** | [**ApiExecutionDeleteBulkRequest**](ApiExecutionDeleteBulkRequest.md) | Delete Bulk IDs request. | 

### Return type

[**DeleteBulkResponse**](DeleteBulkResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionInputFiles

> ExecutionFileInfoList ApiExecutionInputFiles(ctx, id).Execute()

List Input Files for an Execution



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
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionInputFiles(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionInputFiles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionInputFiles`: ExecutionFileInfoList
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionInputFiles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionInputFilesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ExecutionFileInfoList**](ExecutionFileInfoList.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionMetricsDocs

> MetricsQueryResponse ApiExecutionMetricsDocs(ctx).Project(project).StatusFilter(statusFilter).AbortedbyFilter(abortedbyFilter).JobIdListFilter(jobIdListFilter).ExcludeJobIdListFilter(excludeJobIdListFilter).JobListFilter(jobListFilter).ExcludeJobListFilter(excludeJobListFilter).GroupPath(groupPath).GroupPathExact(groupPathExact).ExcludeGroupPath(excludeGroupPath).ExcludeGroupPathExact(excludeGroupPathExact).JobFilter(jobFilter).ExcludeJobFilter(excludeJobFilter).JobExactFilter(jobExactFilter).ExcludeJobExactFilter(excludeJobExactFilter).StartafterFilter(startafterFilter).StartbeforeFilter(startbeforeFilter).EndafterFilter(endafterFilter).EndbeforeFilter(endbeforeFilter).Begin(begin).End(end).Adhoc(adhoc).RecentFilter(recentFilter).OlderFilter(olderFilter).UserFilter(userFilter).ExecutionTypeFilter(executionTypeFilter).UseStats(useStats).GroupByJob(groupByJob).Max(max).Offset(offset).Execute()

Execution Query Metrics



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
	project := "project_example" // string | Project name (optional)
	statusFilter := "statusFilter_example" // string | Execution status (optional)
	abortedbyFilter := "abortedbyFilter_example" // string | Username who aborted an execution (optional)
	jobIdListFilter := "jobIdListFilter_example" // string | specify a Job ID to include, can be specified multiple times (optional)
	excludeJobIdListFilter := "excludeJobIdListFilter_example" // string | specify a Job ID to exclude, can be specified multiple times (optional)
	jobListFilter := "jobListFilter_example" // string | specify a full Job group/name to include, can be specified multiple times (optional)
	excludeJobListFilter := "excludeJobListFilter_example" // string | specify a full Job group/name to exclude, can be specified multiple times (optional)
	groupPath := "groupPath_example" // string | specify a group or partial group path to include all jobs within that group path. Set to the special value \"-\" to match the top level jobs only. (optional)
	groupPathExact := "groupPathExact_example" // string | specify an exact group path to match.  Set to the special value \"-\" to match the top level jobs only. (optional)
	excludeGroupPath := "excludeGroupPath_example" // string | specify a group or partial group path to exclude all jobs within that group path. Set to the special value \"-\" to match the top level jobs only. (optional)
	excludeGroupPathExact := "excludeGroupPathExact_example" // string | specify an exact group path to exclude.  Set to the special value \"-\" to match the top level jobs only. (optional)
	jobFilter := "jobFilter_example" // string | specify a filter for the job Name. Include any job name that matches this value (optional)
	excludeJobFilter := "excludeJobFilter_example" // string | specify a filter for the job Name. Exclude any job name that matches this value. (optional)
	jobExactFilter := "jobExactFilter_example" // string | specify an exact job name to match. (optional)
	excludeJobExactFilter := "excludeJobExactFilter_example" // string | specify an exact job name to exclude. (optional)
	startafterFilter := "startafterFilter_example" // string | start after date (optional)
	startbeforeFilter := "startbeforeFilter_example" // string | start before date (optional)
	endafterFilter := "endafterFilter_example" // string | end after date (optional)
	endbeforeFilter := "endbeforeFilter_example" // string | end before date (optional)
	begin := "begin_example" // string | Specify exact date for earliest execution completion time. Format: a unix millisecond timestamp, or a W3C dateTime string in the format \"yyyy-MM-ddTHH:mm:ssZ\". (optional)
	end := "end_example" // string | Specify exact date for latest execution completion time. Format: a unix millisecond timestamp, or a W3C dateTime string in the format \"yyyy-MM-ddTHH:mm:ssZ\". (optional)
	adhoc := true // bool | if true, include only Adhoc executions, if false return only Job executions. By default any matching executions are returned, however if you use any of the Job filters below, then only Job executions will be returned. (optional)
	recentFilter := "recentFilter_example" // string | Use a simple text format to filter executions that completed within a period of time. The format is \"XY\" where X is an integer, and \"Y\" is one of: * `s`: second * `n`: minute * `h`: hour * `d`: day * `w`: week * `m`: month * `y`: year  So a value of `2w` would return executions that completed within the last two weeks.  (optional)
	olderFilter := "olderFilter_example" // string | (same format as `recentFilter`) return executions that completed before the specified relative period of time.  E.g. a value of `30d` returns executions older than 30 days. (optional)
	userFilter := "userFilter_example" // string | Username who started the execution (optional)
	executionTypeFilter := "executionTypeFilter_example" // string | specify the execution type, one of: `scheduled` (schedule trigger), `user` (user trigger), `user-scheduled` (user scheduled trigger). Since: v20 (optional)
	useStats := true // bool | if true, use snapshot-based metrics from SCHEDULED_EXECUTION_STATS table (fast, returns empty metrics (all zeros) if no stats exist). if false or not provided, use execution table query (slow, always returns data). Since: v57 (optional)
	groupByJob := true // bool | if true with useStats=true, returns metrics for all jobs in the project (batch mode). Requires project parameter. Returns format: {jobs: {uuid1: metrics, uuid2: metrics, ...}}. RUN-3768 Phase 5. Since: v57 (optional)
	max := int32(56) // int32 | maximum number of results to include in response. (default: 20) (optional)
	offset := int32(56) // int32 | offset for first result to include. (default: 0) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionMetricsDocs(context.Background()).Project(project).StatusFilter(statusFilter).AbortedbyFilter(abortedbyFilter).JobIdListFilter(jobIdListFilter).ExcludeJobIdListFilter(excludeJobIdListFilter).JobListFilter(jobListFilter).ExcludeJobListFilter(excludeJobListFilter).GroupPath(groupPath).GroupPathExact(groupPathExact).ExcludeGroupPath(excludeGroupPath).ExcludeGroupPathExact(excludeGroupPathExact).JobFilter(jobFilter).ExcludeJobFilter(excludeJobFilter).JobExactFilter(jobExactFilter).ExcludeJobExactFilter(excludeJobExactFilter).StartafterFilter(startafterFilter).StartbeforeFilter(startbeforeFilter).EndafterFilter(endafterFilter).EndbeforeFilter(endbeforeFilter).Begin(begin).End(end).Adhoc(adhoc).RecentFilter(recentFilter).OlderFilter(olderFilter).UserFilter(userFilter).ExecutionTypeFilter(executionTypeFilter).UseStats(useStats).GroupByJob(groupByJob).Max(max).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionMetricsDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionMetricsDocs`: MetricsQueryResponse
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionMetricsDocs`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionMetricsDocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | **string** | Project name | 
 **statusFilter** | **string** | Execution status | 
 **abortedbyFilter** | **string** | Username who aborted an execution | 
 **jobIdListFilter** | **string** | specify a Job ID to include, can be specified multiple times | 
 **excludeJobIdListFilter** | **string** | specify a Job ID to exclude, can be specified multiple times | 
 **jobListFilter** | **string** | specify a full Job group/name to include, can be specified multiple times | 
 **excludeJobListFilter** | **string** | specify a full Job group/name to exclude, can be specified multiple times | 
 **groupPath** | **string** | specify a group or partial group path to include all jobs within that group path. Set to the special value \&quot;-\&quot; to match the top level jobs only. | 
 **groupPathExact** | **string** | specify an exact group path to match.  Set to the special value \&quot;-\&quot; to match the top level jobs only. | 
 **excludeGroupPath** | **string** | specify a group or partial group path to exclude all jobs within that group path. Set to the special value \&quot;-\&quot; to match the top level jobs only. | 
 **excludeGroupPathExact** | **string** | specify an exact group path to exclude.  Set to the special value \&quot;-\&quot; to match the top level jobs only. | 
 **jobFilter** | **string** | specify a filter for the job Name. Include any job name that matches this value | 
 **excludeJobFilter** | **string** | specify a filter for the job Name. Exclude any job name that matches this value. | 
 **jobExactFilter** | **string** | specify an exact job name to match. | 
 **excludeJobExactFilter** | **string** | specify an exact job name to exclude. | 
 **startafterFilter** | **string** | start after date | 
 **startbeforeFilter** | **string** | start before date | 
 **endafterFilter** | **string** | end after date | 
 **endbeforeFilter** | **string** | end before date | 
 **begin** | **string** | Specify exact date for earliest execution completion time. Format: a unix millisecond timestamp, or a W3C dateTime string in the format \&quot;yyyy-MM-ddTHH:mm:ssZ\&quot;. | 
 **end** | **string** | Specify exact date for latest execution completion time. Format: a unix millisecond timestamp, or a W3C dateTime string in the format \&quot;yyyy-MM-ddTHH:mm:ssZ\&quot;. | 
 **adhoc** | **bool** | if true, include only Adhoc executions, if false return only Job executions. By default any matching executions are returned, however if you use any of the Job filters below, then only Job executions will be returned. | 
 **recentFilter** | **string** | Use a simple text format to filter executions that completed within a period of time. The format is \&quot;XY\&quot; where X is an integer, and \&quot;Y\&quot; is one of: * &#x60;s&#x60;: second * &#x60;n&#x60;: minute * &#x60;h&#x60;: hour * &#x60;d&#x60;: day * &#x60;w&#x60;: week * &#x60;m&#x60;: month * &#x60;y&#x60;: year  So a value of &#x60;2w&#x60; would return executions that completed within the last two weeks.  | 
 **olderFilter** | **string** | (same format as &#x60;recentFilter&#x60;) return executions that completed before the specified relative period of time.  E.g. a value of &#x60;30d&#x60; returns executions older than 30 days. | 
 **userFilter** | **string** | Username who started the execution | 
 **executionTypeFilter** | **string** | specify the execution type, one of: &#x60;scheduled&#x60; (schedule trigger), &#x60;user&#x60; (user trigger), &#x60;user-scheduled&#x60; (user scheduled trigger). Since: v20 | 
 **useStats** | **bool** | if true, use snapshot-based metrics from SCHEDULED_EXECUTION_STATS table (fast, returns empty metrics (all zeros) if no stats exist). if false or not provided, use execution table query (slow, always returns data). Since: v57 | 
 **groupByJob** | **bool** | if true with useStats&#x3D;true, returns metrics for all jobs in the project (batch mode). Requires project parameter. Returns format: {jobs: {uuid1: metrics, uuid2: metrics, ...}}. RUN-3768 Phase 5. Since: v57 | 
 **max** | **int32** | maximum number of results to include in response. (default: 20) | 
 **offset** | **int32** | offset for first result to include. (default: 0) | 

### Return type

[**MetricsQueryResponse**](MetricsQueryResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionMetricsProjectDocs

> MetricsQueryResponse ApiExecutionMetricsProjectDocs(ctx, project).Execute()

Execution Query Metrics



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionMetricsProjectDocs(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionMetricsProjectDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionMetricsProjectDocs`: MetricsQueryResponse
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionMetricsProjectDocs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionMetricsProjectDocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**MetricsQueryResponse**](MetricsQueryResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionOutput

> map[string]interface{} ApiExecutionOutput(ctx, id).Nodename(nodename).Stepctx(stepctx).Offset(offset).Lastlines(lastlines).Lastmod(lastmod).Maxlines(maxlines).Compacted(compacted).Format(format).Execute()

Execution Output



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
	nodename := "nodename_example" // string | Node Name, all results will be filtered for only this node. (optional)
	stepctx := "stepctx_example" // string | Step Context ID. This is a string in the form `1/2/3` indicating the step context. (optional)
	offset := int32(56) // int32 | byte offset to read from in the file. 0 indicates the beginning. (optional)
	lastlines := int32(56) // int32 | number of lines to retrieve from the end of the available output. If specified it will override the `offset` value and return only the specified number of lines at the end of the log. (optional)
	lastmod := int64(789) // int64 | epoch datestamp in milliseconds, return results only if modification changed since the specified date OR if more data is available at the given `offset`. (optional)
	maxlines := int32(56) // int32 | maximum number of lines to retrieve forward from the specified offset. (optional)
	compacted := true // bool | if true, results will be in compacted form. Since: v21 (optional)
	format := "format_example" // string | Specify output format (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionOutput(context.Background(), id).Nodename(nodename).Stepctx(stepctx).Offset(offset).Lastlines(lastlines).Lastmod(lastmod).Maxlines(maxlines).Compacted(compacted).Format(format).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionOutput``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionOutput`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionOutput`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionOutputRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **nodename** | **string** | Node Name, all results will be filtered for only this node. | 
 **stepctx** | **string** | Step Context ID. This is a string in the form &#x60;1/2/3&#x60; indicating the step context. | 
 **offset** | **int32** | byte offset to read from in the file. 0 indicates the beginning. | 
 **lastlines** | **int32** | number of lines to retrieve from the end of the available output. If specified it will override the &#x60;offset&#x60; value and return only the specified number of lines at the end of the log. | 
 **lastmod** | **int64** | epoch datestamp in milliseconds, return results only if modification changed since the specified date OR if more data is available at the given &#x60;offset&#x60;. | 
 **maxlines** | **int32** | maximum number of lines to retrieve forward from the specified offset. | 
 **compacted** | **bool** | if true, results will be in compacted form. Since: v21 | 
 **format** | **string** | Specify output format | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiExecutionOutputNodeFilter

> map[string]interface{} ApiExecutionOutputNodeFilter(ctx, id, nodename).Execute()

Execution Output For Node



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
	nodename := "nodename_example" // string | Node Name, all results will be filtered for only this node.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionOutputNodeFilter(context.Background(), id, nodename).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionOutputNodeFilter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionOutputNodeFilter`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionOutputNodeFilter`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 
**nodename** | **string** | Node Name, all results will be filtered for only this node. | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionOutputNodeFilterRequest struct via the builder pattern


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


## ApiExecutionOutputNodeStepFilter

> map[string]interface{} ApiExecutionOutputNodeStepFilter(ctx, id, nodename, stepctx).Execute()

Execution Output For Node and Step



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
	nodename := "nodename_example" // string | Node Name, all results will be filtered for only this node.
	stepctx := "stepctx_example" // string | Step Context ID. This is a string in the form `1/2/3` indicating the step context.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionOutputNodeStepFilter(context.Background(), id, nodename, stepctx).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionOutputNodeStepFilter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionOutputNodeStepFilter`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionOutputNodeStepFilter`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 
**nodename** | **string** | Node Name, all results will be filtered for only this node. | 
**stepctx** | **string** | Step Context ID. This is a string in the form &#x60;1/2/3&#x60; indicating the step context. | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionOutputNodeStepFilterRequest struct via the builder pattern


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


## ApiExecutionOutputStepFilter

> map[string]interface{} ApiExecutionOutputStepFilter(ctx, id, stepctx).Execute()

Execution Output For Step



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
	stepctx := "stepctx_example" // string | Step Context ID. This is a string in the form `1/2/3` indicating the step context.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionOutputStepFilter(context.Background(), id, stepctx).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionOutputStepFilter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionOutputStepFilter`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionOutputStepFilter`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 
**stepctx** | **string** | Step Context ID. This is a string in the form &#x60;1/2/3&#x60; indicating the step context. | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionOutputStepFilterRequest struct via the builder pattern


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


## ApiExecutionState

> map[string]interface{} ApiExecutionState(ctx, id).Execute()

Execution State



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
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionState(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionState``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionState`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionState`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionStateRequest struct via the builder pattern


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


## ApiExecutionStateOutput

> map[string]interface{} ApiExecutionStateOutput(ctx, id).StateOnly(stateOnly).Execute()

Execution Output with State



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
	stateOnly := true // bool | Whether to include only state information. When false, log entries will be included. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionStateOutput(context.Background(), id).StateOnly(stateOnly).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionStateOutput``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionStateOutput`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionStateOutput`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Execution ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionStateOutputRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **stateOnly** | **bool** | Whether to include only state information. When false, log entries will be included. | 

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


## ApiExecutionsQueryv14Docs

> ApiExecutionsQueryv14Docs(ctx, project).StatusFilter(statusFilter).AbortedbyFilter(abortedbyFilter).JobIdListFilter(jobIdListFilter).ExcludeJobIdListFilter(excludeJobIdListFilter).JobListFilter(jobListFilter).ExcludeJobListFilter(excludeJobListFilter).GroupPath(groupPath).GroupPathExact(groupPathExact).ExcludeGroupPath(excludeGroupPath).ExcludeGroupPathExact(excludeGroupPathExact).JobFilter(jobFilter).ExcludeJobFilter(excludeJobFilter).JobExactFilter(jobExactFilter).ExcludeJobExactFilter(excludeJobExactFilter).StartafterFilter(startafterFilter).StartbeforeFilter(startbeforeFilter).EndafterFilter(endafterFilter).EndbeforeFilter(endbeforeFilter).Begin(begin).End(end).Adhoc(adhoc).RecentFilter(recentFilter).OlderFilter(olderFilter).UserFilter(userFilter).ExecutionTypeFilter(executionTypeFilter).UseStats(useStats).GroupByJob(groupByJob).AdhocStringFilter(adhocStringFilter).NodeFilter(nodeFilter).OptionFilter(optionFilter).Max(max).Offset(offset).Execute()

Execution Query



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
	statusFilter := "statusFilter_example" // string | Execution status (optional)
	abortedbyFilter := "abortedbyFilter_example" // string | Username who aborted an execution (optional)
	jobIdListFilter := "jobIdListFilter_example" // string | specify a Job ID to include, can be specified multiple times (optional)
	excludeJobIdListFilter := "excludeJobIdListFilter_example" // string | specify a Job ID to exclude, can be specified multiple times (optional)
	jobListFilter := "jobListFilter_example" // string | specify a full Job group/name to include, can be specified multiple times (optional)
	excludeJobListFilter := "excludeJobListFilter_example" // string | specify a full Job group/name to exclude, can be specified multiple times (optional)
	groupPath := "groupPath_example" // string | specify a group or partial group path to include all jobs within that group path. Set to the special value \"-\" to match the top level jobs only. (optional)
	groupPathExact := "groupPathExact_example" // string | specify an exact group path to match.  Set to the special value \"-\" to match the top level jobs only. (optional)
	excludeGroupPath := "excludeGroupPath_example" // string | specify a group or partial group path to exclude all jobs within that group path. Set to the special value \"-\" to match the top level jobs only. (optional)
	excludeGroupPathExact := "excludeGroupPathExact_example" // string | specify an exact group path to exclude.  Set to the special value \"-\" to match the top level jobs only. (optional)
	jobFilter := "jobFilter_example" // string | specify a filter for the job Name. Include any job name that matches this value (optional)
	excludeJobFilter := "excludeJobFilter_example" // string | specify a filter for the job Name. Exclude any job name that matches this value. (optional)
	jobExactFilter := "jobExactFilter_example" // string | specify an exact job name to match. (optional)
	excludeJobExactFilter := "excludeJobExactFilter_example" // string | specify an exact job name to exclude. (optional)
	startafterFilter := "startafterFilter_example" // string | start after date (optional)
	startbeforeFilter := "startbeforeFilter_example" // string | start before date (optional)
	endafterFilter := "endafterFilter_example" // string | end after date (optional)
	endbeforeFilter := "endbeforeFilter_example" // string | end before date (optional)
	begin := "begin_example" // string | Specify exact date for earliest execution completion time. Format: a unix millisecond timestamp, or a W3C dateTime string in the format \"yyyy-MM-ddTHH:mm:ssZ\". (optional)
	end := "end_example" // string | Specify exact date for latest execution completion time. Format: a unix millisecond timestamp, or a W3C dateTime string in the format \"yyyy-MM-ddTHH:mm:ssZ\". (optional)
	adhoc := true // bool | if true, include only Adhoc executions, if false return only Job executions. By default any matching executions are returned, however if you use any of the Job filters below, then only Job executions will be returned. (optional)
	recentFilter := "recentFilter_example" // string | Use a simple text format to filter executions that completed within a period of time. The format is \"XY\" where X is an integer, and \"Y\" is one of: * `s`: second * `n`: minute * `h`: hour * `d`: day * `w`: week * `m`: month * `y`: year  So a value of `2w` would return executions that completed within the last two weeks.  (optional)
	olderFilter := "olderFilter_example" // string | (same format as `recentFilter`) return executions that completed before the specified relative period of time.  E.g. a value of `30d` returns executions older than 30 days. (optional)
	userFilter := "userFilter_example" // string | Username who started the execution (optional)
	executionTypeFilter := "executionTypeFilter_example" // string | specify the execution type, one of: `scheduled` (schedule trigger), `user` (user trigger), `user-scheduled` (user scheduled trigger). Since: v20 (optional)
	useStats := true // bool | if true, use snapshot-based metrics from SCHEDULED_EXECUTION_STATS table (fast, returns empty metrics (all zeros) if no stats exist). if false or not provided, use execution table query (slow, always returns data). Since: v57 (optional)
	groupByJob := true // bool | if true with useStats=true, returns metrics for all jobs in the project (batch mode). Requires project parameter. Returns format: {jobs: {uuid1: metrics, uuid2: metrics, ...}}. RUN-3768 Phase 5. Since: v57 (optional)
	adhocStringFilter := "adhocStringFilter_example" // string | filter adhoc executions by command title (partial match). (optional)
	nodeFilter := "nodeFilter_example" // string | filter executions by node name or filter expression (partial match). Use 'name:nodename' for simple node name search, or a filter expression like 'tags:value' for complex filters. (optional)
	optionFilter := "optionFilter_example" // string | filter executions by option values (partial match, e.g. '-test 123'). (optional)
	max := int32(56) // int32 | maximum number of results to include in response. (default: 20) (optional)
	offset := int32(56) // int32 | offset for first result to include. (default: 0) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.JobExecutionsAPI.ApiExecutionsQueryv14Docs(context.Background(), project).StatusFilter(statusFilter).AbortedbyFilter(abortedbyFilter).JobIdListFilter(jobIdListFilter).ExcludeJobIdListFilter(excludeJobIdListFilter).JobListFilter(jobListFilter).ExcludeJobListFilter(excludeJobListFilter).GroupPath(groupPath).GroupPathExact(groupPathExact).ExcludeGroupPath(excludeGroupPath).ExcludeGroupPathExact(excludeGroupPathExact).JobFilter(jobFilter).ExcludeJobFilter(excludeJobFilter).JobExactFilter(jobExactFilter).ExcludeJobExactFilter(excludeJobExactFilter).StartafterFilter(startafterFilter).StartbeforeFilter(startbeforeFilter).EndafterFilter(endafterFilter).EndbeforeFilter(endbeforeFilter).Begin(begin).End(end).Adhoc(adhoc).RecentFilter(recentFilter).OlderFilter(olderFilter).UserFilter(userFilter).ExecutionTypeFilter(executionTypeFilter).UseStats(useStats).GroupByJob(groupByJob).AdhocStringFilter(adhocStringFilter).NodeFilter(nodeFilter).OptionFilter(optionFilter).Max(max).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionsQueryv14Docs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionsQueryv14DocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **statusFilter** | **string** | Execution status | 
 **abortedbyFilter** | **string** | Username who aborted an execution | 
 **jobIdListFilter** | **string** | specify a Job ID to include, can be specified multiple times | 
 **excludeJobIdListFilter** | **string** | specify a Job ID to exclude, can be specified multiple times | 
 **jobListFilter** | **string** | specify a full Job group/name to include, can be specified multiple times | 
 **excludeJobListFilter** | **string** | specify a full Job group/name to exclude, can be specified multiple times | 
 **groupPath** | **string** | specify a group or partial group path to include all jobs within that group path. Set to the special value \&quot;-\&quot; to match the top level jobs only. | 
 **groupPathExact** | **string** | specify an exact group path to match.  Set to the special value \&quot;-\&quot; to match the top level jobs only. | 
 **excludeGroupPath** | **string** | specify a group or partial group path to exclude all jobs within that group path. Set to the special value \&quot;-\&quot; to match the top level jobs only. | 
 **excludeGroupPathExact** | **string** | specify an exact group path to exclude.  Set to the special value \&quot;-\&quot; to match the top level jobs only. | 
 **jobFilter** | **string** | specify a filter for the job Name. Include any job name that matches this value | 
 **excludeJobFilter** | **string** | specify a filter for the job Name. Exclude any job name that matches this value. | 
 **jobExactFilter** | **string** | specify an exact job name to match. | 
 **excludeJobExactFilter** | **string** | specify an exact job name to exclude. | 
 **startafterFilter** | **string** | start after date | 
 **startbeforeFilter** | **string** | start before date | 
 **endafterFilter** | **string** | end after date | 
 **endbeforeFilter** | **string** | end before date | 
 **begin** | **string** | Specify exact date for earliest execution completion time. Format: a unix millisecond timestamp, or a W3C dateTime string in the format \&quot;yyyy-MM-ddTHH:mm:ssZ\&quot;. | 
 **end** | **string** | Specify exact date for latest execution completion time. Format: a unix millisecond timestamp, or a W3C dateTime string in the format \&quot;yyyy-MM-ddTHH:mm:ssZ\&quot;. | 
 **adhoc** | **bool** | if true, include only Adhoc executions, if false return only Job executions. By default any matching executions are returned, however if you use any of the Job filters below, then only Job executions will be returned. | 
 **recentFilter** | **string** | Use a simple text format to filter executions that completed within a period of time. The format is \&quot;XY\&quot; where X is an integer, and \&quot;Y\&quot; is one of: * &#x60;s&#x60;: second * &#x60;n&#x60;: minute * &#x60;h&#x60;: hour * &#x60;d&#x60;: day * &#x60;w&#x60;: week * &#x60;m&#x60;: month * &#x60;y&#x60;: year  So a value of &#x60;2w&#x60; would return executions that completed within the last two weeks.  | 
 **olderFilter** | **string** | (same format as &#x60;recentFilter&#x60;) return executions that completed before the specified relative period of time.  E.g. a value of &#x60;30d&#x60; returns executions older than 30 days. | 
 **userFilter** | **string** | Username who started the execution | 
 **executionTypeFilter** | **string** | specify the execution type, one of: &#x60;scheduled&#x60; (schedule trigger), &#x60;user&#x60; (user trigger), &#x60;user-scheduled&#x60; (user scheduled trigger). Since: v20 | 
 **useStats** | **bool** | if true, use snapshot-based metrics from SCHEDULED_EXECUTION_STATS table (fast, returns empty metrics (all zeros) if no stats exist). if false or not provided, use execution table query (slow, always returns data). Since: v57 | 
 **groupByJob** | **bool** | if true with useStats&#x3D;true, returns metrics for all jobs in the project (batch mode). Requires project parameter. Returns format: {jobs: {uuid1: metrics, uuid2: metrics, ...}}. RUN-3768 Phase 5. Since: v57 | 
 **adhocStringFilter** | **string** | filter adhoc executions by command title (partial match). | 
 **nodeFilter** | **string** | filter executions by node name or filter expression (partial match). Use &#39;name:nodename&#39; for simple node name search, or a filter expression like &#39;tags:value&#39; for complex filters. | 
 **optionFilter** | **string** | filter executions by option values (partial match, e.g. &#39;-test 123&#39;). | 
 **max** | **int32** | maximum number of results to include in response. (default: 20) | 
 **offset** | **int32** | offset for first result to include. (default: 0) | 

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


## ApiExecutionsRunningv14

> map[string]interface{} ApiExecutionsRunningv14(ctx, project).Max(max).Offset(offset).JobIdFilter(jobIdFilter).IncludePostponed(includePostponed).Execute()

Listing Running Executions



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
	project := "project_example" // string | Project Name, or * for all projects
	max := int32(56) // int32 | Paging maximum results, default: 20 (optional)
	offset := int32(56) // int32 | Paging Offset (optional)
	jobIdFilter := "jobIdFilter_example" // string | Specifies a Job ID, the results will only contain running executions for the given job. Since: v32 (optional)
	includePostponed := true // bool | If true, include scheduled and queued executions. Since: v32 (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobExecutionsAPI.ApiExecutionsRunningv14(context.Background(), project).Max(max).Offset(offset).JobIdFilter(jobIdFilter).IncludePostponed(includePostponed).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiExecutionsRunningv14``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiExecutionsRunningv14`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiExecutionsRunningv14`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name, or * for all projects | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiExecutionsRunningv14Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **max** | **int32** | Paging maximum results, default: 20 | 
 **offset** | **int32** | Paging Offset | 
 **jobIdFilter** | **string** | Specifies a Job ID, the results will only contain running executions for the given job. Since: v32 | 
 **includePostponed** | **bool** | If true, include scheduled and queued executions. Since: v32 | 

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


## ApiHomeSummary

> HomeSummary ApiHomeSummary(ctx).Execute()

Summary of executions and projects



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
	resp, r, err := apiClient.JobExecutionsAPI.ApiHomeSummary(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobExecutionsAPI.ApiHomeSummary``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiHomeSummary`: HomeSummary
	fmt.Fprintf(os.Stdout, "Response from `JobExecutionsAPI.ApiHomeSummary`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiHomeSummaryRequest struct via the builder pattern


### Return type

[**HomeSummary**](HomeSummary.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


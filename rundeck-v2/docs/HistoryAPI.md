# \HistoryAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiHistoryv14**](HistoryAPI.md#ApiHistoryv14) | **Get** /project/{project}/history | Listing History



## ApiHistoryv14

> map[string]interface{} ApiHistoryv14(ctx, project).JobIdFilter(jobIdFilter).ReportIdFilter(reportIdFilter).UserFilter(userFilter).StatFilter(statFilter).JobListFilter(jobListFilter).ExcludeJobListFilter(excludeJobListFilter).RecentFilter(recentFilter).Begin(begin).End(end).Max(max).Offset(offset).Execute()

Listing History



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
	jobIdFilter := "jobIdFilter_example" // string | include events for a job ID. (optional)
	reportIdFilter := "reportIdFilter_example" // string | include events for a event Name. (optional)
	userFilter := "userFilter_example" // string | include events created by a user. (optional)
	statFilter := "statFilter_example" // string | include events based on result status.  this can be 'succeed','fail', or 'cancel'. (optional)
	jobListFilter := []string{"Inner_example"} // []string | include events for the job by name, format: 'group/name'.  To use multiple values, include this parameter multiple times. (optional)
	excludeJobListFilter := []string{"Inner_example"} // []string | exclude events for the job by name, format: 'group/name'. To use multiple values, include this parameter multiple times. (optional)
	recentFilter := "recentFilter_example" // string | Use a simple text format to filter events that occurred within a period of time. The format is \"XY\" where X is an integer, and \"Y\" is one of:         * `h`: hour         * `d`: day         * `w`: week         * `m`: month         * `y`: year         So a value of \"2w\" would return events within the last two weeks. (optional)
	begin := "begin_example" // string | Specify exact date for earliest result. a unix millisecond timestamp, or a W3C dateTime string in the format \"yyyy-MM-ddTHH:mm:ssZ\" (optional)
	end := "end_example" // string | Specify exact date for latest result. a unix millisecond timestamp, or a W3C dateTime string in the format \"yyyy-MM-ddTHH:mm:ssZ\" (optional)
	max := int32(56) // int32 | indicate the maximum number of events to return. The default maximum to return is 20 (optional)
	offset := int32(56) // int32 | indicate the 0-indexed offset for the first event to return (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.HistoryAPI.ApiHistoryv14(context.Background(), project).JobIdFilter(jobIdFilter).ReportIdFilter(reportIdFilter).UserFilter(userFilter).StatFilter(statFilter).JobListFilter(jobListFilter).ExcludeJobListFilter(excludeJobListFilter).RecentFilter(recentFilter).Begin(begin).End(end).Max(max).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HistoryAPI.ApiHistoryv14``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiHistoryv14`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `HistoryAPI.ApiHistoryv14`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiHistoryv14Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **jobIdFilter** | **string** | include events for a job ID. | 
 **reportIdFilter** | **string** | include events for a event Name. | 
 **userFilter** | **string** | include events created by a user. | 
 **statFilter** | **string** | include events based on result status.  this can be &#39;succeed&#39;,&#39;fail&#39;, or &#39;cancel&#39;. | 
 **jobListFilter** | **[]string** | include events for the job by name, format: &#39;group/name&#39;.  To use multiple values, include this parameter multiple times. | 
 **excludeJobListFilter** | **[]string** | exclude events for the job by name, format: &#39;group/name&#39;. To use multiple values, include this parameter multiple times. | 
 **recentFilter** | **string** | Use a simple text format to filter events that occurred within a period of time. The format is \&quot;XY\&quot; where X is an integer, and \&quot;Y\&quot; is one of:         * &#x60;h&#x60;: hour         * &#x60;d&#x60;: day         * &#x60;w&#x60;: week         * &#x60;m&#x60;: month         * &#x60;y&#x60;: year         So a value of \&quot;2w\&quot; would return events within the last two weeks. | 
 **begin** | **string** | Specify exact date for earliest result. a unix millisecond timestamp, or a W3C dateTime string in the format \&quot;yyyy-MM-ddTHH:mm:ssZ\&quot; | 
 **end** | **string** | Specify exact date for latest result. a unix millisecond timestamp, or a W3C dateTime string in the format \&quot;yyyy-MM-ddTHH:mm:ssZ\&quot; | 
 **max** | **int32** | indicate the maximum number of events to return. The default maximum to return is 20 | 
 **offset** | **int32** | indicate the 0-indexed offset for the first event to return | 

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


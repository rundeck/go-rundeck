# \CalendarsAPI

All URIs are relative to *https://localhost:4440/api/59*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiDeleteProjectCalendar**](CalendarsAPI.md#ApiDeleteProjectCalendar) | **Delete** /project/{project}/calendars/{id} | Delete Project Calendar [Enterprise]
[**ApiDeleteSystemCalendar**](CalendarsAPI.md#ApiDeleteSystemCalendar) | **Delete** /system/calendars/{id} | Delete System Calendar [Enterprise]
[**ApiLoadProjectCalendars**](CalendarsAPI.md#ApiLoadProjectCalendars) | **Post** /project/{project}/calendars | Create/Update Project Calendar [Enterprise]
[**ApiLoadSystemCalendars**](CalendarsAPI.md#ApiLoadSystemCalendars) | **Post** /system/calendars | Create/Update System Calendar [Enterprise]
[**ApiProjectCalendars**](CalendarsAPI.md#ApiProjectCalendars) | **Get** /project/{project}/calendars | List Project Calendars [Enterprise]
[**ApiSystemCalendars**](CalendarsAPI.md#ApiSystemCalendars) | **Get** /system/calendars | List System Calendars [Enterprise]



## ApiDeleteProjectCalendar

> ApiDeleteProjectCalendar(ctx, project, id).Execute()

Delete Project Calendar [Enterprise]



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
	id := "id_example" // string | Calendar Id to be deleted

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CalendarsAPI.ApiDeleteProjectCalendar(context.Background(), project, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CalendarsAPI.ApiDeleteProjectCalendar``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**id** | **string** | Calendar Id to be deleted | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiDeleteProjectCalendarRequest struct via the builder pattern


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


## ApiDeleteSystemCalendar

> ApiDeleteSystemCalendar(ctx, id).Execute()

Delete System Calendar [Enterprise]



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
	id := "id_example" // string | Calendar Id to be deleted

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CalendarsAPI.ApiDeleteSystemCalendar(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CalendarsAPI.ApiDeleteSystemCalendar``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Calendar Id to be deleted | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiDeleteSystemCalendarRequest struct via the builder pattern


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


## ApiLoadProjectCalendars

> ProjectCalendarsResponse ApiLoadProjectCalendars(ctx, project).Body(body).Execute()

Create/Update Project Calendar [Enterprise]



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
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CalendarsAPI.ApiLoadProjectCalendars(context.Background(), project).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CalendarsAPI.ApiLoadProjectCalendars``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiLoadProjectCalendars`: ProjectCalendarsResponse
	fmt.Fprintf(os.Stdout, "Response from `CalendarsAPI.ApiLoadProjectCalendars`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiLoadProjectCalendarsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | **map[string]interface{}** |  | 

### Return type

[**ProjectCalendarsResponse**](ProjectCalendarsResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiLoadSystemCalendars

> ProjectCalendarsResponse ApiLoadSystemCalendars(ctx).Body(body).Execute()

Create/Update System Calendar [Enterprise]



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
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CalendarsAPI.ApiLoadSystemCalendars(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CalendarsAPI.ApiLoadSystemCalendars``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiLoadSystemCalendars`: ProjectCalendarsResponse
	fmt.Fprintf(os.Stdout, "Response from `CalendarsAPI.ApiLoadSystemCalendars`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiLoadSystemCalendarsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **map[string]interface{}** |  | 

### Return type

[**ProjectCalendarsResponse**](ProjectCalendarsResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectCalendars

> []map[string]interface{} ApiProjectCalendars(ctx, project).Execute()

List Project Calendars [Enterprise]



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
	resp, r, err := apiClient.CalendarsAPI.ApiProjectCalendars(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CalendarsAPI.ApiProjectCalendars``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectCalendars`: []map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `CalendarsAPI.ApiProjectCalendars`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectCalendarsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


## ApiSystemCalendars

> []map[string]interface{} ApiSystemCalendars(ctx).Execute()

List System Calendars [Enterprise]



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
	resp, r, err := apiClient.CalendarsAPI.ApiSystemCalendars(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CalendarsAPI.ApiSystemCalendars``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSystemCalendars`: []map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `CalendarsAPI.ApiSystemCalendars`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiSystemCalendarsRequest struct via the builder pattern


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


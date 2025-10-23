# \AuthorizationAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AppContextAuthorizationsForResourceKind**](AuthorizationAPI.md#AppContextAuthorizationsForResourceKind) | **Get** /authorizations/application/{kind} | Check authorization for application resource kind
[**AppContextAuthorizationsForTypeWithSpecifier**](AuthorizationAPI.md#AppContextAuthorizationsForTypeWithSpecifier) | **Get** /authorizations/application/{type}/{specifier} | Get authorizations for an application type with specifier
[**ProjectContextAuthorizationsForJob**](AuthorizationAPI.md#ProjectContextAuthorizationsForJob) | **Get** /authorizations/project/{project}/job/{specifier} | Get authorizations for a job
[**ProjectContextAuthorizationsForResourceKind**](AuthorizationAPI.md#ProjectContextAuthorizationsForResourceKind) | **Get** /authorizations/project/{project}/{kind} | Get authorizations for a project resource kind
[**ProjectContextAuthorizationsForTypeWithSpecifier**](AuthorizationAPI.md#ProjectContextAuthorizationsForTypeWithSpecifier) | **Get** /authorizations/project/{project}/{type}/{specifier} | Get authorizations for a type with specifier



## AppContextAuthorizationsForResourceKind

> AuthorizationsResponse AppContextAuthorizationsForResourceKind(ctx, kind).Actions(actions).Execute()

Check authorization for application resource kind



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
	kind := "kind_example" // string | Resource Kind
	actions := []string{"Inner_example"} // []string | Actions to check authorization for

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthorizationAPI.AppContextAuthorizationsForResourceKind(context.Background(), kind).Actions(actions).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthorizationAPI.AppContextAuthorizationsForResourceKind``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AppContextAuthorizationsForResourceKind`: AuthorizationsResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthorizationAPI.AppContextAuthorizationsForResourceKind`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**kind** | **string** | Resource Kind | 

### Other Parameters

Other parameters are passed through a pointer to a apiAppContextAuthorizationsForResourceKindRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **actions** | **[]string** | Actions to check authorization for | 

### Return type

[**AuthorizationsResponse**](AuthorizationsResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AppContextAuthorizationsForTypeWithSpecifier

> AuthorizationsResponse AppContextAuthorizationsForTypeWithSpecifier(ctx, type_, specifier).Actions(actions).Execute()

Get authorizations for an application type with specifier



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
	type_ := "type__example" // string | Resource Type
	specifier := "specifier_example" // string | Resource specifier
	actions := []string{"Inner_example"} // []string | Actions to check authorization for

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthorizationAPI.AppContextAuthorizationsForTypeWithSpecifier(context.Background(), type_, specifier).Actions(actions).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthorizationAPI.AppContextAuthorizationsForTypeWithSpecifier``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AppContextAuthorizationsForTypeWithSpecifier`: AuthorizationsResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthorizationAPI.AppContextAuthorizationsForTypeWithSpecifier`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** | Resource Type | 
**specifier** | **string** | Resource specifier | 

### Other Parameters

Other parameters are passed through a pointer to a apiAppContextAuthorizationsForTypeWithSpecifierRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **actions** | **[]string** | Actions to check authorization for | 

### Return type

[**AuthorizationsResponse**](AuthorizationsResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ProjectContextAuthorizationsForJob

> AuthorizationsResponse ProjectContextAuthorizationsForJob(ctx, project, specifier).Actions(actions).Execute()

Get authorizations for a job



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
	specifier := "specifier_example" // string | Job Id
	actions := []string{"Inner_example"} // []string | Actions to check authorization for

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthorizationAPI.ProjectContextAuthorizationsForJob(context.Background(), project, specifier).Actions(actions).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthorizationAPI.ProjectContextAuthorizationsForJob``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ProjectContextAuthorizationsForJob`: AuthorizationsResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthorizationAPI.ProjectContextAuthorizationsForJob`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**specifier** | **string** | Job Id | 

### Other Parameters

Other parameters are passed through a pointer to a apiProjectContextAuthorizationsForJobRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **actions** | **[]string** | Actions to check authorization for | 

### Return type

[**AuthorizationsResponse**](AuthorizationsResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ProjectContextAuthorizationsForResourceKind

> AuthorizationsResponse ProjectContextAuthorizationsForResourceKind(ctx, project, kind).Actions(actions).Execute()

Get authorizations for a project resource kind



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
	kind := "kind_example" // string | Resource Kind
	actions := []string{"Inner_example"} // []string | Actions to check authorization for

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthorizationAPI.ProjectContextAuthorizationsForResourceKind(context.Background(), project, kind).Actions(actions).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthorizationAPI.ProjectContextAuthorizationsForResourceKind``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ProjectContextAuthorizationsForResourceKind`: AuthorizationsResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthorizationAPI.ProjectContextAuthorizationsForResourceKind`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**kind** | **string** | Resource Kind | 

### Other Parameters

Other parameters are passed through a pointer to a apiProjectContextAuthorizationsForResourceKindRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **actions** | **[]string** | Actions to check authorization for | 

### Return type

[**AuthorizationsResponse**](AuthorizationsResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ProjectContextAuthorizationsForTypeWithSpecifier

> AuthorizationsResponse ProjectContextAuthorizationsForTypeWithSpecifier(ctx, project, type_, specifier).Actions(actions).Execute()

Get authorizations for a type with specifier



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
	type_ := "type__example" // string | Resource Type
	specifier := "specifier_example" // string | Resource specifier
	actions := []string{"Inner_example"} // []string | Actions to check authorization for

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthorizationAPI.ProjectContextAuthorizationsForTypeWithSpecifier(context.Background(), project, type_, specifier).Actions(actions).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthorizationAPI.ProjectContextAuthorizationsForTypeWithSpecifier``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ProjectContextAuthorizationsForTypeWithSpecifier`: AuthorizationsResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthorizationAPI.ProjectContextAuthorizationsForTypeWithSpecifier`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**type_** | **string** | Resource Type | 
**specifier** | **string** | Resource specifier | 

### Other Parameters

Other parameters are passed through a pointer to a apiProjectContextAuthorizationsForTypeWithSpecifierRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **actions** | **[]string** | Actions to check authorization for | 

### Return type

[**AuthorizationsResponse**](AuthorizationsResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


# \UserClassAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetEnabled**](UserClassAPI.md#GetEnabled) | **Get** /userclass/enabled | User Class Feature enablement check
[**GetUserClass**](UserClassAPI.md#GetUserClass) | **Get** /userclass/user/{username} | Get a user&#39;s User Class assignment
[**GetUserClassAllocations**](UserClassAPI.md#GetUserClassAllocations) | **Get** /userclass/allocations | Get allocated User Classes
[**GetUserClassAllocationsState**](UserClassAPI.md#GetUserClassAllocationsState) | **Get** /userclass/state | Get allocated User Class State
[**GetUserClassSelf**](UserClassAPI.md#GetUserClassSelf) | **Get** /userclass/self | Get current user&#39;s User Class assignment
[**GetUserClassesAvailable**](UserClassAPI.md#GetUserClassesAvailable) | **Get** /userclass/available | Get available User Classes
[**RemoveUserClass**](UserClassAPI.md#RemoveUserClass) | **Delete** /userclass/user/{username} | Delete a user&#39;s User Class assignment
[**SetUserClass**](UserClassAPI.md#SetUserClass) | **Post** /userclass/user/{username} | Set a user&#39;s User Class assignment
[**StoreUserClasses**](UserClassAPI.md#StoreUserClasses) | **Post** /userclass/update | Update multiple user class assignments



## GetEnabled

> EnabledResponse GetEnabled(ctx).Execute()

User Class Feature enablement check



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
	resp, r, err := apiClient.UserClassAPI.GetEnabled(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserClassAPI.GetEnabled``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEnabled`: EnabledResponse
	fmt.Fprintf(os.Stdout, "Response from `UserClassAPI.GetEnabled`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetEnabledRequest struct via the builder pattern


### Return type

[**EnabledResponse**](EnabledResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUserClass

> UserClassResponse GetUserClass(ctx, username).Execute()

Get a user's User Class assignment



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
	username := "username_example" // string | User Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UserClassAPI.GetUserClass(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserClassAPI.GetUserClass``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUserClass`: UserClassResponse
	fmt.Fprintf(os.Stdout, "Response from `UserClassAPI.GetUserClass`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** | User Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserClassRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**UserClassResponse**](UserClassResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUserClassAllocations

> UserClassAllocationResponse GetUserClassAllocations(ctx).Execute()

Get allocated User Classes



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
	resp, r, err := apiClient.UserClassAPI.GetUserClassAllocations(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserClassAPI.GetUserClassAllocations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUserClassAllocations`: UserClassAllocationResponse
	fmt.Fprintf(os.Stdout, "Response from `UserClassAPI.GetUserClassAllocations`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserClassAllocationsRequest struct via the builder pattern


### Return type

[**UserClassAllocationResponse**](UserClassAllocationResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUserClassAllocationsState

> UserClassAllocationResponse GetUserClassAllocationsState(ctx).Execute()

Get allocated User Class State



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
	resp, r, err := apiClient.UserClassAPI.GetUserClassAllocationsState(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserClassAPI.GetUserClassAllocationsState``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUserClassAllocationsState`: UserClassAllocationResponse
	fmt.Fprintf(os.Stdout, "Response from `UserClassAPI.GetUserClassAllocationsState`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserClassAllocationsStateRequest struct via the builder pattern


### Return type

[**UserClassAllocationResponse**](UserClassAllocationResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUserClassSelf

> UserClassResponse GetUserClassSelf(ctx).Execute()

Get current user's User Class assignment



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
	resp, r, err := apiClient.UserClassAPI.GetUserClassSelf(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserClassAPI.GetUserClassSelf``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUserClassSelf`: UserClassResponse
	fmt.Fprintf(os.Stdout, "Response from `UserClassAPI.GetUserClassSelf`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserClassSelfRequest struct via the builder pattern


### Return type

[**UserClassResponse**](UserClassResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUserClassesAvailable

> UserClassList GetUserClassesAvailable(ctx).Execute()

Get available User Classes



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
	resp, r, err := apiClient.UserClassAPI.GetUserClassesAvailable(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserClassAPI.GetUserClassesAvailable``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUserClassesAvailable`: UserClassList
	fmt.Fprintf(os.Stdout, "Response from `UserClassAPI.GetUserClassesAvailable`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserClassesAvailableRequest struct via the builder pattern


### Return type

[**UserClassList**](UserClassList.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveUserClass

> RemoveUserClass(ctx, username).Execute()

Delete a user's User Class assignment



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
	username := "username_example" // string | User Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.UserClassAPI.RemoveUserClass(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserClassAPI.RemoveUserClass``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** | User Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveUserClassRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SetUserClass

> UserClassResponse SetUserClass(ctx, username).SetUserclassModel(setUserclassModel).Execute()

Set a user's User Class assignment



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
	username := "username_example" // string | User Name
	setUserclassModel := *openapiclient.NewSetUserclassModel() // SetUserclassModel |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UserClassAPI.SetUserClass(context.Background(), username).SetUserclassModel(setUserclassModel).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserClassAPI.SetUserClass``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SetUserClass`: UserClassResponse
	fmt.Fprintf(os.Stdout, "Response from `UserClassAPI.SetUserClass`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** | User Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetUserClassRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **setUserclassModel** | [**SetUserclassModel**](SetUserclassModel.md) |  | 

### Return type

[**UserClassResponse**](UserClassResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StoreUserClasses

> UserClassAllocationResponse StoreUserClasses(ctx).UserClassAllocationChange(userClassAllocationChange).Execute()

Update multiple user class assignments



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
	userClassAllocationChange := *openapiclient.NewUserClassAllocationChange() // UserClassAllocationChange |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UserClassAPI.StoreUserClasses(context.Background()).UserClassAllocationChange(userClassAllocationChange).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserClassAPI.StoreUserClasses``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StoreUserClasses`: UserClassAllocationResponse
	fmt.Fprintf(os.Stdout, "Response from `UserClassAPI.StoreUserClasses`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiStoreUserClassesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userClassAllocationChange** | [**UserClassAllocationChange**](UserClassAllocationChange.md) |  | 

### Return type

[**UserClassAllocationResponse**](UserClassAllocationResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


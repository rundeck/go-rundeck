# \ToursAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiGetProjectResource**](ToursAPI.md#ApiGetProjectResource) | **Get** /project/{project}/tours/resource/{path} | Get Project Tour Resource [Enterprise]
[**ApiGetSystemResource**](ToursAPI.md#ApiGetSystemResource) | **Get** /system/tours/resource/{path} | Get System Tour Resource [Enterprise]
[**ApiProjectImportTour**](ToursAPI.md#ApiProjectImportTour) | **Post** /project/{project}/tour/import/{tourFolder}/{manifestFileName} | Import Tours Archive for a Project [Enterprise]
[**ApiProjectList**](ToursAPI.md#ApiProjectList) | **Get** /project/{project}/tours | Get Project Tours [Enterprise]
[**ApiProjectLoadResource**](ToursAPI.md#ApiProjectLoadResource) | **Post** /project/{project}/tours/{path} | Upload Project Tour Resource [Enterprise]
[**ApiRundeckEndpoints**](ToursAPI.md#ApiRundeckEndpoints) | **Get** /tours/endpoints | Get Tour Endpoints List [Enterprise]
[**ApiSystemImportTour**](ToursAPI.md#ApiSystemImportTour) | **Post** /system/tour/import/{tourFolder}/{manifestFileName} | Import Tours Archive for System [Enterprise]
[**ApiSystemList**](ToursAPI.md#ApiSystemList) | **Get** /system/tours | Get System Tours [Enterprise]
[**ApiSystemLoadResource**](ToursAPI.md#ApiSystemLoadResource) | **Post** /system/tours/{path} | Upload System Tour Resource [Enterprise]



## ApiGetProjectResource

> Tour ApiGetProjectResource(ctx, project, path).Execute()

Get Project Tour Resource [Enterprise]



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
	path := "path_example" // string | Resource Path

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ToursAPI.ApiGetProjectResource(context.Background(), project, path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ToursAPI.ApiGetProjectResource``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiGetProjectResource`: Tour
	fmt.Fprintf(os.Stdout, "Response from `ToursAPI.ApiGetProjectResource`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**path** | **string** | Resource Path | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiGetProjectResourceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**Tour**](Tour.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiGetSystemResource

> Tour ApiGetSystemResource(ctx, path).Execute()

Get System Tour Resource [Enterprise]



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
	path := "path_example" // string | Resource Path

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ToursAPI.ApiGetSystemResource(context.Background(), path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ToursAPI.ApiGetSystemResource``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiGetSystemResource`: Tour
	fmt.Fprintf(os.Stdout, "Response from `ToursAPI.ApiGetSystemResource`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Resource Path | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiGetSystemResourceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Tour**](Tour.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectImportTour

> TourManagerSuccessResponse ApiProjectImportTour(ctx, project, tourFolder, manifestFileName).Body(body).Execute()

Import Tours Archive for a Project [Enterprise]



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
	tourFolder := "tourFolder_example" // string | Tour Folder Name: the name of the zip content folder containing tour.json files.
	manifestFileName := "manifestFileName_example" // string | Manifest File Name: the name of the manifest.json file within the archive
	body := map[string]interface{}{ ... } // map[string]interface{} | Zip archive of Tours (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ToursAPI.ApiProjectImportTour(context.Background(), project, tourFolder, manifestFileName).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ToursAPI.ApiProjectImportTour``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectImportTour`: TourManagerSuccessResponse
	fmt.Fprintf(os.Stdout, "Response from `ToursAPI.ApiProjectImportTour`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**tourFolder** | **string** | Tour Folder Name: the name of the zip content folder containing tour.json files. | 
**manifestFileName** | **string** | Manifest File Name: the name of the manifest.json file within the archive | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectImportTourRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | **map[string]interface{}** | Zip archive of Tours | 

### Return type

[**TourManagerSuccessResponse**](TourManagerSuccessResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/zip
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectList

> Manifest ApiProjectList(ctx, project).Execute()

Get Project Tours [Enterprise]



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
	resp, r, err := apiClient.ToursAPI.ApiProjectList(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ToursAPI.ApiProjectList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectList`: Manifest
	fmt.Fprintf(os.Stdout, "Response from `ToursAPI.ApiProjectList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Manifest**](Manifest.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectLoadResource

> TourManagerSuccessResponse ApiProjectLoadResource(ctx, project, path).ApiProjectLoadResourceRequest(apiProjectLoadResourceRequest).Execute()

Upload Project Tour Resource [Enterprise]



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
	path := "path_example" // string | Resource Path
	apiProjectLoadResourceRequest := openapiclient.apiProjectLoadResource_request{Manifest: openapiclient.NewManifest()} // ApiProjectLoadResourceRequest | Manifest or Tour definition (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ToursAPI.ApiProjectLoadResource(context.Background(), project, path).ApiProjectLoadResourceRequest(apiProjectLoadResourceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ToursAPI.ApiProjectLoadResource``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectLoadResource`: TourManagerSuccessResponse
	fmt.Fprintf(os.Stdout, "Response from `ToursAPI.ApiProjectLoadResource`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**path** | **string** | Resource Path | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectLoadResourceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiProjectLoadResourceRequest** | [**ApiProjectLoadResourceRequest**](ApiProjectLoadResourceRequest.md) | Manifest or Tour definition | 

### Return type

[**TourManagerSuccessResponse**](TourManagerSuccessResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiRundeckEndpoints

> []string ApiRundeckEndpoints(ctx).Execute()

Get Tour Endpoints List [Enterprise]



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
	resp, r, err := apiClient.ToursAPI.ApiRundeckEndpoints(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ToursAPI.ApiRundeckEndpoints``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiRundeckEndpoints`: []string
	fmt.Fprintf(os.Stdout, "Response from `ToursAPI.ApiRundeckEndpoints`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiRundeckEndpointsRequest struct via the builder pattern


### Return type

**[]string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSystemImportTour

> TourManagerSuccessResponse ApiSystemImportTour(ctx, tourFolder, manifestFileName).Body(body).Execute()

Import Tours Archive for System [Enterprise]



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
	tourFolder := "tourFolder_example" // string | Tour Folder Name: the name of the zip content folder containing tour.json files.
	manifestFileName := "manifestFileName_example" // string | Manifest File Name: the name of the manifest.json file within the archive
	body := map[string]interface{}{ ... } // map[string]interface{} | Zip archive of Tours (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ToursAPI.ApiSystemImportTour(context.Background(), tourFolder, manifestFileName).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ToursAPI.ApiSystemImportTour``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSystemImportTour`: TourManagerSuccessResponse
	fmt.Fprintf(os.Stdout, "Response from `ToursAPI.ApiSystemImportTour`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tourFolder** | **string** | Tour Folder Name: the name of the zip content folder containing tour.json files. | 
**manifestFileName** | **string** | Manifest File Name: the name of the manifest.json file within the archive | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSystemImportTourRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | **map[string]interface{}** | Zip archive of Tours | 

### Return type

[**TourManagerSuccessResponse**](TourManagerSuccessResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/zip
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSystemList

> Manifest ApiSystemList(ctx).Execute()

Get System Tours [Enterprise]



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
	resp, r, err := apiClient.ToursAPI.ApiSystemList(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ToursAPI.ApiSystemList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSystemList`: Manifest
	fmt.Fprintf(os.Stdout, "Response from `ToursAPI.ApiSystemList`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiSystemListRequest struct via the builder pattern


### Return type

[**Manifest**](Manifest.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSystemLoadResource

> TourManagerSuccessResponse ApiSystemLoadResource(ctx, path).ApiProjectLoadResourceRequest(apiProjectLoadResourceRequest).Execute()

Upload System Tour Resource [Enterprise]



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
	path := "path_example" // string | Resource Path
	apiProjectLoadResourceRequest := openapiclient.apiProjectLoadResource_request{Manifest: openapiclient.NewManifest()} // ApiProjectLoadResourceRequest | Manifest or Tour definition (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ToursAPI.ApiSystemLoadResource(context.Background(), path).ApiProjectLoadResourceRequest(apiProjectLoadResourceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ToursAPI.ApiSystemLoadResource``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSystemLoadResource`: TourManagerSuccessResponse
	fmt.Fprintf(os.Stdout, "Response from `ToursAPI.ApiSystemLoadResource`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Resource Path | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSystemLoadResourceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiProjectLoadResourceRequest** | [**ApiProjectLoadResourceRequest**](ApiProjectLoadResourceRequest.md) | Manifest or Tour definition | 

### Return type

[**TourManagerSuccessResponse**](TourManagerSuccessResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


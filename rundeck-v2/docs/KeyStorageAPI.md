# \KeyStorageAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiDeleteResource**](KeyStorageAPI.md#ApiDeleteResource) | **Delete** /storage/keys/{path} | Delete A Key
[**ApiGetResource**](KeyStorageAPI.md#ApiGetResource) | **Get** /storage/keys/{path} | List and Get Keys and Key Metadata
[**ApiPostResource**](KeyStorageAPI.md#ApiPostResource) | **Post** /storage/keys/{path} | Create Keys
[**ApiPutResource**](KeyStorageAPI.md#ApiPutResource) | **Put** /storage/keys/{path} | Modify A Key



## ApiDeleteResource

> map[string]interface{} ApiDeleteResource(ctx, path).Execute()

Delete A Key



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
	path := "path_example" // string | Path and Key file name. Can be a directory path such as `subdir/` or include a filename `subdir/file.password`

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.KeyStorageAPI.ApiDeleteResource(context.Background(), path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeyStorageAPI.ApiDeleteResource``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiDeleteResource`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `KeyStorageAPI.ApiDeleteResource`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Path and Key file name. Can be a directory path such as &#x60;subdir/&#x60; or include a filename &#x60;subdir/file.password&#x60; | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiDeleteResourceRequest struct via the builder pattern


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


## ApiGetResource

> map[string]interface{} ApiGetResource(ctx, path).Execute()

List and Get Keys and Key Metadata



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
	path := "path_example" // string | Path and Key file name. Can be a directory path such as `subdir/` or include a filename `subdir/file.password`

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.KeyStorageAPI.ApiGetResource(context.Background(), path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeyStorageAPI.ApiGetResource``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiGetResource`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `KeyStorageAPI.ApiGetResource`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Path and Key file name. Can be a directory path such as &#x60;subdir/&#x60; or include a filename &#x60;subdir/file.password&#x60; | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiGetResourceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/pgp-keys

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiPostResource

> map[string]interface{} ApiPostResource(ctx, path).Body(body).Execute()

Create Keys



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
	path := "path_example" // string | Path and Key file name. Can be a directory path such as `subdir/` or include a filename `subdir/file.password`
	body := "...private key..." // string | Private key, public key, or password content

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.KeyStorageAPI.ApiPostResource(context.Background(), path).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeyStorageAPI.ApiPostResource``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiPostResource`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `KeyStorageAPI.ApiPostResource`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Path and Key file name. Can be a directory path such as &#x60;subdir/&#x60; or include a filename &#x60;subdir/file.password&#x60; | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiPostResourceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | **string** | Private key, public key, or password content | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/octet-stream, application/pgp-keys, application/x-rundeck-data-password
- **Accept**: application/json, application/pgp-keys

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiPutResource

> map[string]interface{} ApiPutResource(ctx, path).Body(body).Execute()

Modify A Key



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
	path := "path_example" // string | Path and Key file name. Can be a directory path such as `subdir/` or include a filename `subdir/file.password`
	body := "...private key..." // string | Private key, public key, or password content

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.KeyStorageAPI.ApiPutResource(context.Background(), path).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeyStorageAPI.ApiPutResource``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiPutResource`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `KeyStorageAPI.ApiPutResource`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Path and Key file name. Can be a directory path such as &#x60;subdir/&#x60; or include a filename &#x60;subdir/file.password&#x60; | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiPutResourceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | **string** | Private key, public key, or password content | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/octet-stream, application/pgp-keys, application/x-rundeck-data-password
- **Accept**: application/json, application/pgp-keys

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


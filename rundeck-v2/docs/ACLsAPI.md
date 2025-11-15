# \ACLsAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiSystemAcls**](ACLsAPI.md#ApiSystemAcls) | **Get** /system/acl/{path} | Get an ACL Policy.
[**ApiSystemAclsDELETEDocs**](ACLsAPI.md#ApiSystemAclsDELETEDocs) | **Delete** /system/acl/{path} | Delete an ACL Policy.
[**ApiSystemAclsPOSTDocs**](ACLsAPI.md#ApiSystemAclsPOSTDocs) | **Post** /system/acl/{path} | Create an ACL Policy.
[**ApiSystemAclsPUTDocs**](ACLsAPI.md#ApiSystemAclsPUTDocs) | **Put** /system/acl/{path} | Update an ACL Policy.



## ApiSystemAcls

> ApiSystemAcls(ctx, path).Execute()

Get an ACL Policy.



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
	path := "path_example" // string | Path to the Acl policy file

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ACLsAPI.ApiSystemAcls(context.Background(), path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLsAPI.ApiSystemAcls``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Path to the Acl policy file | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSystemAclsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain, application/yaml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSystemAclsDELETEDocs

> map[string]interface{} ApiSystemAclsDELETEDocs(ctx, path).Execute()

Delete an ACL Policy.



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
	path := "path_example" // string | Path to the Acl policy file

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ACLsAPI.ApiSystemAclsDELETEDocs(context.Background(), path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLsAPI.ApiSystemAclsDELETEDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSystemAclsDELETEDocs`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ACLsAPI.ApiSystemAclsDELETEDocs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Path to the Acl policy file | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSystemAclsDELETEDocsRequest struct via the builder pattern


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


## ApiSystemAclsPOSTDocs

> map[string]interface{} ApiSystemAclsPOSTDocs(ctx, path).Body(body).Execute()

Create an ACL Policy.



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
	path := "path_example" // string | Path to the Acl policy file
	body := "description: "my policy"
context:
  application: rundeck
for:
  project:
    - allow: read
by:
  group: build" // string | If the `Content-Type` is `application/yaml` or `text/plain`, then the request body is the ACL policy contents directly.  Otherwise, you can use JSON to wrap the yaml content inside `contents`  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ACLsAPI.ApiSystemAclsPOSTDocs(context.Background(), path).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLsAPI.ApiSystemAclsPOSTDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSystemAclsPOSTDocs`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ACLsAPI.ApiSystemAclsPOSTDocs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Path to the Acl policy file | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSystemAclsPOSTDocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | **string** | If the &#x60;Content-Type&#x60; is &#x60;application/yaml&#x60; or &#x60;text/plain&#x60;, then the request body is the ACL policy contents directly.  Otherwise, you can use JSON to wrap the yaml content inside &#x60;contents&#x60;  | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/yaml, application/json
- **Accept**: text/plain, application/yaml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSystemAclsPUTDocs

> ApiSystemAclsPUTDocs(ctx, path).Body(body).Execute()

Update an ACL Policy.



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
	path := "path_example" // string | Path to the Acl policy file
	body := "body_example" // string | If the `Content-Type` is `application/yaml` or `text/plain`, then the request body is the ACL policy contents directly.  Otherwise, you can use JSON to wrap the yaml content inside `contents`  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ACLsAPI.ApiSystemAclsPUTDocs(context.Background(), path).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLsAPI.ApiSystemAclsPUTDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**path** | **string** | Path to the Acl policy file | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSystemAclsPUTDocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | **string** | If the &#x60;Content-Type&#x60; is &#x60;application/yaml&#x60; or &#x60;text/plain&#x60;, then the request body is the ACL policy contents directly.  Otherwise, you can use JSON to wrap the yaml content inside &#x60;contents&#x60;  | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/yaml, application/json
- **Accept**: text/plain, application/yaml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


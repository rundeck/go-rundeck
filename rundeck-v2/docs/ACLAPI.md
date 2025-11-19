# \ACLAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiProjectAclsDeleteDocs**](ACLAPI.md#ApiProjectAclsDeleteDocs) | **Delete** /project/{project}/acl/{path} | Delete an ACL policy file.
[**ApiProjectAclsGetDocs**](ACLAPI.md#ApiProjectAclsGetDocs) | **Get** /project/{project}/acl/{path} | Get ACL Policy file for a project.
[**ApiProjectAclsPostDocs**](ACLAPI.md#ApiProjectAclsPostDocs) | **Post** /project/{project}/acl/{path} | Update a Project ACL Policy
[**ApiProjectAclsPutDocs**](ACLAPI.md#ApiProjectAclsPutDocs) | **Put** /project/{project}/acl/{path} | Update a Project ACL Policy
[**ApiSystemAcls**](ACLAPI.md#ApiSystemAcls) | **Get** /system/acl/{path} | Get an ACL Policy.
[**ApiSystemAclsDELETEDocs**](ACLAPI.md#ApiSystemAclsDELETEDocs) | **Delete** /system/acl/{path} | Delete an ACL Policy.
[**ApiSystemAclsPOSTDocs**](ACLAPI.md#ApiSystemAclsPOSTDocs) | **Post** /system/acl/{path} | Create an ACL Policy.
[**ApiSystemAclsPUTDocs**](ACLAPI.md#ApiSystemAclsPUTDocs) | **Put** /system/acl/{path} | Update an ACL Policy.



## ApiProjectAclsDeleteDocs

> ApiProjectAclsDeleteDocs(ctx, project, path).Execute()

Delete an ACL policy file.



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
	path := "path_example" // string | Path to the ACL policy

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ACLAPI.ApiProjectAclsDeleteDocs(context.Background(), project, path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLAPI.ApiProjectAclsDeleteDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**path** | **string** | Path to the ACL policy | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectAclsDeleteDocsRequest struct via the builder pattern


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


## ApiProjectAclsGetDocs

> string ApiProjectAclsGetDocs(ctx, project, path).Execute()

Get ACL Policy file for a project.



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
	path := "path_example" // string | Path to the Acl policy file

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ACLAPI.ApiProjectAclsGetDocs(context.Background(), project, path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLAPI.ApiProjectAclsGetDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectAclsGetDocs`: string
	fmt.Fprintf(os.Stdout, "Response from `ACLAPI.ApiProjectAclsGetDocs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**path** | **string** | Path to the Acl policy file | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectAclsGetDocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/text, application/yaml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectAclsPostDocs

> string ApiProjectAclsPostDocs(ctx, project, path).Body(body).Execute()

Update a Project ACL Policy



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
	path := "path_example" // string | Path to the ACL Policy
	body := "description: "my policy"
context:
  application: rundeck
for:
  project:
    - allow: read
by:
  group: build" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ACLAPI.ApiProjectAclsPostDocs(context.Background(), project, path).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLAPI.ApiProjectAclsPostDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectAclsPostDocs`: string
	fmt.Fprintf(os.Stdout, "Response from `ACLAPI.ApiProjectAclsPostDocs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**path** | **string** | Path to the ACL Policy | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectAclsPostDocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | **string** |  | 

### Return type

**string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: text/plain, application/yaml, application/json
- **Accept**: text/plain, application/x-yaml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectAclsPutDocs

> ApiProjectAclsPutDocs(ctx, project, path).Body(body).Execute()

Update a Project ACL Policy



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
	path := "path_example" // string | Path to the ACL Policy
	body := "description: "my policy"
context:
  application: rundeck
for:
  project:
    - allow: read
by:
  group: build" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ACLAPI.ApiProjectAclsPutDocs(context.Background(), project, path).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLAPI.ApiProjectAclsPutDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**path** | **string** | Path to the ACL Policy | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectAclsPutDocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | **string** |  | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: text/plain, application/x-yaml, application/json
- **Accept**: application/text, application/yaml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


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
	r, err := apiClient.ACLAPI.ApiSystemAcls(context.Background(), path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLAPI.ApiSystemAcls``: %v\n", err)
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

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

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
	resp, r, err := apiClient.ACLAPI.ApiSystemAclsDELETEDocs(context.Background(), path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLAPI.ApiSystemAclsDELETEDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSystemAclsDELETEDocs`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ACLAPI.ApiSystemAclsDELETEDocs`: %v\n", resp)
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

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

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
	resp, r, err := apiClient.ACLAPI.ApiSystemAclsPOSTDocs(context.Background(), path).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLAPI.ApiSystemAclsPOSTDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSystemAclsPOSTDocs`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ACLAPI.ApiSystemAclsPOSTDocs`: %v\n", resp)
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

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

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
	r, err := apiClient.ACLAPI.ApiSystemAclsPUTDocs(context.Background(), path).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ACLAPI.ApiSystemAclsPUTDocs``: %v\n", err)
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

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/yaml, application/json
- **Accept**: text/plain, application/yaml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


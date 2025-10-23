# \TokensAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiTokenCreate**](TokensAPI.md#ApiTokenCreate) | **Post** /tokens/{user} | Create API Token
[**ApiTokenDelete**](TokensAPI.md#ApiTokenDelete) | **Delete** /token/{tokenid} | Delete a specified auth token.
[**ApiTokenGet**](TokensAPI.md#ApiTokenGet) | **Get** /token/{tokenid} | Get a specified auth token metadata
[**ApiTokenList**](TokensAPI.md#ApiTokenList) | **Get** /tokens/{user} | List all tokens or all tokens for a specific user.
[**ApiTokenRemoveExpired**](TokensAPI.md#ApiTokenRemoveExpired) | **Post** /tokens/{user}/removeExpired | Remove Expired Tokens



## ApiTokenCreate

> map[string]interface{} ApiTokenCreate(ctx, user).ApiTokenCreateRequest(apiTokenCreateRequest).Execute()

Create API Token



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
	user := "user_example" // string | username
	apiTokenCreateRequest := openapiclient.apiTokenCreate_request{CreateToken: openapiclient.NewCreateToken()} // ApiTokenCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TokensAPI.ApiTokenCreate(context.Background(), user).ApiTokenCreateRequest(apiTokenCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TokensAPI.ApiTokenCreate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiTokenCreate`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TokensAPI.ApiTokenCreate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**user** | **string** | username | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiTokenCreateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiTokenCreateRequest** | [**ApiTokenCreateRequest**](ApiTokenCreateRequest.md) |  | 

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


## ApiTokenDelete

> map[string]interface{} ApiTokenDelete(ctx, tokenid).Execute()

Delete a specified auth token.

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
	tokenid := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Token ID (UUID)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TokensAPI.ApiTokenDelete(context.Background(), tokenid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TokensAPI.ApiTokenDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiTokenDelete`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TokensAPI.ApiTokenDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tokenid** | **string** | Token ID (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiTokenDeleteRequest struct via the builder pattern


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


## ApiTokenGet

> Token ApiTokenGet(ctx, tokenid).Execute()

Get a specified auth token metadata



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
	tokenid := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Token ID (UUID)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TokensAPI.ApiTokenGet(context.Background(), tokenid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TokensAPI.ApiTokenGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiTokenGet`: Token
	fmt.Fprintf(os.Stdout, "Response from `TokensAPI.ApiTokenGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tokenid** | **string** | Token ID (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiTokenGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Token**](Token.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiTokenList

> []Token ApiTokenList(ctx, user).Execute()

List all tokens or all tokens for a specific user.

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
	user := "user_example" // string | username

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TokensAPI.ApiTokenList(context.Background(), user).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TokensAPI.ApiTokenList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiTokenList`: []Token
	fmt.Fprintf(os.Stdout, "Response from `TokensAPI.ApiTokenList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**user** | **string** | username | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiTokenListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]Token**](Token.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiTokenRemoveExpired

> RemoveExpiredTokens ApiTokenRemoveExpired(ctx, user).Execute()

Remove Expired Tokens



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
	user := "user_example" // string | username, or special value `*`

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TokensAPI.ApiTokenRemoveExpired(context.Background(), user).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TokensAPI.ApiTokenRemoveExpired``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiTokenRemoveExpired`: RemoveExpiredTokens
	fmt.Fprintf(os.Stdout, "Response from `TokensAPI.ApiTokenRemoveExpired`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**user** | **string** | username, or special value &#x60;*&#x60; | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiTokenRemoveExpiredRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RemoveExpiredTokens**](RemoveExpiredTokens.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


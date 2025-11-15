# \ConfigurationAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ConfigDelete**](ConfigurationAPI.md#ConfigDelete) | **Post** /config/delete | Delete a Single Config Value [Enterprise]
[**ConfigGet**](ConfigurationAPI.md#ConfigGet) | **Get** /config/get | Get Configuration Value [Enterprise]
[**ConfigGetCategories**](ConfigurationAPI.md#ConfigGetCategories) | **Get** /config/getCategories | Get Configuration Categories [Enterprise]
[**ConfigList**](ConfigurationAPI.md#ConfigList) | **Get** /config/list | List All Current Configurations [Enterprise]
[**ConfigMetaList**](ConfigurationAPI.md#ConfigMetaList) | **Get** /config/metaList | List Configuration Metadata [Enterprise]
[**ConfigSave**](ConfigurationAPI.md#ConfigSave) | **Post** /config/save | Create or Update Configurations [Enterprise]
[**Refresh**](ConfigurationAPI.md#Refresh) | **Post** /config/refresh | Refresh Configurations from Properties File [Enterprise]
[**Restart**](ConfigurationAPI.md#Restart) | **Post** /config/restart | Restart the Rundeck Server [Enterprise]
[**StorageConfigList**](ConfigurationAPI.md#StorageConfigList) | **Get** /config/listStoragePlugins | List All Currently configured Storage Plugins [Enterprise]
[**StorageConfigSave**](ConfigurationAPI.md#StorageConfigSave) | **Post** /config/saveStoragePlugins | Create or Update Storage Plugins [Enterprise]



## ConfigDelete

> map[string]interface{} ConfigDelete(ctx).Body(body).Execute()

Delete a Single Config Value [Enterprise]



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
	body := map[string]interface{}{ ... } // map[string]interface{} | Delete Config Request.  * `key` Required   * Represents the config to be deleted.   * Accepts: Any `string` * `strata` Optional   * Whether the config should apply to the current server (`Server`), or to all servers in the cluster (`default`).   * Accepts: `Server`, `default`   * Default: `default`  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConfigurationAPI.ConfigDelete(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.ConfigDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConfigDelete`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ConfigurationAPI.ConfigDelete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConfigDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **map[string]interface{}** | Delete Config Request.  * &#x60;key&#x60; Required   * Represents the config to be deleted.   * Accepts: Any &#x60;string&#x60; * &#x60;strata&#x60; Optional   * Whether the config should apply to the current server (&#x60;Server&#x60;), or to all servers in the cluster (&#x60;default&#x60;).   * Accepts: &#x60;Server&#x60;, &#x60;default&#x60;   * Default: &#x60;default&#x60;  | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ConfigGet

> ConfigGet(ctx).Key(key).Strata(strata).Execute()

Get Configuration Value [Enterprise]



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
	key := "key_example" // string | Configuration key
	strata := "strata_example" // string | Storage Strata. Can be `server` to indicate the current cluster member, or a member UUID, or `default` or global configuration (Default value). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ConfigurationAPI.ConfigGet(context.Background()).Key(key).Strata(strata).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.ConfigGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConfigGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **string** | Configuration key | 
 **strata** | **string** | Storage Strata. Can be &#x60;server&#x60; to indicate the current cluster member, or a member UUID, or &#x60;default&#x60; or global configuration (Default value). | 

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


## ConfigGetCategories

> ConfigGetCategories(ctx).Execute()

Get Configuration Categories [Enterprise]



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
	r, err := apiClient.ConfigurationAPI.ConfigGetCategories(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.ConfigGetCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiConfigGetCategoriesRequest struct via the builder pattern


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


## ConfigList

> ConfigList(ctx).Execute()

List All Current Configurations [Enterprise]



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
	r, err := apiClient.ConfigurationAPI.ConfigList(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.ConfigList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiConfigListRequest struct via the builder pattern


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


## ConfigMetaList

> ConfigMetaList(ctx).Execute()

List Configuration Metadata [Enterprise]



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
	r, err := apiClient.ConfigurationAPI.ConfigMetaList(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.ConfigMetaList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiConfigMetaListRequest struct via the builder pattern


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


## ConfigSave

> ConfigSave(ctx).RequestBody(requestBody).Execute()

Create or Update Configurations [Enterprise]



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
	requestBody := []map[string]interface{}{map[string]interface{}(123)} // []map[string]interface{} | Update Config Request. List of config values, each value contains:  * `key` Required   * Represents either a new config to be created, or an existing config to be updated.   * Accepts: Any `string` * `value` Required   * The value for the desired config `key`.   * Accepts: Any `string` * `strata` Optional   * Whether the config should apply to the current server (`Server`), or to all servers in the cluster (`default`).   * Accepts: `Server`, `default`   * Default: `default` 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ConfigurationAPI.ConfigSave(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.ConfigSave``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConfigSaveRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **requestBody** | **[]map[string]interface{}** | Update Config Request. List of config values, each value contains:  * &#x60;key&#x60; Required   * Represents either a new config to be created, or an existing config to be updated.   * Accepts: Any &#x60;string&#x60; * &#x60;value&#x60; Required   * The value for the desired config &#x60;key&#x60;.   * Accepts: Any &#x60;string&#x60; * &#x60;strata&#x60; Optional   * Whether the config should apply to the current server (&#x60;Server&#x60;), or to all servers in the cluster (&#x60;default&#x60;).   * Accepts: &#x60;Server&#x60;, &#x60;default&#x60;   * Default: &#x60;default&#x60;  | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Refresh

> Refresh(ctx).Execute()

Refresh Configurations from Properties File [Enterprise]



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
	r, err := apiClient.ConfigurationAPI.Refresh(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.Refresh``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRefreshRequest struct via the builder pattern


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


## Restart

> Restart(ctx).Execute()

Restart the Rundeck Server [Enterprise]



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
	r, err := apiClient.ConfigurationAPI.Restart(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.Restart``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRestartRequest struct via the builder pattern


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


## StorageConfigList

> StorageConfigList(ctx).Execute()

List All Currently configured Storage Plugins [Enterprise]



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
	r, err := apiClient.ConfigurationAPI.StorageConfigList(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.StorageConfigList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiStorageConfigListRequest struct via the builder pattern


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


## StorageConfigSave

> StorageConfigSave(ctx).RequestBody(requestBody).Execute()

Create or Update Storage Plugins [Enterprise]



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
	requestBody := []map[string]interface{}{map[string]interface{}(123)} // []map[string]interface{} | Update Storage Plugin Config Request. Configured plugins to be saved should be specified in the `plugins` array. Plugins that have been deleted should be specified in the `removedPlugins` array. 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ConfigurationAPI.StorageConfigSave(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConfigurationAPI.StorageConfigSave``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiStorageConfigSaveRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **requestBody** | **[]map[string]interface{}** | Update Storage Plugin Config Request. Configured plugins to be saved should be specified in the &#x60;plugins&#x60; array. Plugins that have been deleted should be specified in the &#x60;removedPlugins&#x60; array.  | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


# \AdHocAPI

All URIs are relative to *https://localhost:4440/api/59*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiRunCommandv14**](AdHocAPI.md#ApiRunCommandv14) | **Post** /project/{project}/run/command | Run Adhoc Command
[**ApiRunScriptUrlv14**](AdHocAPI.md#ApiRunScriptUrlv14) | **Post** /project/{project}/run/url | Run Adhoc Script URL
[**ApiRunScriptv14**](AdHocAPI.md#ApiRunScriptv14) | **Post** /project/{project}/run/script | Run Adhoc Script
[**RunAdhocInline**](AdHocAPI.md#RunAdhocInline) | **Post** /project/{project}/run/command/inline | Run Adhoc Command (Inline)
[**RunAdhocInlineApi**](AdHocAPI.md#RunAdhocInlineApi) | **Post** /project/{project}/run/command/inline/api | Run Adhoc Command (Inline) - API Auth



## ApiRunCommandv14

> map[string]interface{} ApiRunCommandv14(ctx, project).Filter(filter).Exec(exec).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).AsUser(asUser).ApiRunAdhocRequest(apiRunAdhocRequest).Execute()

Run Adhoc Command



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
	filter := "filter_example" // string | Node Filter String (optional)
	exec := "exec_example" // string | The shell command string to run, e.g. \"echo hello\". (optional)
	nodeThreadcount := int32(56) // int32 | threadcount to use (optional)
	nodeKeepgoing := true // bool | if \"true\", continue executing on other nodes even if some fail. (optional)
	asUser := "asUser_example" // string | specifies a username identifying the user who ran the command. Requires `runAs` permission. (optional)
	apiRunAdhocRequest := *openapiclient.NewApiRunAdhocRequest() // ApiRunAdhocRequest | Request body (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdHocAPI.ApiRunCommandv14(context.Background(), project).Filter(filter).Exec(exec).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).AsUser(asUser).ApiRunAdhocRequest(apiRunAdhocRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdHocAPI.ApiRunCommandv14``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiRunCommandv14`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdHocAPI.ApiRunCommandv14`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiRunCommandv14Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **string** | Node Filter String | 
 **exec** | **string** | The shell command string to run, e.g. \&quot;echo hello\&quot;. | 
 **nodeThreadcount** | **int32** | threadcount to use | 
 **nodeKeepgoing** | **bool** | if \&quot;true\&quot;, continue executing on other nodes even if some fail. | 
 **asUser** | **string** | specifies a username identifying the user who ran the command. Requires &#x60;runAs&#x60; permission. | 
 **apiRunAdhocRequest** | [**ApiRunAdhocRequest**](ApiRunAdhocRequest.md) | Request body | 

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


## ApiRunScriptUrlv14

> map[string]interface{} ApiRunScriptUrlv14(ctx, project).Filter(filter).ArgString(argString).ScriptURL(scriptURL).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).AsUser(asUser).ScriptInterpreter(scriptInterpreter).FileExtension(fileExtension).InterpreterArgsQuoted(interpreterArgsQuoted).ApiRunScriptv14Request1(apiRunScriptv14Request1).Execute()

Run Adhoc Script URL



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
	filter := "filter_example" // string | Node Filter String (optional)
	argString := "argString_example" // string | Arguments to pass to the script when executed (optional)
	scriptURL := "scriptURL_example" // string | A URL pointing to a script file (optional)
	nodeThreadcount := int32(56) // int32 | threadcount to use (optional)
	nodeKeepgoing := true // bool | if \"true\", continue executing on other nodes even if some fail. (optional)
	asUser := "asUser_example" // string | specifies a username identifying the user who ran the command. Requires `runAs` permission. (optional)
	scriptInterpreter := "scriptInterpreter_example" // string | a command to use to run the script (optional)
	fileExtension := "fileExtension_example" // string | extension of the script file on the remote node (since v14) (optional)
	interpreterArgsQuoted := true // bool | if true, the script file and arguments will be quoted as the last argument to the `scriptInterpreter` (optional)
	apiRunScriptv14Request1 := *openapiclient.NewApiRunScriptv14Request1() // ApiRunScriptv14Request1 | Adhoc Script URL Request (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdHocAPI.ApiRunScriptUrlv14(context.Background(), project).Filter(filter).ArgString(argString).ScriptURL(scriptURL).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).AsUser(asUser).ScriptInterpreter(scriptInterpreter).FileExtension(fileExtension).InterpreterArgsQuoted(interpreterArgsQuoted).ApiRunScriptv14Request1(apiRunScriptv14Request1).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdHocAPI.ApiRunScriptUrlv14``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiRunScriptUrlv14`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdHocAPI.ApiRunScriptUrlv14`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiRunScriptUrlv14Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **string** | Node Filter String | 
 **argString** | **string** | Arguments to pass to the script when executed | 
 **scriptURL** | **string** | A URL pointing to a script file | 
 **nodeThreadcount** | **int32** | threadcount to use | 
 **nodeKeepgoing** | **bool** | if \&quot;true\&quot;, continue executing on other nodes even if some fail. | 
 **asUser** | **string** | specifies a username identifying the user who ran the command. Requires &#x60;runAs&#x60; permission. | 
 **scriptInterpreter** | **string** | a command to use to run the script | 
 **fileExtension** | **string** | extension of the script file on the remote node (since v14) | 
 **interpreterArgsQuoted** | **bool** | if true, the script file and arguments will be quoted as the last argument to the &#x60;scriptInterpreter&#x60; | 
 **apiRunScriptv14Request1** | [**ApiRunScriptv14Request1**](ApiRunScriptv14Request1.md) | Adhoc Script URL Request | 

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


## ApiRunScriptv14

> map[string]interface{} ApiRunScriptv14(ctx, project).Filter(filter).ArgString(argString).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).AsUser(asUser).ScriptInterpreter(scriptInterpreter).FileExtension(fileExtension).InterpreterArgsQuoted(interpreterArgsQuoted).RunAdhocRequest(runAdhocRequest).Execute()

Run Adhoc Script



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
	filter := "filter_example" // string | Node Filter String (optional)
	argString := "argString_example" // string | Arguments to pass to the script when executed (optional)
	nodeThreadcount := int32(56) // int32 | threadcount to use (optional)
	nodeKeepgoing := true // bool | if \"true\", continue executing on other nodes even if some fail. (optional)
	asUser := "asUser_example" // string | specifies a username identifying the user who ran the command. Requires `runAs` permission. (optional)
	scriptInterpreter := "scriptInterpreter_example" // string | a command to use to run the script (optional)
	fileExtension := "fileExtension_example" // string | extension of the script file on the remote node (since v14) (optional)
	interpreterArgsQuoted := true // bool | if true, the script file and arguments will be quoted as the last argument to the `scriptInterpreter` (optional)
	runAdhocRequest := *openapiclient.NewApiRunAdhocRequest() // ApiRunAdhocRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdHocAPI.ApiRunScriptv14(context.Background(), project).Filter(filter).ArgString(argString).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).AsUser(asUser).ScriptInterpreter(scriptInterpreter).FileExtension(fileExtension).InterpreterArgsQuoted(interpreterArgsQuoted).RunAdhocRequest(runAdhocRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdHocAPI.ApiRunScriptv14``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiRunScriptv14`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdHocAPI.ApiRunScriptv14`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiRunScriptv14Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **string** | Node Filter String | 
 **argString** | **string** | Arguments to pass to the script when executed | 
 **nodeThreadcount** | **int32** | threadcount to use | 
 **nodeKeepgoing** | **bool** | if \&quot;true\&quot;, continue executing on other nodes even if some fail. | 
 **asUser** | **string** | specifies a username identifying the user who ran the command. Requires &#x60;runAs&#x60; permission. | 
 **scriptInterpreter** | **string** | a command to use to run the script | 
 **fileExtension** | **string** | extension of the script file on the remote node (since v14) | 
 **interpreterArgsQuoted** | **bool** | if true, the script file and arguments will be quoted as the last argument to the &#x60;scriptInterpreter&#x60; | 
 **runAdhocRequest** | [**ApiRunAdhocRequest**](ApiRunAdhocRequest.md) |  | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: multipart/form-data, application/x-www-form-urlencoded, application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RunAdhocInline

> map[string]interface{} RunAdhocInline(ctx, project).Filter(filter).Exec(exec).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).FilterExclude(filterExclude).DoNodedispatch(doNodedispatch).ApiRunAdhocRequest(apiRunAdhocRequest).Execute()

Run Adhoc Command (Inline)



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
	filter := "filter_example" // string | Node Filter String (optional)
	exec := "exec_example" // string | The shell command string to run, e.g. \"echo hello\". (optional)
	nodeThreadcount := int32(56) // int32 | threadcount to use (optional)
	nodeKeepgoing := true // bool | if \"true\", continue executing on other nodes even if some fail. (optional)
	filterExclude := "filterExclude_example" // string | Node exclude filter string (optional)
	doNodedispatch := "doNodedispatch_example" // string | Enable node dispatch (optional)
	apiRunAdhocRequest := *openapiclient.NewApiRunAdhocRequest() // ApiRunAdhocRequest | Request body (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdHocAPI.RunAdhocInline(context.Background(), project).Filter(filter).Exec(exec).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).FilterExclude(filterExclude).DoNodedispatch(doNodedispatch).ApiRunAdhocRequest(apiRunAdhocRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdHocAPI.RunAdhocInline``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RunAdhocInline`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdHocAPI.RunAdhocInline`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiRunAdhocInlineRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **string** | Node Filter String | 
 **exec** | **string** | The shell command string to run, e.g. \&quot;echo hello\&quot;. | 
 **nodeThreadcount** | **int32** | threadcount to use | 
 **nodeKeepgoing** | **bool** | if \&quot;true\&quot;, continue executing on other nodes even if some fail. | 
 **filterExclude** | **string** | Node exclude filter string | 
 **doNodedispatch** | **string** | Enable node dispatch | 
 **apiRunAdhocRequest** | [**ApiRunAdhocRequest**](ApiRunAdhocRequest.md) | Request body | 

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


## RunAdhocInlineApi

> map[string]interface{} RunAdhocInlineApi(ctx, project).Filter(filter).Exec(exec).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).FilterExclude(filterExclude).DoNodedispatch(doNodedispatch).ApiRunAdhocRequest(apiRunAdhocRequest).Execute()

Run Adhoc Command (Inline) - API Auth



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
	filter := "filter_example" // string | Node Filter String (optional)
	exec := "exec_example" // string | The shell command string to run, e.g. \"echo hello\". (optional)
	nodeThreadcount := int32(56) // int32 | threadcount to use (optional)
	nodeKeepgoing := true // bool | if \"true\", continue executing on other nodes even if some fail. (optional)
	filterExclude := "filterExclude_example" // string | Node exclude filter string (optional)
	doNodedispatch := "doNodedispatch_example" // string | Enable node dispatch (optional)
	apiRunAdhocRequest := *openapiclient.NewApiRunAdhocRequest() // ApiRunAdhocRequest | Request body (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdHocAPI.RunAdhocInlineApi(context.Background(), project).Filter(filter).Exec(exec).NodeThreadcount(nodeThreadcount).NodeKeepgoing(nodeKeepgoing).FilterExclude(filterExclude).DoNodedispatch(doNodedispatch).ApiRunAdhocRequest(apiRunAdhocRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdHocAPI.RunAdhocInlineApi``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RunAdhocInlineApi`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdHocAPI.RunAdhocInlineApi`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiRunAdhocInlineApiRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **string** | Node Filter String | 
 **exec** | **string** | The shell command string to run, e.g. \&quot;echo hello\&quot;. | 
 **nodeThreadcount** | **int32** | threadcount to use | 
 **nodeKeepgoing** | **bool** | if \&quot;true\&quot;, continue executing on other nodes even if some fail. | 
 **filterExclude** | **string** | Node exclude filter string | 
 **doNodedispatch** | **string** | Enable node dispatch | 
 **apiRunAdhocRequest** | [**ApiRunAdhocRequest**](ApiRunAdhocRequest.md) | Request body | 

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


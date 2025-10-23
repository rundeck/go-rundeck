# \ProjectAPI

All URIs are relative to *https://localhost:4440/api/44*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiProjectConfigGet**](ProjectAPI.md#ApiProjectConfigGet) | **Get** /project/{project}/config | Get a project config
[**ApiProjectConfigKeyDelete**](ProjectAPI.md#ApiProjectConfigKeyDelete) | **Delete** /project/{project}/config/{keypath} | Delete the key
[**ApiProjectConfigKeyGet**](ProjectAPI.md#ApiProjectConfigKeyGet) | **Get** /project/{project}/config/{keypath} | Get an individual project config by their key
[**ApiProjectConfigKeyPut**](ProjectAPI.md#ApiProjectConfigKeyPut) | **Put** /project/{project}/config/{keypath} | Set the value.
[**ApiProjectConfigPut**](ProjectAPI.md#ApiProjectConfigPut) | **Put** /project/{project}/config | Modify a project config
[**ApiProjectCreate**](ProjectAPI.md#ApiProjectCreate) | **Post** /projects | Create a Project
[**ApiProjectDelete**](ProjectAPI.md#ApiProjectDelete) | **Delete** /project/{project} | Delete a project
[**ApiProjectExport**](ProjectAPI.md#ApiProjectExport) | **Get** /project/{project}/export | Export a zip archive of the project.
[**ApiProjectExportAsyncDocs**](ProjectAPI.md#ApiProjectExportAsyncDocs) | **Get** /project/{project}/export/async | Export a zip archive of the project asynchronously.
[**ApiProjectExportAsyncDownload**](ProjectAPI.md#ApiProjectExportAsyncDownload) | **Get** /project/{project}/export/download/{token} | Download the zip archive file
[**ApiProjectExportAsyncStatus**](ProjectAPI.md#ApiProjectExportAsyncStatus) | **Get** /project/{project}/export/status/{token} | Get the status of an async export request
[**ApiProjectFileDelete**](ProjectAPI.md#ApiProjectFileDelete) | **Delete** /project/{project}/{filename} | Delete &#x60;readme.md&#x60; and &#x60;motd.md&#x60;
[**ApiProjectFileGet**](ProjectAPI.md#ApiProjectFileGet) | **Get** /project/{project}/{filename} | Get &#x60;readme.md&#x60; and &#x60;motd.md&#x60;
[**ApiProjectFilePut**](ProjectAPI.md#ApiProjectFilePut) | **Put** /project/{project}/{filename} | To create or modify the &#x60;readme.md&#x60; and &#x60;motd.md&#x60; contents
[**ApiProjectGet**](ProjectAPI.md#ApiProjectGet) | **Get** /project/{project} | Get a project
[**ApiProjectImport**](ProjectAPI.md#ApiProjectImport) | **Put** /project/{project}/import | Import a zip archive.
[**ApiProjectList1**](ProjectAPI.md#ApiProjectList1) | **Get** /projects | List Projects
[**ApiProjectMeta**](ProjectAPI.md#ApiProjectMeta) | **Get** /project/{project}/meta | Get Project UI Metadata
[**ApiResourcesv2**](ProjectAPI.md#ApiResourcesv2) | **Get** /project/{project}/resources | List Project Nodes
[**ApiResourcev14**](ProjectAPI.md#ApiResourcev14) | **Get** /project/{project}/resource/{name} | Get Node Info
[**ApiSourceGet**](ProjectAPI.md#ApiSourceGet) | **Get** /project/{project}/source/{index} | Get a Resource Model Source for a Project
[**ApiSourceGetContent**](ProjectAPI.md#ApiSourceGetContent) | **Get** /project/{project}/source/{index}/resources | List Resources of a Resource Model Source
[**ApiSourceWriteContent**](ProjectAPI.md#ApiSourceWriteContent) | **Post** /project/{project}/source/{index}/resources | Update Resources of a Resource Model Source
[**ApiSourcesList**](ProjectAPI.md#ApiSourcesList) | **Get** /project/{project}/sources | List Resource Model Sources for a Project
[**ApiTagsForNodes**](ProjectAPI.md#ApiTagsForNodes) | **Get** /project/{project}/nodes/tags | List tags for project nodes
[**SaveProjectPlugins**](ProjectAPI.md#SaveProjectPlugins) | **Post** /project/{project}/plugins/save | Save list-style plugin configurations for a project



## ApiProjectConfigGet

> string ApiProjectConfigGet(ctx, project).Execute()

Get a project config



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
	project := "project_example" // string | Project Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectConfigGet(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectConfigGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectConfigGet`: string
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectConfigGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectConfigGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/text, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectConfigKeyDelete

> ApiProjectConfigKeyDelete(ctx, project, keypath).Execute()

Delete the key



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
	project := "project_example" // string | Project Name
	keypath := "keypath_example" // string | Key Path

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ProjectAPI.ApiProjectConfigKeyDelete(context.Background(), project, keypath).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectConfigKeyDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**keypath** | **string** | Key Path | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectConfigKeyDeleteRequest struct via the builder pattern


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


## ApiProjectConfigKeyGet

> map[string]interface{} ApiProjectConfigKeyGet(ctx, project, keypath).Execute()

Get an individual project config by their key



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
	project := "project_example" // string | Project Name
	keypath := "keypath_example" // string | Key Path

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectConfigKeyGet(context.Background(), project, keypath).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectConfigKeyGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectConfigKeyGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectConfigKeyGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**keypath** | **string** | Key Path | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectConfigKeyGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/text, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectConfigKeyPut

> map[string]interface{} ApiProjectConfigKeyPut(ctx, project, keypath).EnablePluginValidation(enablePluginValidation).Body(body).Execute()

Set the value.



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
	project := "project_example" // string | Project Name
	keypath := "keypath_example" // string | Key Path
	enablePluginValidation := true // bool | Enable plugin validation (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectConfigKeyPut(context.Background(), project, keypath).EnablePluginValidation(enablePluginValidation).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectConfigKeyPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectConfigKeyPut`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectConfigKeyPut`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**keypath** | **string** | Key Path | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectConfigKeyPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **enablePluginValidation** | **bool** | Enable plugin validation | 
 **body** | **map[string]interface{}** |  | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json, text/plain
- **Accept**: application/json, text/plain

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectConfigPut

> map[string]interface{} ApiProjectConfigPut(ctx, project).Body(body).Execute()

Modify a project config



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
	project := "project_example" // string | Project Name
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectConfigPut(context.Background(), project).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectConfigPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectConfigPut`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectConfigPut`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectConfigPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | **map[string]interface{}** |  | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json, text/plain
- **Accept**: application/json, text/plain

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectCreate

> map[string]interface{} ApiProjectCreate(ctx).Body(body).Execute()

Create a Project



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
	body := map[string]interface{}{ ... } // map[string]interface{} | Project Create contains a name, and configuration values (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectCreate(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectCreate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectCreate`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectCreate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectCreateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **map[string]interface{}** | Project Create contains a name, and configuration values | 

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


## ApiProjectDelete

> ApiProjectDelete(ctx, project).Deferred(deferred).Execute()

Delete a project



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
	project := "project_example" // string | Project Name
	deferred := true // bool | Deferred Delete. Since: v45 (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ProjectAPI.ApiProjectDelete(context.Background(), project).Deferred(deferred).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **deferred** | **bool** | Deferred Delete. Since: v45 | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectExport

> map[string]interface{} ApiProjectExport(ctx, project).ArchiveParams(archiveParams).ExecutionIds(executionIds).ExportAll(exportAll).ExportJobs(exportJobs).ExportExecutions(exportExecutions).ExportConfigs(exportConfigs).ExportReadmes(exportReadmes).ExportAcls(exportAcls).ExportComponentsCalendars(exportComponentsCalendars).ExportComponentsSchedule20Definitions(exportComponentsSchedule20Definitions).ExportComponentsToursManager(exportComponentsToursManager).ExportComponentsNodeWizard(exportComponentsNodeWizard).Execute()

Export a zip archive of the project.



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
	project := "project_example" // string | Project Name
	archiveParams := *openapiclient.NewProjectArchiveParams() // ProjectArchiveParams | 
	executionIds := "executionIds_example" // string | List of execution to include to the exported archive (optional)
	exportAll := "exportAll_example" // string | true/false, include all project contents (default: true) (optional)
	exportJobs := "exportJobs_example" // string | true/false, include jobs (optional)
	exportExecutions := "exportExecutions_example" // string | true/false, include executions (optional)
	exportConfigs := "exportConfigs_example" // string | true/false, include project configuration (optional)
	exportReadmes := "exportReadmes_example" // string | true/false, include project readme/motd files (optional)
	exportAcls := "exportAcls_example" // string | true/false, include project ACL Policy files, if authorized (optional)
	exportComponentsCalendars := "exportComponentsCalendars_example" // string | true/false, include project calendars (optional)
	exportComponentsSchedule20Definitions := "exportComponentsSchedule20Definitions_example" // string | true/false, include schedule definitions (optional)
	exportComponentsToursManager := "exportComponentsToursManager_example" // string | true/false, include tours manager (optional)
	exportComponentsNodeWizard := "exportComponentsNodeWizard_example" // string | true/false, include node wizard (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectExport(context.Background(), project).ArchiveParams(archiveParams).ExecutionIds(executionIds).ExportAll(exportAll).ExportJobs(exportJobs).ExportExecutions(exportExecutions).ExportConfigs(exportConfigs).ExportReadmes(exportReadmes).ExportAcls(exportAcls).ExportComponentsCalendars(exportComponentsCalendars).ExportComponentsSchedule20Definitions(exportComponentsSchedule20Definitions).ExportComponentsToursManager(exportComponentsToursManager).ExportComponentsNodeWizard(exportComponentsNodeWizard).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectExport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectExport`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectExport`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectExportRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **archiveParams** | [**ProjectArchiveParams**](ProjectArchiveParams.md) |  | 
 **executionIds** | **string** | List of execution to include to the exported archive | 
 **exportAll** | **string** | true/false, include all project contents (default: true) | 
 **exportJobs** | **string** | true/false, include jobs | 
 **exportExecutions** | **string** | true/false, include executions | 
 **exportConfigs** | **string** | true/false, include project configuration | 
 **exportReadmes** | **string** | true/false, include project readme/motd files | 
 **exportAcls** | **string** | true/false, include project ACL Policy files, if authorized | 
 **exportComponentsCalendars** | **string** | true/false, include project calendars | 
 **exportComponentsSchedule20Definitions** | **string** | true/false, include schedule definitions | 
 **exportComponentsToursManager** | **string** | true/false, include tours manager | 
 **exportComponentsNodeWizard** | **string** | true/false, include node wizard | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/zip, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectExportAsyncDocs

> map[string]interface{} ApiProjectExportAsyncDocs(ctx, project).ExecutionIds(executionIds).ExportAll(exportAll).ExportJobs(exportJobs).ExportExecutions(exportExecutions).ExportConfigs(exportConfigs).ExportReadmes(exportReadmes).ExportAcls(exportAcls).ExportComponentsCalendars(exportComponentsCalendars).ExportComponentsSchedule20Definitions(exportComponentsSchedule20Definitions).ExportComponentsToursManager(exportComponentsToursManager).ExportComponentsNodeWizard(exportComponentsNodeWizard).Execute()

Export a zip archive of the project asynchronously.



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
	project := "project_example" // string | Project Name
	executionIds := "executionIds_example" // string | List of execution to include to the exported archive (optional)
	exportAll := "exportAll_example" // string | true/false, include all project contents (default: true) (optional)
	exportJobs := "exportJobs_example" // string | true/false, include jobs (optional)
	exportExecutions := "exportExecutions_example" // string | true/false, include executions (optional)
	exportConfigs := "exportConfigs_example" // string | true/false, include project configuration (optional)
	exportReadmes := "exportReadmes_example" // string | true/false, include project readme/motd files (optional)
	exportAcls := "exportAcls_example" // string | true/false, include project ACL Policy files, if authorized (optional)
	exportComponentsCalendars := "exportComponentsCalendars_example" // string | true/false, include project calendars (optional)
	exportComponentsSchedule20Definitions := "exportComponentsSchedule20Definitions_example" // string | true/false, include schedule definitions (optional)
	exportComponentsToursManager := "exportComponentsToursManager_example" // string | true/false, include tours manager (optional)
	exportComponentsNodeWizard := "exportComponentsNodeWizard_example" // string | true/false, include node wizard (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectExportAsyncDocs(context.Background(), project).ExecutionIds(executionIds).ExportAll(exportAll).ExportJobs(exportJobs).ExportExecutions(exportExecutions).ExportConfigs(exportConfigs).ExportReadmes(exportReadmes).ExportAcls(exportAcls).ExportComponentsCalendars(exportComponentsCalendars).ExportComponentsSchedule20Definitions(exportComponentsSchedule20Definitions).ExportComponentsToursManager(exportComponentsToursManager).ExportComponentsNodeWizard(exportComponentsNodeWizard).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectExportAsyncDocs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectExportAsyncDocs`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectExportAsyncDocs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectExportAsyncDocsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **executionIds** | **string** | List of execution to include to the exported archive | 
 **exportAll** | **string** | true/false, include all project contents (default: true) | 
 **exportJobs** | **string** | true/false, include jobs | 
 **exportExecutions** | **string** | true/false, include executions | 
 **exportConfigs** | **string** | true/false, include project configuration | 
 **exportReadmes** | **string** | true/false, include project readme/motd files | 
 **exportAcls** | **string** | true/false, include project ACL Policy files, if authorized | 
 **exportComponentsCalendars** | **string** | true/false, include project calendars | 
 **exportComponentsSchedule20Definitions** | **string** | true/false, include schedule definitions | 
 **exportComponentsToursManager** | **string** | true/false, include tours manager | 
 **exportComponentsNodeWizard** | **string** | true/false, include node wizard | 

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


## ApiProjectExportAsyncDownload

> map[string]interface{} ApiProjectExportAsyncDownload(ctx, project, token).Execute()

Download the zip archive file



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
	project := "project_example" // string | Project Name
	token := "token_example" // string | Token to retrieve export status

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectExportAsyncDownload(context.Background(), project, token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectExportAsyncDownload``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectExportAsyncDownload`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectExportAsyncDownload`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**token** | **string** | Token to retrieve export status | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectExportAsyncDownloadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/zip, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectExportAsyncStatus

> map[string]interface{} ApiProjectExportAsyncStatus(ctx, project, token).Execute()

Get the status of an async export request



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
	project := "project_example" // string | Project Name
	token := "token_example" // string | Token to retrieve export status

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectExportAsyncStatus(context.Background(), project, token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectExportAsyncStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectExportAsyncStatus`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectExportAsyncStatus`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**token** | **string** | Token to retrieve export status | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectExportAsyncStatusRequest struct via the builder pattern


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


## ApiProjectFileDelete

> ApiProjectFileDelete(ctx, project, filename).Execute()

Delete `readme.md` and `motd.md`



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
	project := "project_example" // string | Project Name
	filename := "filename_example" // string | `readme.md` or `motd.md` file name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ProjectAPI.ApiProjectFileDelete(context.Background(), project, filename).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectFileDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**filename** | **string** | &#x60;readme.md&#x60; or &#x60;motd.md&#x60; file name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectFileDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectFileGet

> string ApiProjectFileGet(ctx, project, filename).Execute()

Get `readme.md` and `motd.md`



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
	project := "project_example" // string | Project Name
	filename := "filename_example" // string | `readme.md` or `motd.md` file name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectFileGet(context.Background(), project, filename).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectFileGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectFileGet`: string
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectFileGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**filename** | **string** | &#x60;readme.md&#x60; or &#x60;motd.md&#x60; file name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectFileGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/text, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectFilePut

> string ApiProjectFilePut(ctx, project, filename).Body(body).Execute()

To create or modify the `readme.md` and `motd.md` contents



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
	project := "project_example" // string | Project Name
	filename := "filename_example" // string | `readme.md` and `motd.md` file name
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectFilePut(context.Background(), project, filename).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectFilePut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectFilePut`: string
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectFilePut`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**filename** | **string** | &#x60;readme.md&#x60; and &#x60;motd.md&#x60; file name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectFilePutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | **map[string]interface{}** |  | 

### Return type

**string**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json, text/plain
- **Accept**: application/text, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectGet

> map[string]interface{} ApiProjectGet(ctx, project).Execute()

Get a project



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
	project := "project_example" // string | Project Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectGet(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectGetRequest struct via the builder pattern


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


## ApiProjectImport

> map[string]interface{} ApiProjectImport(ctx, project).JobUuidOption(jobUuidOption).ImportExecutions(importExecutions).ImportConfig(importConfig).ImportACL(importACL).ImportScm(importScm).ImportWebhooks(importWebhooks).WhkRegenAuthTokens(whkRegenAuthTokens).ImportNodesSources(importNodesSources).ImportComponentsNAME(importComponentsNAME).ImportOptsNAMEKEY(importOptsNAMEKEY).Body(body).Execute()

Import a zip archive.



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
	project := "project_example" // string | Project Name
	jobUuidOption := "jobUuidOption_example" // string | Option declaring how duplicate Job UUIDs should be handled.  If preserve (default) then imported job UUIDs will not be modified, and may conflict with jobs in other projects.  If remove then all job UUIDs will be removed before importing. (optional)
	importExecutions := true // bool | If true, import all executions and logs from the archive (default).  If false, do not import executions or logs. (optional)
	importConfig := true // bool | If true, import the project configuration from the archive.  If false, do not import the project configuration (default). (optional)
	importACL := true // bool | If true, import all of the ACL Policies from the archive.  If false, do not import the ACL Policies (default). (optional)
	importScm := true // bool | If true, import SCM configuration from the archive.  If false, do not import the SCM configuration (default). (optional)
	importWebhooks := true // bool | In APIv34 or later: If true, import the webhooks in the archive.  If false, do not import webhooks (default). (optional)
	whkRegenAuthTokens := true // bool | In APIv34 or later: If true, always regenerate the auth tokens associated with the webhook.  If false, the webhook auth token in the archive will be imported.  If no auth token info was included with the webhook, it will be generated (default). (optional)
	importNodesSources := true // bool | In APIv38 or later: If true, import Node Resources Source defined on project properties.  If false, do not import the nodes sources. (optional)
	importComponentsNAME := "importComponentsNAME_example" // string | Enable a component for import. Project archives may contain \"components\" which can be imported, beyond the base set of contents. This includes some data used by Runbook Automation (prev. Rundeck Enterprise) features.  For example, to enable Webhook import, you could use `importWebhooks` and `whkRegenAuthTokens` params, but those are simply shortcuts for the following parameters:  * `importComponents.webhooks=true&importOpts.webhooks.regenAuthTokens=true`  Import schedules definitions:  * `importComponents.Schedule%20Definitions=true` (optional)
	importOptsNAMEKEY := "importOptsNAMEKEY_example" // string | Set a component option. See `importComponents.NAME` parameter description (optional)
	body := os.NewFile(1234, "some_file") // *os.File |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectImport(context.Background(), project).JobUuidOption(jobUuidOption).ImportExecutions(importExecutions).ImportConfig(importConfig).ImportACL(importACL).ImportScm(importScm).ImportWebhooks(importWebhooks).WhkRegenAuthTokens(whkRegenAuthTokens).ImportNodesSources(importNodesSources).ImportComponentsNAME(importComponentsNAME).ImportOptsNAMEKEY(importOptsNAMEKEY).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectImport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectImport`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectImport`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectImportRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **jobUuidOption** | **string** | Option declaring how duplicate Job UUIDs should be handled.  If preserve (default) then imported job UUIDs will not be modified, and may conflict with jobs in other projects.  If remove then all job UUIDs will be removed before importing. | 
 **importExecutions** | **bool** | If true, import all executions and logs from the archive (default).  If false, do not import executions or logs. | 
 **importConfig** | **bool** | If true, import the project configuration from the archive.  If false, do not import the project configuration (default). | 
 **importACL** | **bool** | If true, import all of the ACL Policies from the archive.  If false, do not import the ACL Policies (default). | 
 **importScm** | **bool** | If true, import SCM configuration from the archive.  If false, do not import the SCM configuration (default). | 
 **importWebhooks** | **bool** | In APIv34 or later: If true, import the webhooks in the archive.  If false, do not import webhooks (default). | 
 **whkRegenAuthTokens** | **bool** | In APIv34 or later: If true, always regenerate the auth tokens associated with the webhook.  If false, the webhook auth token in the archive will be imported.  If no auth token info was included with the webhook, it will be generated (default). | 
 **importNodesSources** | **bool** | In APIv38 or later: If true, import Node Resources Source defined on project properties.  If false, do not import the nodes sources. | 
 **importComponentsNAME** | **string** | Enable a component for import. Project archives may contain \&quot;components\&quot; which can be imported, beyond the base set of contents. This includes some data used by Runbook Automation (prev. Rundeck Enterprise) features.  For example, to enable Webhook import, you could use &#x60;importWebhooks&#x60; and &#x60;whkRegenAuthTokens&#x60; params, but those are simply shortcuts for the following parameters:  * &#x60;importComponents.webhooks&#x3D;true&amp;importOpts.webhooks.regenAuthTokens&#x3D;true&#x60;  Import schedules definitions:  * &#x60;importComponents.Schedule%20Definitions&#x3D;true&#x60; | 
 **importOptsNAMEKEY** | **string** | Set a component option. See &#x60;importComponents.NAME&#x60; parameter description | 
 **body** | ***os.File** |  | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/zip
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectList1

> []map[string]interface{} ApiProjectList1(ctx).Meta(meta).Execute()

List Projects



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
	meta := "meta_example" // string | Comma-separated list of metadata items to include, or \"*\" for all (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectList1(context.Background()).Meta(meta).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectList1``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectList1`: []map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectList1`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectList1Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **meta** | **string** | Comma-separated list of metadata items to include, or \&quot;*\&quot; for all | 

### Return type

**[]map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiProjectMeta

> []ItemMeta ApiProjectMeta(ctx, project).Meta(meta).Execute()

Get Project UI Metadata



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
	project := "project_example" // string | Project name
	meta := "meta_example" // string | Comma-separated list of metadata items to include, or \"*\" for all (default)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiProjectMeta(context.Background(), project).Meta(meta).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiProjectMeta``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiProjectMeta`: []ItemMeta
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiProjectMeta`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiProjectMetaRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **meta** | **string** | Comma-separated list of metadata items to include, or \&quot;*\&quot; for all (default) | 

### Return type

[**[]ItemMeta**](ItemMeta.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiResourcesv2

> map[string]interface{} ApiResourcesv2(ctx, project).Filter(filter).Execute()

List Project Nodes



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
	project := "project_example" // string | Project Name
	filter := "filter_example" // string | Node Filter String (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiResourcesv2(context.Background(), project).Filter(filter).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiResourcesv2``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiResourcesv2`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiResourcesv2`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiResourcesv2Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **string** | Node Filter String | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/yaml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiResourcev14

> map[string]interface{} ApiResourcev14(ctx, project, name).Execute()

Get Node Info



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
	project := "project_example" // string | Project Name
	name := "name_example" // string | Node Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiResourcev14(context.Background(), project, name).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiResourcev14``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiResourcev14`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiResourcev14`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**name** | **string** | Node Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiResourcev14Request struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/yaml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSourceGet

> Source ApiSourceGet(ctx, project, index).Execute()

Get a Resource Model Source for a Project



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
	project := "project_example" // string | Project Name
	index := int32(56) // int32 | Source Index

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiSourceGet(context.Background(), project, index).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiSourceGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSourceGet`: Source
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiSourceGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**index** | **int32** | Source Index | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSourceGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**Source**](Source.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSourceGetContent

> map[string]interface{} ApiSourceGetContent(ctx, project, index).Execute()

List Resources of a Resource Model Source



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
	project := "project_example" // string | Project Name
	index := int32(56) // int32 | Source Index

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiSourceGetContent(context.Background(), project, index).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiSourceGetContent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSourceGetContent`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiSourceGetContent`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**index** | **int32** | Source Index | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSourceGetContentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/yaml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSourceWriteContent

> map[string]interface{} ApiSourceWriteContent(ctx, project, index).Body(body).Execute()

Update Resources of a Resource Model Source



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
	project := "project_example" // string | Project Name
	index := int32(56) // int32 | Source Index
	body := map[string]interface{}{ ... } // map[string]interface{} | Resource model data in the supported format

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiSourceWriteContent(context.Background(), project, index).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiSourceWriteContent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSourceWriteContent`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiSourceWriteContent`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 
**index** | **int32** | Source Index | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSourceWriteContentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | **map[string]interface{}** | Resource model data in the supported format | 

### Return type

**map[string]interface{}**

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json, text/yaml
- **Accept**: application/json, text/yaml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiSourcesList

> []Source ApiSourcesList(ctx, project).Execute()

List Resource Model Sources for a Project



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
	project := "project_example" // string | Project Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiSourcesList(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiSourcesList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiSourcesList`: []Source
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiSourcesList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiSourcesListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]Source**](Source.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiTagsForNodes

> TagsForNodesResponse ApiTagsForNodes(ctx, project).Execute()

List tags for project nodes



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
	project := "project_example" // string | Project Name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProjectAPI.ApiTagsForNodes(context.Background(), project).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.ApiTagsForNodes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiTagsForNodes`: TagsForNodesResponse
	fmt.Fprintf(os.Stdout, "Response from `ProjectAPI.ApiTagsForNodes`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project Name | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiTagsForNodesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TagsForNodesResponse**](TagsForNodesResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SaveProjectPlugins

> SaveProjectPlugins(ctx, project).ServiceName(serviceName).ConfigPrefix(configPrefix).Body(body).Execute()

Save list-style plugin configurations for a project



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
	project := "project_example" // string | Project name
	serviceName := "serviceName_example" // string | Plugin service name (e.g. `ResourceModelSource`)
	configPrefix := "configPrefix_example" // string | Property prefix (e.g. `resources.source`)
	body := map[string]interface{}{ ... } // map[string]interface{} | Plugins payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ProjectAPI.SaveProjectPlugins(context.Background(), project).ServiceName(serviceName).ConfigPrefix(configPrefix).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProjectAPI.SaveProjectPlugins``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**project** | **string** | Project name | 

### Other Parameters

Other parameters are passed through a pointer to a apiSaveProjectPluginsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **serviceName** | **string** | Plugin service name (e.g. &#x60;ResourceModelSource&#x60;) | 
 **configPrefix** | **string** | Property prefix (e.g. &#x60;resources.source&#x60;) | 
 **body** | **map[string]interface{}** | Plugins payload | 

### Return type

 (empty response body)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


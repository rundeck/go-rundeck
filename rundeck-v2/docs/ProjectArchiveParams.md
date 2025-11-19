# ProjectArchiveParams

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Project** | Pointer to **string** |  | [optional] 
**JobUuidOption** | Pointer to **string** |  | [optional] 
**ImportExecutions** | Pointer to **bool** |  | [optional] 
**ImportConfig** | Pointer to **bool** |  | [optional] 
**ImportNodesSources** | Pointer to **bool** |  | [optional] 
**ImportACL** | Pointer to **bool** |  | [optional] 
**ImportScm** | Pointer to **bool** |  | [optional] 
**ValidateJobref** | Pointer to **bool** |  | [optional] 
**ExportAll** | Pointer to **bool** |  | [optional] 
**ExportJobs** | Pointer to **bool** |  | [optional] 
**ExportExecutions** | Pointer to **bool** |  | [optional] 
**ExportConfigs** | Pointer to **bool** |  | [optional] 
**ExportReadmes** | Pointer to **bool** |  | [optional] 
**ExportAcls** | Pointer to **bool** |  | [optional] 
**ExportScm** | Pointer to **bool** |  | [optional] 
**ImportComponents** | Pointer to **map[string]bool** |  | [optional] 
**ImportOpts** | Pointer to **map[string]map[string]string** |  | [optional] 
**ExportComponents** | Pointer to **map[string]bool** |  | [optional] 
**ExportOpts** | Pointer to **map[string]map[string]string** |  | [optional] 
**StripJobRef** | Pointer to **string** |  | [optional] 
**Targetproject** | Pointer to **string** |  | [optional] 
**Apitoken** | Pointer to **string** |  | [optional] 
**Url** | Pointer to **string** |  | [optional] 
**Preserveuuid** | Pointer to **bool** |  | [optional] 
**AsyncImport** | Pointer to **bool** |  | [optional] 

## Methods

### NewProjectArchiveParams

`func NewProjectArchiveParams() *ProjectArchiveParams`

NewProjectArchiveParams instantiates a new ProjectArchiveParams object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProjectArchiveParamsWithDefaults

`func NewProjectArchiveParamsWithDefaults() *ProjectArchiveParams`

NewProjectArchiveParamsWithDefaults instantiates a new ProjectArchiveParams object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProject

`func (o *ProjectArchiveParams) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *ProjectArchiveParams) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *ProjectArchiveParams) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *ProjectArchiveParams) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetJobUuidOption

`func (o *ProjectArchiveParams) GetJobUuidOption() string`

GetJobUuidOption returns the JobUuidOption field if non-nil, zero value otherwise.

### GetJobUuidOptionOk

`func (o *ProjectArchiveParams) GetJobUuidOptionOk() (*string, bool)`

GetJobUuidOptionOk returns a tuple with the JobUuidOption field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobUuidOption

`func (o *ProjectArchiveParams) SetJobUuidOption(v string)`

SetJobUuidOption sets JobUuidOption field to given value.

### HasJobUuidOption

`func (o *ProjectArchiveParams) HasJobUuidOption() bool`

HasJobUuidOption returns a boolean if a field has been set.

### GetImportExecutions

`func (o *ProjectArchiveParams) GetImportExecutions() bool`

GetImportExecutions returns the ImportExecutions field if non-nil, zero value otherwise.

### GetImportExecutionsOk

`func (o *ProjectArchiveParams) GetImportExecutionsOk() (*bool, bool)`

GetImportExecutionsOk returns a tuple with the ImportExecutions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportExecutions

`func (o *ProjectArchiveParams) SetImportExecutions(v bool)`

SetImportExecutions sets ImportExecutions field to given value.

### HasImportExecutions

`func (o *ProjectArchiveParams) HasImportExecutions() bool`

HasImportExecutions returns a boolean if a field has been set.

### GetImportConfig

`func (o *ProjectArchiveParams) GetImportConfig() bool`

GetImportConfig returns the ImportConfig field if non-nil, zero value otherwise.

### GetImportConfigOk

`func (o *ProjectArchiveParams) GetImportConfigOk() (*bool, bool)`

GetImportConfigOk returns a tuple with the ImportConfig field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportConfig

`func (o *ProjectArchiveParams) SetImportConfig(v bool)`

SetImportConfig sets ImportConfig field to given value.

### HasImportConfig

`func (o *ProjectArchiveParams) HasImportConfig() bool`

HasImportConfig returns a boolean if a field has been set.

### GetImportNodesSources

`func (o *ProjectArchiveParams) GetImportNodesSources() bool`

GetImportNodesSources returns the ImportNodesSources field if non-nil, zero value otherwise.

### GetImportNodesSourcesOk

`func (o *ProjectArchiveParams) GetImportNodesSourcesOk() (*bool, bool)`

GetImportNodesSourcesOk returns a tuple with the ImportNodesSources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportNodesSources

`func (o *ProjectArchiveParams) SetImportNodesSources(v bool)`

SetImportNodesSources sets ImportNodesSources field to given value.

### HasImportNodesSources

`func (o *ProjectArchiveParams) HasImportNodesSources() bool`

HasImportNodesSources returns a boolean if a field has been set.

### GetImportACL

`func (o *ProjectArchiveParams) GetImportACL() bool`

GetImportACL returns the ImportACL field if non-nil, zero value otherwise.

### GetImportACLOk

`func (o *ProjectArchiveParams) GetImportACLOk() (*bool, bool)`

GetImportACLOk returns a tuple with the ImportACL field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportACL

`func (o *ProjectArchiveParams) SetImportACL(v bool)`

SetImportACL sets ImportACL field to given value.

### HasImportACL

`func (o *ProjectArchiveParams) HasImportACL() bool`

HasImportACL returns a boolean if a field has been set.

### GetImportScm

`func (o *ProjectArchiveParams) GetImportScm() bool`

GetImportScm returns the ImportScm field if non-nil, zero value otherwise.

### GetImportScmOk

`func (o *ProjectArchiveParams) GetImportScmOk() (*bool, bool)`

GetImportScmOk returns a tuple with the ImportScm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportScm

`func (o *ProjectArchiveParams) SetImportScm(v bool)`

SetImportScm sets ImportScm field to given value.

### HasImportScm

`func (o *ProjectArchiveParams) HasImportScm() bool`

HasImportScm returns a boolean if a field has been set.

### GetValidateJobref

`func (o *ProjectArchiveParams) GetValidateJobref() bool`

GetValidateJobref returns the ValidateJobref field if non-nil, zero value otherwise.

### GetValidateJobrefOk

`func (o *ProjectArchiveParams) GetValidateJobrefOk() (*bool, bool)`

GetValidateJobrefOk returns a tuple with the ValidateJobref field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValidateJobref

`func (o *ProjectArchiveParams) SetValidateJobref(v bool)`

SetValidateJobref sets ValidateJobref field to given value.

### HasValidateJobref

`func (o *ProjectArchiveParams) HasValidateJobref() bool`

HasValidateJobref returns a boolean if a field has been set.

### GetExportAll

`func (o *ProjectArchiveParams) GetExportAll() bool`

GetExportAll returns the ExportAll field if non-nil, zero value otherwise.

### GetExportAllOk

`func (o *ProjectArchiveParams) GetExportAllOk() (*bool, bool)`

GetExportAllOk returns a tuple with the ExportAll field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportAll

`func (o *ProjectArchiveParams) SetExportAll(v bool)`

SetExportAll sets ExportAll field to given value.

### HasExportAll

`func (o *ProjectArchiveParams) HasExportAll() bool`

HasExportAll returns a boolean if a field has been set.

### GetExportJobs

`func (o *ProjectArchiveParams) GetExportJobs() bool`

GetExportJobs returns the ExportJobs field if non-nil, zero value otherwise.

### GetExportJobsOk

`func (o *ProjectArchiveParams) GetExportJobsOk() (*bool, bool)`

GetExportJobsOk returns a tuple with the ExportJobs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportJobs

`func (o *ProjectArchiveParams) SetExportJobs(v bool)`

SetExportJobs sets ExportJobs field to given value.

### HasExportJobs

`func (o *ProjectArchiveParams) HasExportJobs() bool`

HasExportJobs returns a boolean if a field has been set.

### GetExportExecutions

`func (o *ProjectArchiveParams) GetExportExecutions() bool`

GetExportExecutions returns the ExportExecutions field if non-nil, zero value otherwise.

### GetExportExecutionsOk

`func (o *ProjectArchiveParams) GetExportExecutionsOk() (*bool, bool)`

GetExportExecutionsOk returns a tuple with the ExportExecutions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportExecutions

`func (o *ProjectArchiveParams) SetExportExecutions(v bool)`

SetExportExecutions sets ExportExecutions field to given value.

### HasExportExecutions

`func (o *ProjectArchiveParams) HasExportExecutions() bool`

HasExportExecutions returns a boolean if a field has been set.

### GetExportConfigs

`func (o *ProjectArchiveParams) GetExportConfigs() bool`

GetExportConfigs returns the ExportConfigs field if non-nil, zero value otherwise.

### GetExportConfigsOk

`func (o *ProjectArchiveParams) GetExportConfigsOk() (*bool, bool)`

GetExportConfigsOk returns a tuple with the ExportConfigs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportConfigs

`func (o *ProjectArchiveParams) SetExportConfigs(v bool)`

SetExportConfigs sets ExportConfigs field to given value.

### HasExportConfigs

`func (o *ProjectArchiveParams) HasExportConfigs() bool`

HasExportConfigs returns a boolean if a field has been set.

### GetExportReadmes

`func (o *ProjectArchiveParams) GetExportReadmes() bool`

GetExportReadmes returns the ExportReadmes field if non-nil, zero value otherwise.

### GetExportReadmesOk

`func (o *ProjectArchiveParams) GetExportReadmesOk() (*bool, bool)`

GetExportReadmesOk returns a tuple with the ExportReadmes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportReadmes

`func (o *ProjectArchiveParams) SetExportReadmes(v bool)`

SetExportReadmes sets ExportReadmes field to given value.

### HasExportReadmes

`func (o *ProjectArchiveParams) HasExportReadmes() bool`

HasExportReadmes returns a boolean if a field has been set.

### GetExportAcls

`func (o *ProjectArchiveParams) GetExportAcls() bool`

GetExportAcls returns the ExportAcls field if non-nil, zero value otherwise.

### GetExportAclsOk

`func (o *ProjectArchiveParams) GetExportAclsOk() (*bool, bool)`

GetExportAclsOk returns a tuple with the ExportAcls field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportAcls

`func (o *ProjectArchiveParams) SetExportAcls(v bool)`

SetExportAcls sets ExportAcls field to given value.

### HasExportAcls

`func (o *ProjectArchiveParams) HasExportAcls() bool`

HasExportAcls returns a boolean if a field has been set.

### GetExportScm

`func (o *ProjectArchiveParams) GetExportScm() bool`

GetExportScm returns the ExportScm field if non-nil, zero value otherwise.

### GetExportScmOk

`func (o *ProjectArchiveParams) GetExportScmOk() (*bool, bool)`

GetExportScmOk returns a tuple with the ExportScm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportScm

`func (o *ProjectArchiveParams) SetExportScm(v bool)`

SetExportScm sets ExportScm field to given value.

### HasExportScm

`func (o *ProjectArchiveParams) HasExportScm() bool`

HasExportScm returns a boolean if a field has been set.

### GetImportComponents

`func (o *ProjectArchiveParams) GetImportComponents() map[string]bool`

GetImportComponents returns the ImportComponents field if non-nil, zero value otherwise.

### GetImportComponentsOk

`func (o *ProjectArchiveParams) GetImportComponentsOk() (*map[string]bool, bool)`

GetImportComponentsOk returns a tuple with the ImportComponents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportComponents

`func (o *ProjectArchiveParams) SetImportComponents(v map[string]bool)`

SetImportComponents sets ImportComponents field to given value.

### HasImportComponents

`func (o *ProjectArchiveParams) HasImportComponents() bool`

HasImportComponents returns a boolean if a field has been set.

### GetImportOpts

`func (o *ProjectArchiveParams) GetImportOpts() map[string]map[string]string`

GetImportOpts returns the ImportOpts field if non-nil, zero value otherwise.

### GetImportOptsOk

`func (o *ProjectArchiveParams) GetImportOptsOk() (*map[string]map[string]string, bool)`

GetImportOptsOk returns a tuple with the ImportOpts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportOpts

`func (o *ProjectArchiveParams) SetImportOpts(v map[string]map[string]string)`

SetImportOpts sets ImportOpts field to given value.

### HasImportOpts

`func (o *ProjectArchiveParams) HasImportOpts() bool`

HasImportOpts returns a boolean if a field has been set.

### GetExportComponents

`func (o *ProjectArchiveParams) GetExportComponents() map[string]bool`

GetExportComponents returns the ExportComponents field if non-nil, zero value otherwise.

### GetExportComponentsOk

`func (o *ProjectArchiveParams) GetExportComponentsOk() (*map[string]bool, bool)`

GetExportComponentsOk returns a tuple with the ExportComponents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportComponents

`func (o *ProjectArchiveParams) SetExportComponents(v map[string]bool)`

SetExportComponents sets ExportComponents field to given value.

### HasExportComponents

`func (o *ProjectArchiveParams) HasExportComponents() bool`

HasExportComponents returns a boolean if a field has been set.

### GetExportOpts

`func (o *ProjectArchiveParams) GetExportOpts() map[string]map[string]string`

GetExportOpts returns the ExportOpts field if non-nil, zero value otherwise.

### GetExportOptsOk

`func (o *ProjectArchiveParams) GetExportOptsOk() (*map[string]map[string]string, bool)`

GetExportOptsOk returns a tuple with the ExportOpts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportOpts

`func (o *ProjectArchiveParams) SetExportOpts(v map[string]map[string]string)`

SetExportOpts sets ExportOpts field to given value.

### HasExportOpts

`func (o *ProjectArchiveParams) HasExportOpts() bool`

HasExportOpts returns a boolean if a field has been set.

### GetStripJobRef

`func (o *ProjectArchiveParams) GetStripJobRef() string`

GetStripJobRef returns the StripJobRef field if non-nil, zero value otherwise.

### GetStripJobRefOk

`func (o *ProjectArchiveParams) GetStripJobRefOk() (*string, bool)`

GetStripJobRefOk returns a tuple with the StripJobRef field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripJobRef

`func (o *ProjectArchiveParams) SetStripJobRef(v string)`

SetStripJobRef sets StripJobRef field to given value.

### HasStripJobRef

`func (o *ProjectArchiveParams) HasStripJobRef() bool`

HasStripJobRef returns a boolean if a field has been set.

### GetTargetproject

`func (o *ProjectArchiveParams) GetTargetproject() string`

GetTargetproject returns the Targetproject field if non-nil, zero value otherwise.

### GetTargetprojectOk

`func (o *ProjectArchiveParams) GetTargetprojectOk() (*string, bool)`

GetTargetprojectOk returns a tuple with the Targetproject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetproject

`func (o *ProjectArchiveParams) SetTargetproject(v string)`

SetTargetproject sets Targetproject field to given value.

### HasTargetproject

`func (o *ProjectArchiveParams) HasTargetproject() bool`

HasTargetproject returns a boolean if a field has been set.

### GetApitoken

`func (o *ProjectArchiveParams) GetApitoken() string`

GetApitoken returns the Apitoken field if non-nil, zero value otherwise.

### GetApitokenOk

`func (o *ProjectArchiveParams) GetApitokenOk() (*string, bool)`

GetApitokenOk returns a tuple with the Apitoken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApitoken

`func (o *ProjectArchiveParams) SetApitoken(v string)`

SetApitoken sets Apitoken field to given value.

### HasApitoken

`func (o *ProjectArchiveParams) HasApitoken() bool`

HasApitoken returns a boolean if a field has been set.

### GetUrl

`func (o *ProjectArchiveParams) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ProjectArchiveParams) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ProjectArchiveParams) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *ProjectArchiveParams) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetPreserveuuid

`func (o *ProjectArchiveParams) GetPreserveuuid() bool`

GetPreserveuuid returns the Preserveuuid field if non-nil, zero value otherwise.

### GetPreserveuuidOk

`func (o *ProjectArchiveParams) GetPreserveuuidOk() (*bool, bool)`

GetPreserveuuidOk returns a tuple with the Preserveuuid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreserveuuid

`func (o *ProjectArchiveParams) SetPreserveuuid(v bool)`

SetPreserveuuid sets Preserveuuid field to given value.

### HasPreserveuuid

`func (o *ProjectArchiveParams) HasPreserveuuid() bool`

HasPreserveuuid returns a boolean if a field has been set.

### GetAsyncImport

`func (o *ProjectArchiveParams) GetAsyncImport() bool`

GetAsyncImport returns the AsyncImport field if non-nil, zero value otherwise.

### GetAsyncImportOk

`func (o *ProjectArchiveParams) GetAsyncImportOk() (*bool, bool)`

GetAsyncImportOk returns a tuple with the AsyncImport field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsyncImport

`func (o *ProjectArchiveParams) SetAsyncImport(v bool)`

SetAsyncImport sets AsyncImport field to given value.

### HasAsyncImport

`func (o *ProjectArchiveParams) HasAsyncImport() bool`

HasAsyncImport returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



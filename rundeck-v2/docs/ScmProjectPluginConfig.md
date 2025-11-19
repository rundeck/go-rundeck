# ScmProjectPluginConfig

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Integration** | Pointer to **string** |  | [optional] 
**Project** | Pointer to **string** | project name | [optional] 
**Type** | Pointer to **string** | plugin type name | [optional] 
**Enabled** | Pointer to **bool** |  | [optional] 
**Config** | Pointer to **map[string]string** |  set of key/value pairs for the configuration | [optional] 

## Methods

### NewScmProjectPluginConfig

`func NewScmProjectPluginConfig() *ScmProjectPluginConfig`

NewScmProjectPluginConfig instantiates a new ScmProjectPluginConfig object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmProjectPluginConfigWithDefaults

`func NewScmProjectPluginConfigWithDefaults() *ScmProjectPluginConfig`

NewScmProjectPluginConfigWithDefaults instantiates a new ScmProjectPluginConfig object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIntegration

`func (o *ScmProjectPluginConfig) GetIntegration() string`

GetIntegration returns the Integration field if non-nil, zero value otherwise.

### GetIntegrationOk

`func (o *ScmProjectPluginConfig) GetIntegrationOk() (*string, bool)`

GetIntegrationOk returns a tuple with the Integration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegration

`func (o *ScmProjectPluginConfig) SetIntegration(v string)`

SetIntegration sets Integration field to given value.

### HasIntegration

`func (o *ScmProjectPluginConfig) HasIntegration() bool`

HasIntegration returns a boolean if a field has been set.

### GetProject

`func (o *ScmProjectPluginConfig) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *ScmProjectPluginConfig) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *ScmProjectPluginConfig) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *ScmProjectPluginConfig) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetType

`func (o *ScmProjectPluginConfig) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ScmProjectPluginConfig) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ScmProjectPluginConfig) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ScmProjectPluginConfig) HasType() bool`

HasType returns a boolean if a field has been set.

### GetEnabled

`func (o *ScmProjectPluginConfig) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *ScmProjectPluginConfig) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *ScmProjectPluginConfig) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *ScmProjectPluginConfig) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetConfig

`func (o *ScmProjectPluginConfig) GetConfig() map[string]string`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *ScmProjectPluginConfig) GetConfigOk() (*map[string]string, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *ScmProjectPluginConfig) SetConfig(v map[string]string)`

SetConfig sets Config field to given value.

### HasConfig

`func (o *ScmProjectPluginConfig) HasConfig() bool`

HasConfig returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ScmPluginList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Integration** | Pointer to **string** |  | [optional] 
**Plugins** | Pointer to [**[]ScmPluginDescription**](ScmPluginDescription.md) |  | [optional] 

## Methods

### NewScmPluginList

`func NewScmPluginList() *ScmPluginList`

NewScmPluginList instantiates a new ScmPluginList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmPluginListWithDefaults

`func NewScmPluginListWithDefaults() *ScmPluginList`

NewScmPluginListWithDefaults instantiates a new ScmPluginList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIntegration

`func (o *ScmPluginList) GetIntegration() string`

GetIntegration returns the Integration field if non-nil, zero value otherwise.

### GetIntegrationOk

`func (o *ScmPluginList) GetIntegrationOk() (*string, bool)`

GetIntegrationOk returns a tuple with the Integration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegration

`func (o *ScmPluginList) SetIntegration(v string)`

SetIntegration sets Integration field to given value.

### HasIntegration

`func (o *ScmPluginList) HasIntegration() bool`

HasIntegration returns a boolean if a field has been set.

### GetPlugins

`func (o *ScmPluginList) GetPlugins() []ScmPluginDescription`

GetPlugins returns the Plugins field if non-nil, zero value otherwise.

### GetPluginsOk

`func (o *ScmPluginList) GetPluginsOk() (*[]ScmPluginDescription, bool)`

GetPluginsOk returns a tuple with the Plugins field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlugins

`func (o *ScmPluginList) SetPlugins(v []ScmPluginDescription)`

SetPlugins sets Plugins field to given value.

### HasPlugins

`func (o *ScmPluginList) HasPlugins() bool`

HasPlugins returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



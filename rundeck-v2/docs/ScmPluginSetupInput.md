# ScmPluginSetupInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** |  | [optional] 
**Integration** | Pointer to **string** |  | [optional] 
**Fields** | Pointer to [**[]ScmPluginInputField**](ScmPluginInputField.md) |  | [optional] 

## Methods

### NewScmPluginSetupInput

`func NewScmPluginSetupInput() *ScmPluginSetupInput`

NewScmPluginSetupInput instantiates a new ScmPluginSetupInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmPluginSetupInputWithDefaults

`func NewScmPluginSetupInputWithDefaults() *ScmPluginSetupInput`

NewScmPluginSetupInputWithDefaults instantiates a new ScmPluginSetupInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *ScmPluginSetupInput) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ScmPluginSetupInput) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ScmPluginSetupInput) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ScmPluginSetupInput) HasType() bool`

HasType returns a boolean if a field has been set.

### GetIntegration

`func (o *ScmPluginSetupInput) GetIntegration() string`

GetIntegration returns the Integration field if non-nil, zero value otherwise.

### GetIntegrationOk

`func (o *ScmPluginSetupInput) GetIntegrationOk() (*string, bool)`

GetIntegrationOk returns a tuple with the Integration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegration

`func (o *ScmPluginSetupInput) SetIntegration(v string)`

SetIntegration sets Integration field to given value.

### HasIntegration

`func (o *ScmPluginSetupInput) HasIntegration() bool`

HasIntegration returns a boolean if a field has been set.

### GetFields

`func (o *ScmPluginSetupInput) GetFields() []ScmPluginInputField`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *ScmPluginSetupInput) GetFieldsOk() (*[]ScmPluginInputField, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *ScmPluginSetupInput) SetFields(v []ScmPluginInputField)`

SetFields sets Fields field to given value.

### HasFields

`func (o *ScmPluginSetupInput) HasFields() bool`

HasFields returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



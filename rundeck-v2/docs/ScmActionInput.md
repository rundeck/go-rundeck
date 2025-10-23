# ScmActionInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ActionId** | Pointer to **string** | ID for the action | [optional] 
**Integration** | Pointer to **string** |  | [optional] 
**Title** | Pointer to **string** | Display title for the action | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Fields** | Pointer to [**[]ScmPluginInputField**](ScmPluginInputField.md) |  | [optional] 
**ImportItems** | Pointer to [**[]ScmImportActionItem**](ScmImportActionItem.md) |  | [optional] 
**ExportItems** | Pointer to [**[]ScmExportActionItem**](ScmExportActionItem.md) |  | [optional] 

## Methods

### NewScmActionInput

`func NewScmActionInput() *ScmActionInput`

NewScmActionInput instantiates a new ScmActionInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmActionInputWithDefaults

`func NewScmActionInputWithDefaults() *ScmActionInput`

NewScmActionInputWithDefaults instantiates a new ScmActionInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActionId

`func (o *ScmActionInput) GetActionId() string`

GetActionId returns the ActionId field if non-nil, zero value otherwise.

### GetActionIdOk

`func (o *ScmActionInput) GetActionIdOk() (*string, bool)`

GetActionIdOk returns a tuple with the ActionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionId

`func (o *ScmActionInput) SetActionId(v string)`

SetActionId sets ActionId field to given value.

### HasActionId

`func (o *ScmActionInput) HasActionId() bool`

HasActionId returns a boolean if a field has been set.

### GetIntegration

`func (o *ScmActionInput) GetIntegration() string`

GetIntegration returns the Integration field if non-nil, zero value otherwise.

### GetIntegrationOk

`func (o *ScmActionInput) GetIntegrationOk() (*string, bool)`

GetIntegrationOk returns a tuple with the Integration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegration

`func (o *ScmActionInput) SetIntegration(v string)`

SetIntegration sets Integration field to given value.

### HasIntegration

`func (o *ScmActionInput) HasIntegration() bool`

HasIntegration returns a boolean if a field has been set.

### GetTitle

`func (o *ScmActionInput) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ScmActionInput) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ScmActionInput) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ScmActionInput) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetDescription

`func (o *ScmActionInput) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ScmActionInput) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ScmActionInput) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ScmActionInput) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetFields

`func (o *ScmActionInput) GetFields() []ScmPluginInputField`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *ScmActionInput) GetFieldsOk() (*[]ScmPluginInputField, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *ScmActionInput) SetFields(v []ScmPluginInputField)`

SetFields sets Fields field to given value.

### HasFields

`func (o *ScmActionInput) HasFields() bool`

HasFields returns a boolean if a field has been set.

### GetImportItems

`func (o *ScmActionInput) GetImportItems() []ScmImportActionItem`

GetImportItems returns the ImportItems field if non-nil, zero value otherwise.

### GetImportItemsOk

`func (o *ScmActionInput) GetImportItemsOk() (*[]ScmImportActionItem, bool)`

GetImportItemsOk returns a tuple with the ImportItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportItems

`func (o *ScmActionInput) SetImportItems(v []ScmImportActionItem)`

SetImportItems sets ImportItems field to given value.

### HasImportItems

`func (o *ScmActionInput) HasImportItems() bool`

HasImportItems returns a boolean if a field has been set.

### GetExportItems

`func (o *ScmActionInput) GetExportItems() []ScmExportActionItem`

GetExportItems returns the ExportItems field if non-nil, zero value otherwise.

### GetExportItemsOk

`func (o *ScmActionInput) GetExportItemsOk() (*[]ScmExportActionItem, bool)`

GetExportItemsOk returns a tuple with the ExportItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportItems

`func (o *ScmActionInput) SetExportItems(v []ScmExportActionItem)`

SetExportItems sets ExportItems field to given value.

### HasExportItems

`func (o *ScmActionInput) HasExportItems() bool`

HasExportItems returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



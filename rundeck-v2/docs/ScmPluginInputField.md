# ScmPluginInputField

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | Pointer to **string** | display title for the field | [optional] 
**Name** | Pointer to **string** | identifier for the field, used when submitting the input values | [optional] 
**Description** | Pointer to **string** | textual description | [optional] 
**Type** | Pointer to **string** | data type of the field: &#x60;String&#x60;, &#x60;Integer&#x60;, &#x60;Select&#x60; (multi-value), &#x60;FreeSelect&#x60; (open-ended multi-value), &#x60;Boolean&#x60; (true/false) | [optional] 
**Required** | Pointer to **bool** | whether the input is required | [optional] 
**DefaultValue** | Pointer to **string** | a default value if the input does not specify one | [optional] 
**Values** | Pointer to **[]string** | if the type is &#x60;Select&#x60; or &#x60;FreeSelect&#x60;, a list of string values to choose from | [optional] 
**Scope** | Pointer to **string** |  | [optional] 
**RenderingOptions** | Pointer to **map[string]string** | a key/value map of options, such as declaring that GUI display the input as a password field. | [optional] 

## Methods

### NewScmPluginInputField

`func NewScmPluginInputField() *ScmPluginInputField`

NewScmPluginInputField instantiates a new ScmPluginInputField object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmPluginInputFieldWithDefaults

`func NewScmPluginInputFieldWithDefaults() *ScmPluginInputField`

NewScmPluginInputFieldWithDefaults instantiates a new ScmPluginInputField object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *ScmPluginInputField) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ScmPluginInputField) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ScmPluginInputField) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ScmPluginInputField) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetName

`func (o *ScmPluginInputField) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ScmPluginInputField) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ScmPluginInputField) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ScmPluginInputField) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *ScmPluginInputField) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ScmPluginInputField) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ScmPluginInputField) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ScmPluginInputField) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetType

`func (o *ScmPluginInputField) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ScmPluginInputField) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ScmPluginInputField) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ScmPluginInputField) HasType() bool`

HasType returns a boolean if a field has been set.

### GetRequired

`func (o *ScmPluginInputField) GetRequired() bool`

GetRequired returns the Required field if non-nil, zero value otherwise.

### GetRequiredOk

`func (o *ScmPluginInputField) GetRequiredOk() (*bool, bool)`

GetRequiredOk returns a tuple with the Required field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequired

`func (o *ScmPluginInputField) SetRequired(v bool)`

SetRequired sets Required field to given value.

### HasRequired

`func (o *ScmPluginInputField) HasRequired() bool`

HasRequired returns a boolean if a field has been set.

### GetDefaultValue

`func (o *ScmPluginInputField) GetDefaultValue() string`

GetDefaultValue returns the DefaultValue field if non-nil, zero value otherwise.

### GetDefaultValueOk

`func (o *ScmPluginInputField) GetDefaultValueOk() (*string, bool)`

GetDefaultValueOk returns a tuple with the DefaultValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultValue

`func (o *ScmPluginInputField) SetDefaultValue(v string)`

SetDefaultValue sets DefaultValue field to given value.

### HasDefaultValue

`func (o *ScmPluginInputField) HasDefaultValue() bool`

HasDefaultValue returns a boolean if a field has been set.

### GetValues

`func (o *ScmPluginInputField) GetValues() []string`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *ScmPluginInputField) GetValuesOk() (*[]string, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *ScmPluginInputField) SetValues(v []string)`

SetValues sets Values field to given value.

### HasValues

`func (o *ScmPluginInputField) HasValues() bool`

HasValues returns a boolean if a field has been set.

### GetScope

`func (o *ScmPluginInputField) GetScope() string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *ScmPluginInputField) GetScopeOk() (*string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *ScmPluginInputField) SetScope(v string)`

SetScope sets Scope field to given value.

### HasScope

`func (o *ScmPluginInputField) HasScope() bool`

HasScope returns a boolean if a field has been set.

### GetRenderingOptions

`func (o *ScmPluginInputField) GetRenderingOptions() map[string]string`

GetRenderingOptions returns the RenderingOptions field if non-nil, zero value otherwise.

### GetRenderingOptionsOk

`func (o *ScmPluginInputField) GetRenderingOptionsOk() (*map[string]string, bool)`

GetRenderingOptionsOk returns a tuple with the RenderingOptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenderingOptions

`func (o *ScmPluginInputField) SetRenderingOptions(v map[string]string)`

SetRenderingOptions sets RenderingOptions field to given value.

### HasRenderingOptions

`func (o *ScmPluginInputField) HasRenderingOptions() bool`

HasRenderingOptions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



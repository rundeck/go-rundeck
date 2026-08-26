# TypeResource

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | Resource Type | 
**Specifier** | Pointer to **string** | Type Specifier | [optional] 

## Methods

### NewTypeResource

`func NewTypeResource(type_ string, ) *TypeResource`

NewTypeResource instantiates a new TypeResource object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTypeResourceWithDefaults

`func NewTypeResourceWithDefaults() *TypeResource`

NewTypeResourceWithDefaults instantiates a new TypeResource object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *TypeResource) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *TypeResource) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *TypeResource) SetType(v string)`

SetType sets Type field to given value.


### GetSpecifier

`func (o *TypeResource) GetSpecifier() string`

GetSpecifier returns the Specifier field if non-nil, zero value otherwise.

### GetSpecifierOk

`func (o *TypeResource) GetSpecifierOk() (*string, bool)`

GetSpecifierOk returns a tuple with the Specifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecifier

`func (o *TypeResource) SetSpecifier(v string)`

SetSpecifier sets Specifier field to given value.

### HasSpecifier

`func (o *TypeResource) HasSpecifier() bool`

HasSpecifier returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



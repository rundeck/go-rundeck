# UserClassList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Classes** | Pointer to [**[]UserClassDefinition**](UserClassDefinition.md) |  | [optional] 

## Methods

### NewUserClassList

`func NewUserClassList() *UserClassList`

NewUserClassList instantiates a new UserClassList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserClassListWithDefaults

`func NewUserClassListWithDefaults() *UserClassList`

NewUserClassListWithDefaults instantiates a new UserClassList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetClasses

`func (o *UserClassList) GetClasses() []UserClassDefinition`

GetClasses returns the Classes field if non-nil, zero value otherwise.

### GetClassesOk

`func (o *UserClassList) GetClassesOk() (*[]UserClassDefinition, bool)`

GetClassesOk returns a tuple with the Classes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClasses

`func (o *UserClassList) SetClasses(v []UserClassDefinition)`

SetClasses sets Classes field to given value.

### HasClasses

`func (o *UserClassList) HasClasses() bool`

HasClasses returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



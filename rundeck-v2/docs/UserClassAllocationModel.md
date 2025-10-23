# UserClassAllocationModel

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Allocations** | Pointer to **map[string]string** | The current User Class allocation set, as a map of user name to user class name. | [optional] 

## Methods

### NewUserClassAllocationModel

`func NewUserClassAllocationModel() *UserClassAllocationModel`

NewUserClassAllocationModel instantiates a new UserClassAllocationModel object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserClassAllocationModelWithDefaults

`func NewUserClassAllocationModelWithDefaults() *UserClassAllocationModel`

NewUserClassAllocationModelWithDefaults instantiates a new UserClassAllocationModel object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAllocations

`func (o *UserClassAllocationModel) GetAllocations() map[string]string`

GetAllocations returns the Allocations field if non-nil, zero value otherwise.

### GetAllocationsOk

`func (o *UserClassAllocationModel) GetAllocationsOk() (*map[string]string, bool)`

GetAllocationsOk returns a tuple with the Allocations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllocations

`func (o *UserClassAllocationModel) SetAllocations(v map[string]string)`

SetAllocations sets Allocations field to given value.

### HasAllocations

`func (o *UserClassAllocationModel) HasAllocations() bool`

HasAllocations returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



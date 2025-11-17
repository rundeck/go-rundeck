# UserClassAllocationChange

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Allocations** | Pointer to **map[string]string** | The current User Class allocation set, as a map of user name to user class name. | [optional] 
**Usernames** | Pointer to **[]string** |  | [optional] 
**BulkAssign** | Pointer to **string** |  | [optional] 
**BulkRemove** | Pointer to **bool** |  | [optional] 

## Methods

### NewUserClassAllocationChange

`func NewUserClassAllocationChange() *UserClassAllocationChange`

NewUserClassAllocationChange instantiates a new UserClassAllocationChange object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserClassAllocationChangeWithDefaults

`func NewUserClassAllocationChangeWithDefaults() *UserClassAllocationChange`

NewUserClassAllocationChangeWithDefaults instantiates a new UserClassAllocationChange object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAllocations

`func (o *UserClassAllocationChange) GetAllocations() map[string]string`

GetAllocations returns the Allocations field if non-nil, zero value otherwise.

### GetAllocationsOk

`func (o *UserClassAllocationChange) GetAllocationsOk() (*map[string]string, bool)`

GetAllocationsOk returns a tuple with the Allocations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllocations

`func (o *UserClassAllocationChange) SetAllocations(v map[string]string)`

SetAllocations sets Allocations field to given value.

### HasAllocations

`func (o *UserClassAllocationChange) HasAllocations() bool`

HasAllocations returns a boolean if a field has been set.

### GetUsernames

`func (o *UserClassAllocationChange) GetUsernames() []string`

GetUsernames returns the Usernames field if non-nil, zero value otherwise.

### GetUsernamesOk

`func (o *UserClassAllocationChange) GetUsernamesOk() (*[]string, bool)`

GetUsernamesOk returns a tuple with the Usernames field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsernames

`func (o *UserClassAllocationChange) SetUsernames(v []string)`

SetUsernames sets Usernames field to given value.

### HasUsernames

`func (o *UserClassAllocationChange) HasUsernames() bool`

HasUsernames returns a boolean if a field has been set.

### GetBulkAssign

`func (o *UserClassAllocationChange) GetBulkAssign() string`

GetBulkAssign returns the BulkAssign field if non-nil, zero value otherwise.

### GetBulkAssignOk

`func (o *UserClassAllocationChange) GetBulkAssignOk() (*string, bool)`

GetBulkAssignOk returns a tuple with the BulkAssign field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBulkAssign

`func (o *UserClassAllocationChange) SetBulkAssign(v string)`

SetBulkAssign sets BulkAssign field to given value.

### HasBulkAssign

`func (o *UserClassAllocationChange) HasBulkAssign() bool`

HasBulkAssign returns a boolean if a field has been set.

### GetBulkRemove

`func (o *UserClassAllocationChange) GetBulkRemove() bool`

GetBulkRemove returns the BulkRemove field if non-nil, zero value otherwise.

### GetBulkRemoveOk

`func (o *UserClassAllocationChange) GetBulkRemoveOk() (*bool, bool)`

GetBulkRemoveOk returns a tuple with the BulkRemove field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBulkRemove

`func (o *UserClassAllocationChange) SetBulkRemove(v bool)`

SetBulkRemove sets BulkRemove field to given value.

### HasBulkRemove

`func (o *UserClassAllocationChange) HasBulkRemove() bool`

HasBulkRemove returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



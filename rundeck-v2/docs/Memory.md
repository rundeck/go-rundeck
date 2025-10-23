# Memory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Unit** | Pointer to **string** |  | [optional] 
**Max** | Pointer to **int64** |  | [optional] 
**Free** | Pointer to **int64** |  | [optional] 
**Total** | Pointer to **int64** |  | [optional] 

## Methods

### NewMemory

`func NewMemory() *Memory`

NewMemory instantiates a new Memory object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMemoryWithDefaults

`func NewMemoryWithDefaults() *Memory`

NewMemoryWithDefaults instantiates a new Memory object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUnit

`func (o *Memory) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *Memory) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *Memory) SetUnit(v string)`

SetUnit sets Unit field to given value.

### HasUnit

`func (o *Memory) HasUnit() bool`

HasUnit returns a boolean if a field has been set.

### GetMax

`func (o *Memory) GetMax() int64`

GetMax returns the Max field if non-nil, zero value otherwise.

### GetMaxOk

`func (o *Memory) GetMaxOk() (*int64, bool)`

GetMaxOk returns a tuple with the Max field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMax

`func (o *Memory) SetMax(v int64)`

SetMax sets Max field to given value.

### HasMax

`func (o *Memory) HasMax() bool`

HasMax returns a boolean if a field has been set.

### GetFree

`func (o *Memory) GetFree() int64`

GetFree returns the Free field if non-nil, zero value otherwise.

### GetFreeOk

`func (o *Memory) GetFreeOk() (*int64, bool)`

GetFreeOk returns a tuple with the Free field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFree

`func (o *Memory) SetFree(v int64)`

SetFree sets Free field to given value.

### HasFree

`func (o *Memory) HasFree() bool`

HasFree returns a boolean if a field has been set.

### GetTotal

`func (o *Memory) GetTotal() int64`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *Memory) GetTotalOk() (*int64, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *Memory) SetTotal(v int64)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *Memory) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



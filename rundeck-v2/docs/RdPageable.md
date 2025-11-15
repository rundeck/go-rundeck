# RdPageable

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Offset** | Pointer to **int32** |  | [optional] 
**Errors** | Pointer to [**Errors**](Errors.md) |  | [optional] 
**Max** | Pointer to **int32** |  | [optional] 
**SortOrders** | Pointer to [**[]SortOrder**](SortOrder.md) |  | [optional] 

## Methods

### NewRdPageable

`func NewRdPageable() *RdPageable`

NewRdPageable instantiates a new RdPageable object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRdPageableWithDefaults

`func NewRdPageableWithDefaults() *RdPageable`

NewRdPageableWithDefaults instantiates a new RdPageable object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOffset

`func (o *RdPageable) GetOffset() int32`

GetOffset returns the Offset field if non-nil, zero value otherwise.

### GetOffsetOk

`func (o *RdPageable) GetOffsetOk() (*int32, bool)`

GetOffsetOk returns a tuple with the Offset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOffset

`func (o *RdPageable) SetOffset(v int32)`

SetOffset sets Offset field to given value.

### HasOffset

`func (o *RdPageable) HasOffset() bool`

HasOffset returns a boolean if a field has been set.

### GetErrors

`func (o *RdPageable) GetErrors() Errors`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *RdPageable) GetErrorsOk() (*Errors, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *RdPageable) SetErrors(v Errors)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *RdPageable) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetMax

`func (o *RdPageable) GetMax() int32`

GetMax returns the Max field if non-nil, zero value otherwise.

### GetMaxOk

`func (o *RdPageable) GetMaxOk() (*int32, bool)`

GetMaxOk returns a tuple with the Max field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMax

`func (o *RdPageable) SetMax(v int32)`

SetMax sets Max field to given value.

### HasMax

`func (o *RdPageable) HasMax() bool`

HasMax returns a boolean if a field has been set.

### GetSortOrders

`func (o *RdPageable) GetSortOrders() []SortOrder`

GetSortOrders returns the SortOrders field if non-nil, zero value otherwise.

### GetSortOrdersOk

`func (o *RdPageable) GetSortOrdersOk() (*[]SortOrder, bool)`

GetSortOrdersOk returns a tuple with the SortOrders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrders

`func (o *RdPageable) SetSortOrders(v []SortOrder)`

SetSortOrders sets SortOrders field to given value.

### HasSortOrders

`func (o *RdPageable) HasSortOrders() bool`

HasSortOrders returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



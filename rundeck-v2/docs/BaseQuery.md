# BaseQuery

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Max** | Pointer to **int32** |  | [optional] 
**Offset** | Pointer to **int32** |  | [optional] 
**SortBy** | Pointer to **string** |  | [optional] 
**SortOrder** | Pointer to **string** |  | [optional] 

## Methods

### NewBaseQuery

`func NewBaseQuery() *BaseQuery`

NewBaseQuery instantiates a new BaseQuery object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBaseQueryWithDefaults

`func NewBaseQueryWithDefaults() *BaseQuery`

NewBaseQueryWithDefaults instantiates a new BaseQuery object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMax

`func (o *BaseQuery) GetMax() int32`

GetMax returns the Max field if non-nil, zero value otherwise.

### GetMaxOk

`func (o *BaseQuery) GetMaxOk() (*int32, bool)`

GetMaxOk returns a tuple with the Max field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMax

`func (o *BaseQuery) SetMax(v int32)`

SetMax sets Max field to given value.

### HasMax

`func (o *BaseQuery) HasMax() bool`

HasMax returns a boolean if a field has been set.

### GetOffset

`func (o *BaseQuery) GetOffset() int32`

GetOffset returns the Offset field if non-nil, zero value otherwise.

### GetOffsetOk

`func (o *BaseQuery) GetOffsetOk() (*int32, bool)`

GetOffsetOk returns a tuple with the Offset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOffset

`func (o *BaseQuery) SetOffset(v int32)`

SetOffset sets Offset field to given value.

### HasOffset

`func (o *BaseQuery) HasOffset() bool`

HasOffset returns a boolean if a field has been set.

### GetSortBy

`func (o *BaseQuery) GetSortBy() string`

GetSortBy returns the SortBy field if non-nil, zero value otherwise.

### GetSortByOk

`func (o *BaseQuery) GetSortByOk() (*string, bool)`

GetSortByOk returns a tuple with the SortBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortBy

`func (o *BaseQuery) SetSortBy(v string)`

SetSortBy sets SortBy field to given value.

### HasSortBy

`func (o *BaseQuery) HasSortBy() bool`

HasSortBy returns a boolean if a field has been set.

### GetSortOrder

`func (o *BaseQuery) GetSortOrder() string`

GetSortOrder returns the SortOrder field if non-nil, zero value otherwise.

### GetSortOrderOk

`func (o *BaseQuery) GetSortOrderOk() (*string, bool)`

GetSortOrderOk returns a tuple with the SortOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrder

`func (o *BaseQuery) SetSortOrder(v string)`

SetSortOrder sets SortOrder field to given value.

### HasSortOrder

`func (o *BaseQuery) HasSortOrder() bool`

HasSortOrder returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



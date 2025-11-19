# SortOrder

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Column** | Pointer to **string** |  | [optional] 
**Direction** | Pointer to **string** |  | [optional] 

## Methods

### NewSortOrder

`func NewSortOrder() *SortOrder`

NewSortOrder instantiates a new SortOrder object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSortOrderWithDefaults

`func NewSortOrderWithDefaults() *SortOrder`

NewSortOrderWithDefaults instantiates a new SortOrder object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetColumn

`func (o *SortOrder) GetColumn() string`

GetColumn returns the Column field if non-nil, zero value otherwise.

### GetColumnOk

`func (o *SortOrder) GetColumnOk() (*string, bool)`

GetColumnOk returns a tuple with the Column field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColumn

`func (o *SortOrder) SetColumn(v string)`

SetColumn sets Column field to given value.

### HasColumn

`func (o *SortOrder) HasColumn() bool`

HasColumn returns a boolean if a field has been set.

### GetDirection

`func (o *SortOrder) GetDirection() string`

GetDirection returns the Direction field if non-nil, zero value otherwise.

### GetDirectionOk

`func (o *SortOrder) GetDirectionOk() (*string, bool)`

GetDirectionOk returns a tuple with the Direction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDirection

`func (o *SortOrder) SetDirection(v string)`

SetDirection sets Direction field to given value.

### HasDirection

`func (o *SortOrder) HasDirection() bool`

HasDirection returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



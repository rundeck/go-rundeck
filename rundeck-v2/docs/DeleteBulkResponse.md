# DeleteBulkResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RequestCount** | Pointer to **int32** | number of requested execution deletions | [optional] 
**Allsuccessful** | Pointer to **bool** | true if all deletions were successful | [optional] 
**SuccessCount** | Pointer to **int32** | number of deletion attempts that succeeded | [optional] 
**FailedCount** | Pointer to **int32** | number of deletion attempts that failed | [optional] 
**Failures** | Pointer to [**[]FailedItem**](FailedItem.md) |  | [optional] 

## Methods

### NewDeleteBulkResponse

`func NewDeleteBulkResponse() *DeleteBulkResponse`

NewDeleteBulkResponse instantiates a new DeleteBulkResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeleteBulkResponseWithDefaults

`func NewDeleteBulkResponseWithDefaults() *DeleteBulkResponse`

NewDeleteBulkResponseWithDefaults instantiates a new DeleteBulkResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRequestCount

`func (o *DeleteBulkResponse) GetRequestCount() int32`

GetRequestCount returns the RequestCount field if non-nil, zero value otherwise.

### GetRequestCountOk

`func (o *DeleteBulkResponse) GetRequestCountOk() (*int32, bool)`

GetRequestCountOk returns a tuple with the RequestCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequestCount

`func (o *DeleteBulkResponse) SetRequestCount(v int32)`

SetRequestCount sets RequestCount field to given value.

### HasRequestCount

`func (o *DeleteBulkResponse) HasRequestCount() bool`

HasRequestCount returns a boolean if a field has been set.

### GetAllsuccessful

`func (o *DeleteBulkResponse) GetAllsuccessful() bool`

GetAllsuccessful returns the Allsuccessful field if non-nil, zero value otherwise.

### GetAllsuccessfulOk

`func (o *DeleteBulkResponse) GetAllsuccessfulOk() (*bool, bool)`

GetAllsuccessfulOk returns a tuple with the Allsuccessful field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllsuccessful

`func (o *DeleteBulkResponse) SetAllsuccessful(v bool)`

SetAllsuccessful sets Allsuccessful field to given value.

### HasAllsuccessful

`func (o *DeleteBulkResponse) HasAllsuccessful() bool`

HasAllsuccessful returns a boolean if a field has been set.

### GetSuccessCount

`func (o *DeleteBulkResponse) GetSuccessCount() int32`

GetSuccessCount returns the SuccessCount field if non-nil, zero value otherwise.

### GetSuccessCountOk

`func (o *DeleteBulkResponse) GetSuccessCountOk() (*int32, bool)`

GetSuccessCountOk returns a tuple with the SuccessCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccessCount

`func (o *DeleteBulkResponse) SetSuccessCount(v int32)`

SetSuccessCount sets SuccessCount field to given value.

### HasSuccessCount

`func (o *DeleteBulkResponse) HasSuccessCount() bool`

HasSuccessCount returns a boolean if a field has been set.

### GetFailedCount

`func (o *DeleteBulkResponse) GetFailedCount() int32`

GetFailedCount returns the FailedCount field if non-nil, zero value otherwise.

### GetFailedCountOk

`func (o *DeleteBulkResponse) GetFailedCountOk() (*int32, bool)`

GetFailedCountOk returns a tuple with the FailedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailedCount

`func (o *DeleteBulkResponse) SetFailedCount(v int32)`

SetFailedCount sets FailedCount field to given value.

### HasFailedCount

`func (o *DeleteBulkResponse) HasFailedCount() bool`

HasFailedCount returns a boolean if a field has been set.

### GetFailures

`func (o *DeleteBulkResponse) GetFailures() []FailedItem`

GetFailures returns the Failures field if non-nil, zero value otherwise.

### GetFailuresOk

`func (o *DeleteBulkResponse) GetFailuresOk() (*[]FailedItem, bool)`

GetFailuresOk returns a tuple with the Failures field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailures

`func (o *DeleteBulkResponse) SetFailures(v []FailedItem)`

SetFailures sets Failures field to given value.

### HasFailures

`func (o *DeleteBulkResponse) HasFailures() bool`

HasFailures returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ApiBulkJobDeleteRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Ids** | Pointer to **[]string** |  | [optional] 
**Idlist** | Pointer to **string** |  | [optional] 
**Id** | Pointer to **string** |  | [optional] 
**Errors** | Pointer to [**Errors**](Errors.md) |  | [optional] 

## Methods

### NewApiBulkJobDeleteRequest

`func NewApiBulkJobDeleteRequest() *ApiBulkJobDeleteRequest`

NewApiBulkJobDeleteRequest instantiates a new ApiBulkJobDeleteRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiBulkJobDeleteRequestWithDefaults

`func NewApiBulkJobDeleteRequestWithDefaults() *ApiBulkJobDeleteRequest`

NewApiBulkJobDeleteRequestWithDefaults instantiates a new ApiBulkJobDeleteRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIds

`func (o *ApiBulkJobDeleteRequest) GetIds() []string`

GetIds returns the Ids field if non-nil, zero value otherwise.

### GetIdsOk

`func (o *ApiBulkJobDeleteRequest) GetIdsOk() (*[]string, bool)`

GetIdsOk returns a tuple with the Ids field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIds

`func (o *ApiBulkJobDeleteRequest) SetIds(v []string)`

SetIds sets Ids field to given value.

### HasIds

`func (o *ApiBulkJobDeleteRequest) HasIds() bool`

HasIds returns a boolean if a field has been set.

### GetIdlist

`func (o *ApiBulkJobDeleteRequest) GetIdlist() string`

GetIdlist returns the Idlist field if non-nil, zero value otherwise.

### GetIdlistOk

`func (o *ApiBulkJobDeleteRequest) GetIdlistOk() (*string, bool)`

GetIdlistOk returns a tuple with the Idlist field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIdlist

`func (o *ApiBulkJobDeleteRequest) SetIdlist(v string)`

SetIdlist sets Idlist field to given value.

### HasIdlist

`func (o *ApiBulkJobDeleteRequest) HasIdlist() bool`

HasIdlist returns a boolean if a field has been set.

### GetId

`func (o *ApiBulkJobDeleteRequest) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApiBulkJobDeleteRequest) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApiBulkJobDeleteRequest) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *ApiBulkJobDeleteRequest) HasId() bool`

HasId returns a boolean if a field has been set.

### GetErrors

`func (o *ApiBulkJobDeleteRequest) GetErrors() Errors`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *ApiBulkJobDeleteRequest) GetErrorsOk() (*Errors, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *ApiBulkJobDeleteRequest) SetErrors(v Errors)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *ApiBulkJobDeleteRequest) HasErrors() bool`

HasErrors returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Timestamp

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Epoch** | Pointer to **int64** |  | [optional] 
**Unit** | Pointer to **string** |  | [optional] 
**Datetime** | Pointer to **string** |  | [optional] 

## Methods

### NewTimestamp

`func NewTimestamp() *Timestamp`

NewTimestamp instantiates a new Timestamp object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTimestampWithDefaults

`func NewTimestampWithDefaults() *Timestamp`

NewTimestampWithDefaults instantiates a new Timestamp object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEpoch

`func (o *Timestamp) GetEpoch() int64`

GetEpoch returns the Epoch field if non-nil, zero value otherwise.

### GetEpochOk

`func (o *Timestamp) GetEpochOk() (*int64, bool)`

GetEpochOk returns a tuple with the Epoch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpoch

`func (o *Timestamp) SetEpoch(v int64)`

SetEpoch sets Epoch field to given value.

### HasEpoch

`func (o *Timestamp) HasEpoch() bool`

HasEpoch returns a boolean if a field has been set.

### GetUnit

`func (o *Timestamp) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *Timestamp) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *Timestamp) SetUnit(v string)`

SetUnit sets Unit field to given value.

### HasUnit

`func (o *Timestamp) HasUnit() bool`

HasUnit returns a boolean if a field has been set.

### GetDatetime

`func (o *Timestamp) GetDatetime() string`

GetDatetime returns the Datetime field if non-nil, zero value otherwise.

### GetDatetimeOk

`func (o *Timestamp) GetDatetimeOk() (*string, bool)`

GetDatetimeOk returns a tuple with the Datetime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDatetime

`func (o *Timestamp) SetDatetime(v string)`

SetDatetime sets Datetime field to given value.

### HasDatetime

`func (o *Timestamp) HasDatetime() bool`

HasDatetime returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



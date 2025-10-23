# Uptime

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Duration** | Pointer to **int32** |  | [optional] 
**Unit** | Pointer to **string** |  | [optional] 
**Since** | Pointer to [**Since**](Since.md) |  | [optional] 

## Methods

### NewUptime

`func NewUptime() *Uptime`

NewUptime instantiates a new Uptime object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUptimeWithDefaults

`func NewUptimeWithDefaults() *Uptime`

NewUptimeWithDefaults instantiates a new Uptime object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDuration

`func (o *Uptime) GetDuration() int32`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *Uptime) GetDurationOk() (*int32, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *Uptime) SetDuration(v int32)`

SetDuration sets Duration field to given value.

### HasDuration

`func (o *Uptime) HasDuration() bool`

HasDuration returns a boolean if a field has been set.

### GetUnit

`func (o *Uptime) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *Uptime) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *Uptime) SetUnit(v string)`

SetUnit sets Unit field to given value.

### HasUnit

`func (o *Uptime) HasUnit() bool`

HasUnit returns a boolean if a field has been set.

### GetSince

`func (o *Uptime) GetSince() Since`

GetSince returns the Since field if non-nil, zero value otherwise.

### GetSinceOk

`func (o *Uptime) GetSinceOk() (*Since, bool)`

GetSinceOk returns a tuple with the Since field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSince

`func (o *Uptime) SetSince(v Since)`

SetSince sets Since field to given value.

### HasSince

`func (o *Uptime) HasSince() bool`

HasSince returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



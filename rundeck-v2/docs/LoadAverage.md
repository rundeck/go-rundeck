# LoadAverage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Unit** | Pointer to **string** |  | [optional] 
**Average** | Pointer to **int32** |  | [optional] 

## Methods

### NewLoadAverage

`func NewLoadAverage() *LoadAverage`

NewLoadAverage instantiates a new LoadAverage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLoadAverageWithDefaults

`func NewLoadAverageWithDefaults() *LoadAverage`

NewLoadAverageWithDefaults instantiates a new LoadAverage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUnit

`func (o *LoadAverage) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *LoadAverage) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *LoadAverage) SetUnit(v string)`

SetUnit sets Unit field to given value.

### HasUnit

`func (o *LoadAverage) HasUnit() bool`

HasUnit returns a boolean if a field has been set.

### GetAverage

`func (o *LoadAverage) GetAverage() int32`

GetAverage returns the Average field if non-nil, zero value otherwise.

### GetAverageOk

`func (o *LoadAverage) GetAverageOk() (*int32, bool)`

GetAverageOk returns a tuple with the Average field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAverage

`func (o *LoadAverage) SetAverage(v int32)`

SetAverage sets Average field to given value.

### HasAverage

`func (o *LoadAverage) HasAverage() bool`

HasAverage returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



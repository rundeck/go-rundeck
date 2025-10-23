# Cpu

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LoadAverage** | Pointer to [**LoadAverage**](LoadAverage.md) |  | [optional] 
**Processors** | Pointer to **int32** |  | [optional] 

## Methods

### NewCpu

`func NewCpu() *Cpu`

NewCpu instantiates a new Cpu object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCpuWithDefaults

`func NewCpuWithDefaults() *Cpu`

NewCpuWithDefaults instantiates a new Cpu object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLoadAverage

`func (o *Cpu) GetLoadAverage() LoadAverage`

GetLoadAverage returns the LoadAverage field if non-nil, zero value otherwise.

### GetLoadAverageOk

`func (o *Cpu) GetLoadAverageOk() (*LoadAverage, bool)`

GetLoadAverageOk returns a tuple with the LoadAverage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLoadAverage

`func (o *Cpu) SetLoadAverage(v LoadAverage)`

SetLoadAverage sets LoadAverage field to given value.

### HasLoadAverage

`func (o *Cpu) HasLoadAverage() bool`

HasLoadAverage returns a boolean if a field has been set.

### GetProcessors

`func (o *Cpu) GetProcessors() int32`

GetProcessors returns the Processors field if non-nil, zero value otherwise.

### GetProcessorsOk

`func (o *Cpu) GetProcessorsOk() (*int32, bool)`

GetProcessorsOk returns a tuple with the Processors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProcessors

`func (o *Cpu) SetProcessors(v int32)`

SetProcessors sets Processors field to given value.

### HasProcessors

`func (o *Cpu) HasProcessors() bool`

HasProcessors returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



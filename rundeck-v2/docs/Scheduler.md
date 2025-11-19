# Scheduler

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Running** | Pointer to **int32** |  | [optional] 
**ThreadPoolSize** | Pointer to **int32** |  | [optional] 

## Methods

### NewScheduler

`func NewScheduler() *Scheduler`

NewScheduler instantiates a new Scheduler object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSchedulerWithDefaults

`func NewSchedulerWithDefaults() *Scheduler`

NewSchedulerWithDefaults instantiates a new Scheduler object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRunning

`func (o *Scheduler) GetRunning() int32`

GetRunning returns the Running field if non-nil, zero value otherwise.

### GetRunningOk

`func (o *Scheduler) GetRunningOk() (*int32, bool)`

GetRunningOk returns a tuple with the Running field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunning

`func (o *Scheduler) SetRunning(v int32)`

SetRunning sets Running field to given value.

### HasRunning

`func (o *Scheduler) HasRunning() bool`

HasRunning returns a boolean if a field has been set.

### GetThreadPoolSize

`func (o *Scheduler) GetThreadPoolSize() int32`

GetThreadPoolSize returns the ThreadPoolSize field if non-nil, zero value otherwise.

### GetThreadPoolSizeOk

`func (o *Scheduler) GetThreadPoolSizeOk() (*int32, bool)`

GetThreadPoolSizeOk returns a tuple with the ThreadPoolSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreadPoolSize

`func (o *Scheduler) SetThreadPoolSize(v int32)`

SetThreadPoolSize sets ThreadPoolSize field to given value.

### HasThreadPoolSize

`func (o *Scheduler) HasThreadPoolSize() bool`

HasThreadPoolSize returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



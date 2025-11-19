# Stats

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Uptime** | Pointer to [**Uptime**](Uptime.md) |  | [optional] 
**Cpu** | Pointer to [**Cpu**](Cpu.md) |  | [optional] 
**Memory** | Pointer to [**Memory**](Memory.md) |  | [optional] 
**Scheduler** | Pointer to [**Scheduler**](Scheduler.md) |  | [optional] 
**Threads** | Pointer to [**Threads**](Threads.md) |  | [optional] 

## Methods

### NewStats

`func NewStats() *Stats`

NewStats instantiates a new Stats object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStatsWithDefaults

`func NewStatsWithDefaults() *Stats`

NewStatsWithDefaults instantiates a new Stats object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUptime

`func (o *Stats) GetUptime() Uptime`

GetUptime returns the Uptime field if non-nil, zero value otherwise.

### GetUptimeOk

`func (o *Stats) GetUptimeOk() (*Uptime, bool)`

GetUptimeOk returns a tuple with the Uptime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUptime

`func (o *Stats) SetUptime(v Uptime)`

SetUptime sets Uptime field to given value.

### HasUptime

`func (o *Stats) HasUptime() bool`

HasUptime returns a boolean if a field has been set.

### GetCpu

`func (o *Stats) GetCpu() Cpu`

GetCpu returns the Cpu field if non-nil, zero value otherwise.

### GetCpuOk

`func (o *Stats) GetCpuOk() (*Cpu, bool)`

GetCpuOk returns a tuple with the Cpu field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCpu

`func (o *Stats) SetCpu(v Cpu)`

SetCpu sets Cpu field to given value.

### HasCpu

`func (o *Stats) HasCpu() bool`

HasCpu returns a boolean if a field has been set.

### GetMemory

`func (o *Stats) GetMemory() Memory`

GetMemory returns the Memory field if non-nil, zero value otherwise.

### GetMemoryOk

`func (o *Stats) GetMemoryOk() (*Memory, bool)`

GetMemoryOk returns a tuple with the Memory field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemory

`func (o *Stats) SetMemory(v Memory)`

SetMemory sets Memory field to given value.

### HasMemory

`func (o *Stats) HasMemory() bool`

HasMemory returns a boolean if a field has been set.

### GetScheduler

`func (o *Stats) GetScheduler() Scheduler`

GetScheduler returns the Scheduler field if non-nil, zero value otherwise.

### GetSchedulerOk

`func (o *Stats) GetSchedulerOk() (*Scheduler, bool)`

GetSchedulerOk returns a tuple with the Scheduler field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScheduler

`func (o *Stats) SetScheduler(v Scheduler)`

SetScheduler sets Scheduler field to given value.

### HasScheduler

`func (o *Stats) HasScheduler() bool`

HasScheduler returns a boolean if a field has been set.

### GetThreads

`func (o *Stats) GetThreads() Threads`

GetThreads returns the Threads field if non-nil, zero value otherwise.

### GetThreadsOk

`func (o *Stats) GetThreadsOk() (*Threads, bool)`

GetThreadsOk returns a tuple with the Threads field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreads

`func (o *Stats) SetThreads(v Threads)`

SetThreads sets Threads field to given value.

### HasThreads

`func (o *Stats) HasThreads() bool`

HasThreads returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



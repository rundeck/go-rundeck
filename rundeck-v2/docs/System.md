# System

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Timestamp** | Pointer to [**Timestamp**](Timestamp.md) |  | [optional] 
**Rundeck** | Pointer to [**Rundeck**](Rundeck.md) |  | [optional] 
**Executions** | Pointer to [**Executions**](Executions.md) |  | [optional] 
**Os** | Pointer to [**Os**](Os.md) |  | [optional] 
**Jvm** | Pointer to [**Jvm**](Jvm.md) |  | [optional] 
**Stats** | Pointer to [**Stats**](Stats.md) |  | [optional] 
**Metrics** | Pointer to [**Metrics**](Metrics.md) |  | [optional] 
**ThreadDump** | Pointer to [**ThreadDump**](ThreadDump.md) |  | [optional] 
**Healthcheck** | Pointer to [**Healthcheck**](Healthcheck.md) |  | [optional] 
**Ping** | Pointer to [**Ping**](Ping.md) |  | [optional] 
**Extended** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewSystem

`func NewSystem() *System`

NewSystem instantiates a new System object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSystemWithDefaults

`func NewSystemWithDefaults() *System`

NewSystemWithDefaults instantiates a new System object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTimestamp

`func (o *System) GetTimestamp() Timestamp`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *System) GetTimestampOk() (*Timestamp, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *System) SetTimestamp(v Timestamp)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *System) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetRundeck

`func (o *System) GetRundeck() Rundeck`

GetRundeck returns the Rundeck field if non-nil, zero value otherwise.

### GetRundeckOk

`func (o *System) GetRundeckOk() (*Rundeck, bool)`

GetRundeckOk returns a tuple with the Rundeck field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRundeck

`func (o *System) SetRundeck(v Rundeck)`

SetRundeck sets Rundeck field to given value.

### HasRundeck

`func (o *System) HasRundeck() bool`

HasRundeck returns a boolean if a field has been set.

### GetExecutions

`func (o *System) GetExecutions() Executions`

GetExecutions returns the Executions field if non-nil, zero value otherwise.

### GetExecutionsOk

`func (o *System) GetExecutionsOk() (*Executions, bool)`

GetExecutionsOk returns a tuple with the Executions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutions

`func (o *System) SetExecutions(v Executions)`

SetExecutions sets Executions field to given value.

### HasExecutions

`func (o *System) HasExecutions() bool`

HasExecutions returns a boolean if a field has been set.

### GetOs

`func (o *System) GetOs() Os`

GetOs returns the Os field if non-nil, zero value otherwise.

### GetOsOk

`func (o *System) GetOsOk() (*Os, bool)`

GetOsOk returns a tuple with the Os field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOs

`func (o *System) SetOs(v Os)`

SetOs sets Os field to given value.

### HasOs

`func (o *System) HasOs() bool`

HasOs returns a boolean if a field has been set.

### GetJvm

`func (o *System) GetJvm() Jvm`

GetJvm returns the Jvm field if non-nil, zero value otherwise.

### GetJvmOk

`func (o *System) GetJvmOk() (*Jvm, bool)`

GetJvmOk returns a tuple with the Jvm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJvm

`func (o *System) SetJvm(v Jvm)`

SetJvm sets Jvm field to given value.

### HasJvm

`func (o *System) HasJvm() bool`

HasJvm returns a boolean if a field has been set.

### GetStats

`func (o *System) GetStats() Stats`

GetStats returns the Stats field if non-nil, zero value otherwise.

### GetStatsOk

`func (o *System) GetStatsOk() (*Stats, bool)`

GetStatsOk returns a tuple with the Stats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStats

`func (o *System) SetStats(v Stats)`

SetStats sets Stats field to given value.

### HasStats

`func (o *System) HasStats() bool`

HasStats returns a boolean if a field has been set.

### GetMetrics

`func (o *System) GetMetrics() Metrics`

GetMetrics returns the Metrics field if non-nil, zero value otherwise.

### GetMetricsOk

`func (o *System) GetMetricsOk() (*Metrics, bool)`

GetMetricsOk returns a tuple with the Metrics field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetrics

`func (o *System) SetMetrics(v Metrics)`

SetMetrics sets Metrics field to given value.

### HasMetrics

`func (o *System) HasMetrics() bool`

HasMetrics returns a boolean if a field has been set.

### GetThreadDump

`func (o *System) GetThreadDump() ThreadDump`

GetThreadDump returns the ThreadDump field if non-nil, zero value otherwise.

### GetThreadDumpOk

`func (o *System) GetThreadDumpOk() (*ThreadDump, bool)`

GetThreadDumpOk returns a tuple with the ThreadDump field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreadDump

`func (o *System) SetThreadDump(v ThreadDump)`

SetThreadDump sets ThreadDump field to given value.

### HasThreadDump

`func (o *System) HasThreadDump() bool`

HasThreadDump returns a boolean if a field has been set.

### GetHealthcheck

`func (o *System) GetHealthcheck() Healthcheck`

GetHealthcheck returns the Healthcheck field if non-nil, zero value otherwise.

### GetHealthcheckOk

`func (o *System) GetHealthcheckOk() (*Healthcheck, bool)`

GetHealthcheckOk returns a tuple with the Healthcheck field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHealthcheck

`func (o *System) SetHealthcheck(v Healthcheck)`

SetHealthcheck sets Healthcheck field to given value.

### HasHealthcheck

`func (o *System) HasHealthcheck() bool`

HasHealthcheck returns a boolean if a field has been set.

### GetPing

`func (o *System) GetPing() Ping`

GetPing returns the Ping field if non-nil, zero value otherwise.

### GetPingOk

`func (o *System) GetPingOk() (*Ping, bool)`

GetPingOk returns a tuple with the Ping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPing

`func (o *System) SetPing(v Ping)`

SetPing sets Ping field to given value.

### HasPing

`func (o *System) HasPing() bool`

HasPing returns a boolean if a field has been set.

### GetExtended

`func (o *System) GetExtended() map[string]interface{}`

GetExtended returns the Extended field if non-nil, zero value otherwise.

### GetExtendedOk

`func (o *System) GetExtendedOk() (*map[string]interface{}, bool)`

GetExtendedOk returns a tuple with the Extended field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtended

`func (o *System) SetExtended(v map[string]interface{})`

SetExtended sets Extended field to given value.

### HasExtended

`func (o *System) HasExtended() bool`

HasExtended returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



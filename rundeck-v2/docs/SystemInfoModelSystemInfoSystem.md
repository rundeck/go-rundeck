# SystemInfoModelSystemInfoSystem

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
**Extended** | Pointer to **map[string]map[string]interface{}** |  | [optional] 

## Methods

### NewSystemInfoModelSystemInfoSystem

`func NewSystemInfoModelSystemInfoSystem() *SystemInfoModelSystemInfoSystem`

NewSystemInfoModelSystemInfoSystem instantiates a new SystemInfoModelSystemInfoSystem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSystemInfoModelSystemInfoSystemWithDefaults

`func NewSystemInfoModelSystemInfoSystemWithDefaults() *SystemInfoModelSystemInfoSystem`

NewSystemInfoModelSystemInfoSystemWithDefaults instantiates a new SystemInfoModelSystemInfoSystem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTimestamp

`func (o *SystemInfoModelSystemInfoSystem) GetTimestamp() Timestamp`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *SystemInfoModelSystemInfoSystem) GetTimestampOk() (*Timestamp, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *SystemInfoModelSystemInfoSystem) SetTimestamp(v Timestamp)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *SystemInfoModelSystemInfoSystem) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetRundeck

`func (o *SystemInfoModelSystemInfoSystem) GetRundeck() Rundeck`

GetRundeck returns the Rundeck field if non-nil, zero value otherwise.

### GetRundeckOk

`func (o *SystemInfoModelSystemInfoSystem) GetRundeckOk() (*Rundeck, bool)`

GetRundeckOk returns a tuple with the Rundeck field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRundeck

`func (o *SystemInfoModelSystemInfoSystem) SetRundeck(v Rundeck)`

SetRundeck sets Rundeck field to given value.

### HasRundeck

`func (o *SystemInfoModelSystemInfoSystem) HasRundeck() bool`

HasRundeck returns a boolean if a field has been set.

### GetExecutions

`func (o *SystemInfoModelSystemInfoSystem) GetExecutions() Executions`

GetExecutions returns the Executions field if non-nil, zero value otherwise.

### GetExecutionsOk

`func (o *SystemInfoModelSystemInfoSystem) GetExecutionsOk() (*Executions, bool)`

GetExecutionsOk returns a tuple with the Executions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutions

`func (o *SystemInfoModelSystemInfoSystem) SetExecutions(v Executions)`

SetExecutions sets Executions field to given value.

### HasExecutions

`func (o *SystemInfoModelSystemInfoSystem) HasExecutions() bool`

HasExecutions returns a boolean if a field has been set.

### GetOs

`func (o *SystemInfoModelSystemInfoSystem) GetOs() Os`

GetOs returns the Os field if non-nil, zero value otherwise.

### GetOsOk

`func (o *SystemInfoModelSystemInfoSystem) GetOsOk() (*Os, bool)`

GetOsOk returns a tuple with the Os field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOs

`func (o *SystemInfoModelSystemInfoSystem) SetOs(v Os)`

SetOs sets Os field to given value.

### HasOs

`func (o *SystemInfoModelSystemInfoSystem) HasOs() bool`

HasOs returns a boolean if a field has been set.

### GetJvm

`func (o *SystemInfoModelSystemInfoSystem) GetJvm() Jvm`

GetJvm returns the Jvm field if non-nil, zero value otherwise.

### GetJvmOk

`func (o *SystemInfoModelSystemInfoSystem) GetJvmOk() (*Jvm, bool)`

GetJvmOk returns a tuple with the Jvm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJvm

`func (o *SystemInfoModelSystemInfoSystem) SetJvm(v Jvm)`

SetJvm sets Jvm field to given value.

### HasJvm

`func (o *SystemInfoModelSystemInfoSystem) HasJvm() bool`

HasJvm returns a boolean if a field has been set.

### GetStats

`func (o *SystemInfoModelSystemInfoSystem) GetStats() Stats`

GetStats returns the Stats field if non-nil, zero value otherwise.

### GetStatsOk

`func (o *SystemInfoModelSystemInfoSystem) GetStatsOk() (*Stats, bool)`

GetStatsOk returns a tuple with the Stats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStats

`func (o *SystemInfoModelSystemInfoSystem) SetStats(v Stats)`

SetStats sets Stats field to given value.

### HasStats

`func (o *SystemInfoModelSystemInfoSystem) HasStats() bool`

HasStats returns a boolean if a field has been set.

### GetMetrics

`func (o *SystemInfoModelSystemInfoSystem) GetMetrics() Metrics`

GetMetrics returns the Metrics field if non-nil, zero value otherwise.

### GetMetricsOk

`func (o *SystemInfoModelSystemInfoSystem) GetMetricsOk() (*Metrics, bool)`

GetMetricsOk returns a tuple with the Metrics field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetrics

`func (o *SystemInfoModelSystemInfoSystem) SetMetrics(v Metrics)`

SetMetrics sets Metrics field to given value.

### HasMetrics

`func (o *SystemInfoModelSystemInfoSystem) HasMetrics() bool`

HasMetrics returns a boolean if a field has been set.

### GetThreadDump

`func (o *SystemInfoModelSystemInfoSystem) GetThreadDump() ThreadDump`

GetThreadDump returns the ThreadDump field if non-nil, zero value otherwise.

### GetThreadDumpOk

`func (o *SystemInfoModelSystemInfoSystem) GetThreadDumpOk() (*ThreadDump, bool)`

GetThreadDumpOk returns a tuple with the ThreadDump field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreadDump

`func (o *SystemInfoModelSystemInfoSystem) SetThreadDump(v ThreadDump)`

SetThreadDump sets ThreadDump field to given value.

### HasThreadDump

`func (o *SystemInfoModelSystemInfoSystem) HasThreadDump() bool`

HasThreadDump returns a boolean if a field has been set.

### GetHealthcheck

`func (o *SystemInfoModelSystemInfoSystem) GetHealthcheck() Healthcheck`

GetHealthcheck returns the Healthcheck field if non-nil, zero value otherwise.

### GetHealthcheckOk

`func (o *SystemInfoModelSystemInfoSystem) GetHealthcheckOk() (*Healthcheck, bool)`

GetHealthcheckOk returns a tuple with the Healthcheck field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHealthcheck

`func (o *SystemInfoModelSystemInfoSystem) SetHealthcheck(v Healthcheck)`

SetHealthcheck sets Healthcheck field to given value.

### HasHealthcheck

`func (o *SystemInfoModelSystemInfoSystem) HasHealthcheck() bool`

HasHealthcheck returns a boolean if a field has been set.

### GetPing

`func (o *SystemInfoModelSystemInfoSystem) GetPing() Ping`

GetPing returns the Ping field if non-nil, zero value otherwise.

### GetPingOk

`func (o *SystemInfoModelSystemInfoSystem) GetPingOk() (*Ping, bool)`

GetPingOk returns a tuple with the Ping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPing

`func (o *SystemInfoModelSystemInfoSystem) SetPing(v Ping)`

SetPing sets Ping field to given value.

### HasPing

`func (o *SystemInfoModelSystemInfoSystem) HasPing() bool`

HasPing returns a boolean if a field has been set.

### GetExtended

`func (o *SystemInfoModelSystemInfoSystem) GetExtended() map[string]map[string]interface{}`

GetExtended returns the Extended field if non-nil, zero value otherwise.

### GetExtendedOk

`func (o *SystemInfoModelSystemInfoSystem) GetExtendedOk() (*map[string]map[string]interface{}, bool)`

GetExtendedOk returns a tuple with the Extended field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtended

`func (o *SystemInfoModelSystemInfoSystem) SetExtended(v map[string]map[string]interface{})`

SetExtended sets Extended field to given value.

### HasExtended

`func (o *SystemInfoModelSystemInfoSystem) HasExtended() bool`

HasExtended returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



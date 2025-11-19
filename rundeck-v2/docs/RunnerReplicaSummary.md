# RunnerReplicaSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReplicaId** | Pointer to **string** | Unique identifier for the Runner replica. | [optional] 
**RunnerId** | Pointer to **string** | Unique identifier for the Runner instance. | [optional] 
**SessionId** | Pointer to **string** | Session identifier for the replica&#39;s current session. | [optional] 
**Status** | Pointer to **string** | Current status of the replica (e.g., active, offline). | [optional] 
**Version** | Pointer to **string** | Version of the Runner software. | [optional] 
**Hostname** | Pointer to **string** | Hostname of the machine running the replica. | [optional] 
**InstallationPath** | Pointer to **string** | Installation path of the Runner on the host machine. | [optional] 
**IpAddress** | Pointer to **string** | IP address of the replica host. | [optional] 
**CreateTime** | Pointer to **time.Time** | Timestamp when the replica was created. | [optional] 
**LastCheckin** | Pointer to **string** | Last check-in time as a formatted string. | [optional] 
**LastCheckinAlert** | Pointer to **bool** | Indicates if the last check-in triggered an alert. | [optional] 
**Uptime** | Pointer to **int64** | Uptime of the replica in milliseconds. | [optional] 
**RunningOperations** | Pointer to **int64** | Number of currently running operations on the replica. | [optional] 
**VersionWarning** | Pointer to **bool** | Indicates if there is a version mismatch warning for the replica. | [optional] 

## Methods

### NewRunnerReplicaSummary

`func NewRunnerReplicaSummary() *RunnerReplicaSummary`

NewRunnerReplicaSummary instantiates a new RunnerReplicaSummary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRunnerReplicaSummaryWithDefaults

`func NewRunnerReplicaSummaryWithDefaults() *RunnerReplicaSummary`

NewRunnerReplicaSummaryWithDefaults instantiates a new RunnerReplicaSummary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReplicaId

`func (o *RunnerReplicaSummary) GetReplicaId() string`

GetReplicaId returns the ReplicaId field if non-nil, zero value otherwise.

### GetReplicaIdOk

`func (o *RunnerReplicaSummary) GetReplicaIdOk() (*string, bool)`

GetReplicaIdOk returns a tuple with the ReplicaId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaId

`func (o *RunnerReplicaSummary) SetReplicaId(v string)`

SetReplicaId sets ReplicaId field to given value.

### HasReplicaId

`func (o *RunnerReplicaSummary) HasReplicaId() bool`

HasReplicaId returns a boolean if a field has been set.

### GetRunnerId

`func (o *RunnerReplicaSummary) GetRunnerId() string`

GetRunnerId returns the RunnerId field if non-nil, zero value otherwise.

### GetRunnerIdOk

`func (o *RunnerReplicaSummary) GetRunnerIdOk() (*string, bool)`

GetRunnerIdOk returns a tuple with the RunnerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerId

`func (o *RunnerReplicaSummary) SetRunnerId(v string)`

SetRunnerId sets RunnerId field to given value.

### HasRunnerId

`func (o *RunnerReplicaSummary) HasRunnerId() bool`

HasRunnerId returns a boolean if a field has been set.

### GetSessionId

`func (o *RunnerReplicaSummary) GetSessionId() string`

GetSessionId returns the SessionId field if non-nil, zero value otherwise.

### GetSessionIdOk

`func (o *RunnerReplicaSummary) GetSessionIdOk() (*string, bool)`

GetSessionIdOk returns a tuple with the SessionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSessionId

`func (o *RunnerReplicaSummary) SetSessionId(v string)`

SetSessionId sets SessionId field to given value.

### HasSessionId

`func (o *RunnerReplicaSummary) HasSessionId() bool`

HasSessionId returns a boolean if a field has been set.

### GetStatus

`func (o *RunnerReplicaSummary) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *RunnerReplicaSummary) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *RunnerReplicaSummary) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *RunnerReplicaSummary) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetVersion

`func (o *RunnerReplicaSummary) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *RunnerReplicaSummary) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *RunnerReplicaSummary) SetVersion(v string)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *RunnerReplicaSummary) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### GetHostname

`func (o *RunnerReplicaSummary) GetHostname() string`

GetHostname returns the Hostname field if non-nil, zero value otherwise.

### GetHostnameOk

`func (o *RunnerReplicaSummary) GetHostnameOk() (*string, bool)`

GetHostnameOk returns a tuple with the Hostname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostname

`func (o *RunnerReplicaSummary) SetHostname(v string)`

SetHostname sets Hostname field to given value.

### HasHostname

`func (o *RunnerReplicaSummary) HasHostname() bool`

HasHostname returns a boolean if a field has been set.

### GetInstallationPath

`func (o *RunnerReplicaSummary) GetInstallationPath() string`

GetInstallationPath returns the InstallationPath field if non-nil, zero value otherwise.

### GetInstallationPathOk

`func (o *RunnerReplicaSummary) GetInstallationPathOk() (*string, bool)`

GetInstallationPathOk returns a tuple with the InstallationPath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstallationPath

`func (o *RunnerReplicaSummary) SetInstallationPath(v string)`

SetInstallationPath sets InstallationPath field to given value.

### HasInstallationPath

`func (o *RunnerReplicaSummary) HasInstallationPath() bool`

HasInstallationPath returns a boolean if a field has been set.

### GetIpAddress

`func (o *RunnerReplicaSummary) GetIpAddress() string`

GetIpAddress returns the IpAddress field if non-nil, zero value otherwise.

### GetIpAddressOk

`func (o *RunnerReplicaSummary) GetIpAddressOk() (*string, bool)`

GetIpAddressOk returns a tuple with the IpAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpAddress

`func (o *RunnerReplicaSummary) SetIpAddress(v string)`

SetIpAddress sets IpAddress field to given value.

### HasIpAddress

`func (o *RunnerReplicaSummary) HasIpAddress() bool`

HasIpAddress returns a boolean if a field has been set.

### GetCreateTime

`func (o *RunnerReplicaSummary) GetCreateTime() time.Time`

GetCreateTime returns the CreateTime field if non-nil, zero value otherwise.

### GetCreateTimeOk

`func (o *RunnerReplicaSummary) GetCreateTimeOk() (*time.Time, bool)`

GetCreateTimeOk returns a tuple with the CreateTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTime

`func (o *RunnerReplicaSummary) SetCreateTime(v time.Time)`

SetCreateTime sets CreateTime field to given value.

### HasCreateTime

`func (o *RunnerReplicaSummary) HasCreateTime() bool`

HasCreateTime returns a boolean if a field has been set.

### GetLastCheckin

`func (o *RunnerReplicaSummary) GetLastCheckin() string`

GetLastCheckin returns the LastCheckin field if non-nil, zero value otherwise.

### GetLastCheckinOk

`func (o *RunnerReplicaSummary) GetLastCheckinOk() (*string, bool)`

GetLastCheckinOk returns a tuple with the LastCheckin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastCheckin

`func (o *RunnerReplicaSummary) SetLastCheckin(v string)`

SetLastCheckin sets LastCheckin field to given value.

### HasLastCheckin

`func (o *RunnerReplicaSummary) HasLastCheckin() bool`

HasLastCheckin returns a boolean if a field has been set.

### GetLastCheckinAlert

`func (o *RunnerReplicaSummary) GetLastCheckinAlert() bool`

GetLastCheckinAlert returns the LastCheckinAlert field if non-nil, zero value otherwise.

### GetLastCheckinAlertOk

`func (o *RunnerReplicaSummary) GetLastCheckinAlertOk() (*bool, bool)`

GetLastCheckinAlertOk returns a tuple with the LastCheckinAlert field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastCheckinAlert

`func (o *RunnerReplicaSummary) SetLastCheckinAlert(v bool)`

SetLastCheckinAlert sets LastCheckinAlert field to given value.

### HasLastCheckinAlert

`func (o *RunnerReplicaSummary) HasLastCheckinAlert() bool`

HasLastCheckinAlert returns a boolean if a field has been set.

### GetUptime

`func (o *RunnerReplicaSummary) GetUptime() int64`

GetUptime returns the Uptime field if non-nil, zero value otherwise.

### GetUptimeOk

`func (o *RunnerReplicaSummary) GetUptimeOk() (*int64, bool)`

GetUptimeOk returns a tuple with the Uptime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUptime

`func (o *RunnerReplicaSummary) SetUptime(v int64)`

SetUptime sets Uptime field to given value.

### HasUptime

`func (o *RunnerReplicaSummary) HasUptime() bool`

HasUptime returns a boolean if a field has been set.

### GetRunningOperations

`func (o *RunnerReplicaSummary) GetRunningOperations() int64`

GetRunningOperations returns the RunningOperations field if non-nil, zero value otherwise.

### GetRunningOperationsOk

`func (o *RunnerReplicaSummary) GetRunningOperationsOk() (*int64, bool)`

GetRunningOperationsOk returns a tuple with the RunningOperations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunningOperations

`func (o *RunnerReplicaSummary) SetRunningOperations(v int64)`

SetRunningOperations sets RunningOperations field to given value.

### HasRunningOperations

`func (o *RunnerReplicaSummary) HasRunningOperations() bool`

HasRunningOperations returns a boolean if a field has been set.

### GetVersionWarning

`func (o *RunnerReplicaSummary) GetVersionWarning() bool`

GetVersionWarning returns the VersionWarning field if non-nil, zero value otherwise.

### GetVersionWarningOk

`func (o *RunnerReplicaSummary) GetVersionWarningOk() (*bool, bool)`

GetVersionWarningOk returns a tuple with the VersionWarning field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionWarning

`func (o *RunnerReplicaSummary) SetVersionWarning(v bool)`

SetVersionWarning sets VersionWarning field to given value.

### HasVersionWarning

`func (o *RunnerReplicaSummary) HasVersionWarning() bool`

HasVersionWarning returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



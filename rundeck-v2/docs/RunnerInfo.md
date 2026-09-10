# RunnerInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**Version** | Pointer to **string** |  | [optional] 
**ProjectAssociations** | Pointer to [**RunnerProjectAssociations**](RunnerProjectAssociations.md) |  | [optional] 
**DateCreated** | Pointer to **time.Time** |  | [optional] 
**LastUpdated** | Pointer to **time.Time** |  | [optional] 
**LastCheckin** | Pointer to **string** |  | [optional] 
**LastCheckinAlert** | Pointer to **bool** |  | [optional] 
**RunningOperations** | Pointer to **int32** | Number of currently running operations on the runner. | [optional] 
**MaxRunningOperations** | Pointer to **int32** | Maximum concurrent operations this runner is configured to handle. | [optional] 
**QueuedOperations** | Pointer to **int32** | Operations waiting in the executor queue. | [optional] 
**CompletedOperations** | Pointer to **int32** | Total operations completed since runner startup. | [optional] 
**Uptime** | Pointer to **int64** |  | [optional] 
**TagNames** | Pointer to **[]string** |  | [optional] 
**RunnerAsNodeEnabled** | Pointer to **bool** |  | [optional] 
**RemoteNodeDispatch** | Pointer to **bool** |  | [optional] 
**RunnerNodeFilter** | Pointer to **string** |  | [optional] 
**Hostname** | Pointer to **string** |  | [optional] 
**OsFamily** | Pointer to **string** |  | [optional] 
**ReplicaType** | Pointer to [**RunnerReplicaType**](RunnerReplicaType.md) |  | [optional] 
**InstallationType** | Pointer to [**RunnerInstallationType**](RunnerInstallationType.md) |  | [optional] 
**ReplicaValidation** | Pointer to [**ReplicaValidationResult**](ReplicaValidationResult.md) |  | [optional] 

## Methods

### NewRunnerInfo

`func NewRunnerInfo() *RunnerInfo`

NewRunnerInfo instantiates a new RunnerInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRunnerInfoWithDefaults

`func NewRunnerInfoWithDefaults() *RunnerInfo`

NewRunnerInfoWithDefaults instantiates a new RunnerInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *RunnerInfo) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *RunnerInfo) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *RunnerInfo) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *RunnerInfo) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *RunnerInfo) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *RunnerInfo) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *RunnerInfo) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *RunnerInfo) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *RunnerInfo) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *RunnerInfo) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *RunnerInfo) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *RunnerInfo) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetStatus

`func (o *RunnerInfo) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *RunnerInfo) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *RunnerInfo) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *RunnerInfo) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetVersion

`func (o *RunnerInfo) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *RunnerInfo) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *RunnerInfo) SetVersion(v string)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *RunnerInfo) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### GetProjectAssociations

`func (o *RunnerInfo) GetProjectAssociations() RunnerProjectAssociations`

GetProjectAssociations returns the ProjectAssociations field if non-nil, zero value otherwise.

### GetProjectAssociationsOk

`func (o *RunnerInfo) GetProjectAssociationsOk() (*RunnerProjectAssociations, bool)`

GetProjectAssociationsOk returns a tuple with the ProjectAssociations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectAssociations

`func (o *RunnerInfo) SetProjectAssociations(v RunnerProjectAssociations)`

SetProjectAssociations sets ProjectAssociations field to given value.

### HasProjectAssociations

`func (o *RunnerInfo) HasProjectAssociations() bool`

HasProjectAssociations returns a boolean if a field has been set.

### GetDateCreated

`func (o *RunnerInfo) GetDateCreated() time.Time`

GetDateCreated returns the DateCreated field if non-nil, zero value otherwise.

### GetDateCreatedOk

`func (o *RunnerInfo) GetDateCreatedOk() (*time.Time, bool)`

GetDateCreatedOk returns a tuple with the DateCreated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateCreated

`func (o *RunnerInfo) SetDateCreated(v time.Time)`

SetDateCreated sets DateCreated field to given value.

### HasDateCreated

`func (o *RunnerInfo) HasDateCreated() bool`

HasDateCreated returns a boolean if a field has been set.

### GetLastUpdated

`func (o *RunnerInfo) GetLastUpdated() time.Time`

GetLastUpdated returns the LastUpdated field if non-nil, zero value otherwise.

### GetLastUpdatedOk

`func (o *RunnerInfo) GetLastUpdatedOk() (*time.Time, bool)`

GetLastUpdatedOk returns a tuple with the LastUpdated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUpdated

`func (o *RunnerInfo) SetLastUpdated(v time.Time)`

SetLastUpdated sets LastUpdated field to given value.

### HasLastUpdated

`func (o *RunnerInfo) HasLastUpdated() bool`

HasLastUpdated returns a boolean if a field has been set.

### GetLastCheckin

`func (o *RunnerInfo) GetLastCheckin() string`

GetLastCheckin returns the LastCheckin field if non-nil, zero value otherwise.

### GetLastCheckinOk

`func (o *RunnerInfo) GetLastCheckinOk() (*string, bool)`

GetLastCheckinOk returns a tuple with the LastCheckin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastCheckin

`func (o *RunnerInfo) SetLastCheckin(v string)`

SetLastCheckin sets LastCheckin field to given value.

### HasLastCheckin

`func (o *RunnerInfo) HasLastCheckin() bool`

HasLastCheckin returns a boolean if a field has been set.

### GetLastCheckinAlert

`func (o *RunnerInfo) GetLastCheckinAlert() bool`

GetLastCheckinAlert returns the LastCheckinAlert field if non-nil, zero value otherwise.

### GetLastCheckinAlertOk

`func (o *RunnerInfo) GetLastCheckinAlertOk() (*bool, bool)`

GetLastCheckinAlertOk returns a tuple with the LastCheckinAlert field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastCheckinAlert

`func (o *RunnerInfo) SetLastCheckinAlert(v bool)`

SetLastCheckinAlert sets LastCheckinAlert field to given value.

### HasLastCheckinAlert

`func (o *RunnerInfo) HasLastCheckinAlert() bool`

HasLastCheckinAlert returns a boolean if a field has been set.

### GetRunningOperations

`func (o *RunnerInfo) GetRunningOperations() int32`

GetRunningOperations returns the RunningOperations field if non-nil, zero value otherwise.

### GetRunningOperationsOk

`func (o *RunnerInfo) GetRunningOperationsOk() (*int32, bool)`

GetRunningOperationsOk returns a tuple with the RunningOperations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunningOperations

`func (o *RunnerInfo) SetRunningOperations(v int32)`

SetRunningOperations sets RunningOperations field to given value.

### HasRunningOperations

`func (o *RunnerInfo) HasRunningOperations() bool`

HasRunningOperations returns a boolean if a field has been set.

### GetMaxRunningOperations

`func (o *RunnerInfo) GetMaxRunningOperations() int32`

GetMaxRunningOperations returns the MaxRunningOperations field if non-nil, zero value otherwise.

### GetMaxRunningOperationsOk

`func (o *RunnerInfo) GetMaxRunningOperationsOk() (*int32, bool)`

GetMaxRunningOperationsOk returns a tuple with the MaxRunningOperations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxRunningOperations

`func (o *RunnerInfo) SetMaxRunningOperations(v int32)`

SetMaxRunningOperations sets MaxRunningOperations field to given value.

### HasMaxRunningOperations

`func (o *RunnerInfo) HasMaxRunningOperations() bool`

HasMaxRunningOperations returns a boolean if a field has been set.

### GetQueuedOperations

`func (o *RunnerInfo) GetQueuedOperations() int32`

GetQueuedOperations returns the QueuedOperations field if non-nil, zero value otherwise.

### GetQueuedOperationsOk

`func (o *RunnerInfo) GetQueuedOperationsOk() (*int32, bool)`

GetQueuedOperationsOk returns a tuple with the QueuedOperations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedOperations

`func (o *RunnerInfo) SetQueuedOperations(v int32)`

SetQueuedOperations sets QueuedOperations field to given value.

### HasQueuedOperations

`func (o *RunnerInfo) HasQueuedOperations() bool`

HasQueuedOperations returns a boolean if a field has been set.

### GetCompletedOperations

`func (o *RunnerInfo) GetCompletedOperations() int32`

GetCompletedOperations returns the CompletedOperations field if non-nil, zero value otherwise.

### GetCompletedOperationsOk

`func (o *RunnerInfo) GetCompletedOperationsOk() (*int32, bool)`

GetCompletedOperationsOk returns a tuple with the CompletedOperations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedOperations

`func (o *RunnerInfo) SetCompletedOperations(v int32)`

SetCompletedOperations sets CompletedOperations field to given value.

### HasCompletedOperations

`func (o *RunnerInfo) HasCompletedOperations() bool`

HasCompletedOperations returns a boolean if a field has been set.

### GetUptime

`func (o *RunnerInfo) GetUptime() int64`

GetUptime returns the Uptime field if non-nil, zero value otherwise.

### GetUptimeOk

`func (o *RunnerInfo) GetUptimeOk() (*int64, bool)`

GetUptimeOk returns a tuple with the Uptime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUptime

`func (o *RunnerInfo) SetUptime(v int64)`

SetUptime sets Uptime field to given value.

### HasUptime

`func (o *RunnerInfo) HasUptime() bool`

HasUptime returns a boolean if a field has been set.

### GetTagNames

`func (o *RunnerInfo) GetTagNames() []string`

GetTagNames returns the TagNames field if non-nil, zero value otherwise.

### GetTagNamesOk

`func (o *RunnerInfo) GetTagNamesOk() (*[]string, bool)`

GetTagNamesOk returns a tuple with the TagNames field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagNames

`func (o *RunnerInfo) SetTagNames(v []string)`

SetTagNames sets TagNames field to given value.

### HasTagNames

`func (o *RunnerInfo) HasTagNames() bool`

HasTagNames returns a boolean if a field has been set.

### GetRunnerAsNodeEnabled

`func (o *RunnerInfo) GetRunnerAsNodeEnabled() bool`

GetRunnerAsNodeEnabled returns the RunnerAsNodeEnabled field if non-nil, zero value otherwise.

### GetRunnerAsNodeEnabledOk

`func (o *RunnerInfo) GetRunnerAsNodeEnabledOk() (*bool, bool)`

GetRunnerAsNodeEnabledOk returns a tuple with the RunnerAsNodeEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerAsNodeEnabled

`func (o *RunnerInfo) SetRunnerAsNodeEnabled(v bool)`

SetRunnerAsNodeEnabled sets RunnerAsNodeEnabled field to given value.

### HasRunnerAsNodeEnabled

`func (o *RunnerInfo) HasRunnerAsNodeEnabled() bool`

HasRunnerAsNodeEnabled returns a boolean if a field has been set.

### GetRemoteNodeDispatch

`func (o *RunnerInfo) GetRemoteNodeDispatch() bool`

GetRemoteNodeDispatch returns the RemoteNodeDispatch field if non-nil, zero value otherwise.

### GetRemoteNodeDispatchOk

`func (o *RunnerInfo) GetRemoteNodeDispatchOk() (*bool, bool)`

GetRemoteNodeDispatchOk returns a tuple with the RemoteNodeDispatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoteNodeDispatch

`func (o *RunnerInfo) SetRemoteNodeDispatch(v bool)`

SetRemoteNodeDispatch sets RemoteNodeDispatch field to given value.

### HasRemoteNodeDispatch

`func (o *RunnerInfo) HasRemoteNodeDispatch() bool`

HasRemoteNodeDispatch returns a boolean if a field has been set.

### GetRunnerNodeFilter

`func (o *RunnerInfo) GetRunnerNodeFilter() string`

GetRunnerNodeFilter returns the RunnerNodeFilter field if non-nil, zero value otherwise.

### GetRunnerNodeFilterOk

`func (o *RunnerInfo) GetRunnerNodeFilterOk() (*string, bool)`

GetRunnerNodeFilterOk returns a tuple with the RunnerNodeFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerNodeFilter

`func (o *RunnerInfo) SetRunnerNodeFilter(v string)`

SetRunnerNodeFilter sets RunnerNodeFilter field to given value.

### HasRunnerNodeFilter

`func (o *RunnerInfo) HasRunnerNodeFilter() bool`

HasRunnerNodeFilter returns a boolean if a field has been set.

### GetHostname

`func (o *RunnerInfo) GetHostname() string`

GetHostname returns the Hostname field if non-nil, zero value otherwise.

### GetHostnameOk

`func (o *RunnerInfo) GetHostnameOk() (*string, bool)`

GetHostnameOk returns a tuple with the Hostname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostname

`func (o *RunnerInfo) SetHostname(v string)`

SetHostname sets Hostname field to given value.

### HasHostname

`func (o *RunnerInfo) HasHostname() bool`

HasHostname returns a boolean if a field has been set.

### GetOsFamily

`func (o *RunnerInfo) GetOsFamily() string`

GetOsFamily returns the OsFamily field if non-nil, zero value otherwise.

### GetOsFamilyOk

`func (o *RunnerInfo) GetOsFamilyOk() (*string, bool)`

GetOsFamilyOk returns a tuple with the OsFamily field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOsFamily

`func (o *RunnerInfo) SetOsFamily(v string)`

SetOsFamily sets OsFamily field to given value.

### HasOsFamily

`func (o *RunnerInfo) HasOsFamily() bool`

HasOsFamily returns a boolean if a field has been set.

### GetReplicaType

`func (o *RunnerInfo) GetReplicaType() RunnerReplicaType`

GetReplicaType returns the ReplicaType field if non-nil, zero value otherwise.

### GetReplicaTypeOk

`func (o *RunnerInfo) GetReplicaTypeOk() (*RunnerReplicaType, bool)`

GetReplicaTypeOk returns a tuple with the ReplicaType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaType

`func (o *RunnerInfo) SetReplicaType(v RunnerReplicaType)`

SetReplicaType sets ReplicaType field to given value.

### HasReplicaType

`func (o *RunnerInfo) HasReplicaType() bool`

HasReplicaType returns a boolean if a field has been set.

### GetInstallationType

`func (o *RunnerInfo) GetInstallationType() RunnerInstallationType`

GetInstallationType returns the InstallationType field if non-nil, zero value otherwise.

### GetInstallationTypeOk

`func (o *RunnerInfo) GetInstallationTypeOk() (*RunnerInstallationType, bool)`

GetInstallationTypeOk returns a tuple with the InstallationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstallationType

`func (o *RunnerInfo) SetInstallationType(v RunnerInstallationType)`

SetInstallationType sets InstallationType field to given value.

### HasInstallationType

`func (o *RunnerInfo) HasInstallationType() bool`

HasInstallationType returns a boolean if a field has been set.

### GetReplicaValidation

`func (o *RunnerInfo) GetReplicaValidation() ReplicaValidationResult`

GetReplicaValidation returns the ReplicaValidation field if non-nil, zero value otherwise.

### GetReplicaValidationOk

`func (o *RunnerInfo) GetReplicaValidationOk() (*ReplicaValidationResult, bool)`

GetReplicaValidationOk returns a tuple with the ReplicaValidation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaValidation

`func (o *RunnerInfo) SetReplicaValidation(v ReplicaValidationResult)`

SetReplicaValidation sets ReplicaValidation field to given value.

### HasReplicaValidation

`func (o *RunnerInfo) HasReplicaValidation() bool`

HasReplicaValidation returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



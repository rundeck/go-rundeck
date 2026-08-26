# RunnerSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**Version** | Pointer to **string** |  | [optional] 
**AssociatedProjects** | Pointer to **int32** |  | [optional] 
**LastCheckin** | Pointer to **string** |  | [optional] 
**RunnerAsNodeEnabled** | Pointer to **bool** |  | [optional] 
**LastCheckinAlert** | Pointer to **bool** |  | [optional] 
**Selected** | Pointer to **bool** |  | [optional] 
**TagNames** | Pointer to **[]string** |  | [optional] 
**UiData** | Pointer to [**UiData**](UiData.md) |  | [optional] 
**RunnerNodeFilter** | Pointer to **string** |  | [optional] 
**RemoteNodeDispatch** | Pointer to **bool** |  | [optional] 
**Hostname** | Pointer to **string** |  | [optional] 
**OsFamily** | Pointer to **string** |  | [optional] 
**ReplicaType** | Pointer to [**RunnerReplicaType**](RunnerReplicaType.md) |  | [optional] 
**InstallationType** | Pointer to [**RunnerInstallationType**](RunnerInstallationType.md) |  | [optional] 
**Providers** | Pointer to [**[]RunnerProviderSummary**](RunnerProviderSummary.md) |  | [optional] 
**RunnerReplicas** | Pointer to **int32** |  | [optional] 
**HealthyRunnerReplicas** | Pointer to **int32** |  | [optional] 
**RunningOperations** | Pointer to **int32** |  | [optional] 
**MaxRunningOperations** | Pointer to **int32** |  | [optional] 
**QueuedOperations** | Pointer to **int32** |  | [optional] 
**CompletedOperations** | Pointer to **int32** |  | [optional] 
**Uptime** | Pointer to **int64** |  | [optional] 
**DateCreated** | Pointer to **time.Time** |  | [optional] 
**LastUpdated** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewRunnerSummary

`func NewRunnerSummary() *RunnerSummary`

NewRunnerSummary instantiates a new RunnerSummary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRunnerSummaryWithDefaults

`func NewRunnerSummaryWithDefaults() *RunnerSummary`

NewRunnerSummaryWithDefaults instantiates a new RunnerSummary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *RunnerSummary) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *RunnerSummary) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *RunnerSummary) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *RunnerSummary) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *RunnerSummary) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *RunnerSummary) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *RunnerSummary) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *RunnerSummary) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *RunnerSummary) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *RunnerSummary) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *RunnerSummary) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *RunnerSummary) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetStatus

`func (o *RunnerSummary) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *RunnerSummary) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *RunnerSummary) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *RunnerSummary) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetVersion

`func (o *RunnerSummary) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *RunnerSummary) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *RunnerSummary) SetVersion(v string)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *RunnerSummary) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### GetAssociatedProjects

`func (o *RunnerSummary) GetAssociatedProjects() int32`

GetAssociatedProjects returns the AssociatedProjects field if non-nil, zero value otherwise.

### GetAssociatedProjectsOk

`func (o *RunnerSummary) GetAssociatedProjectsOk() (*int32, bool)`

GetAssociatedProjectsOk returns a tuple with the AssociatedProjects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssociatedProjects

`func (o *RunnerSummary) SetAssociatedProjects(v int32)`

SetAssociatedProjects sets AssociatedProjects field to given value.

### HasAssociatedProjects

`func (o *RunnerSummary) HasAssociatedProjects() bool`

HasAssociatedProjects returns a boolean if a field has been set.

### GetLastCheckin

`func (o *RunnerSummary) GetLastCheckin() string`

GetLastCheckin returns the LastCheckin field if non-nil, zero value otherwise.

### GetLastCheckinOk

`func (o *RunnerSummary) GetLastCheckinOk() (*string, bool)`

GetLastCheckinOk returns a tuple with the LastCheckin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastCheckin

`func (o *RunnerSummary) SetLastCheckin(v string)`

SetLastCheckin sets LastCheckin field to given value.

### HasLastCheckin

`func (o *RunnerSummary) HasLastCheckin() bool`

HasLastCheckin returns a boolean if a field has been set.

### GetRunnerAsNodeEnabled

`func (o *RunnerSummary) GetRunnerAsNodeEnabled() bool`

GetRunnerAsNodeEnabled returns the RunnerAsNodeEnabled field if non-nil, zero value otherwise.

### GetRunnerAsNodeEnabledOk

`func (o *RunnerSummary) GetRunnerAsNodeEnabledOk() (*bool, bool)`

GetRunnerAsNodeEnabledOk returns a tuple with the RunnerAsNodeEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerAsNodeEnabled

`func (o *RunnerSummary) SetRunnerAsNodeEnabled(v bool)`

SetRunnerAsNodeEnabled sets RunnerAsNodeEnabled field to given value.

### HasRunnerAsNodeEnabled

`func (o *RunnerSummary) HasRunnerAsNodeEnabled() bool`

HasRunnerAsNodeEnabled returns a boolean if a field has been set.

### GetLastCheckinAlert

`func (o *RunnerSummary) GetLastCheckinAlert() bool`

GetLastCheckinAlert returns the LastCheckinAlert field if non-nil, zero value otherwise.

### GetLastCheckinAlertOk

`func (o *RunnerSummary) GetLastCheckinAlertOk() (*bool, bool)`

GetLastCheckinAlertOk returns a tuple with the LastCheckinAlert field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastCheckinAlert

`func (o *RunnerSummary) SetLastCheckinAlert(v bool)`

SetLastCheckinAlert sets LastCheckinAlert field to given value.

### HasLastCheckinAlert

`func (o *RunnerSummary) HasLastCheckinAlert() bool`

HasLastCheckinAlert returns a boolean if a field has been set.

### GetSelected

`func (o *RunnerSummary) GetSelected() bool`

GetSelected returns the Selected field if non-nil, zero value otherwise.

### GetSelectedOk

`func (o *RunnerSummary) GetSelectedOk() (*bool, bool)`

GetSelectedOk returns a tuple with the Selected field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSelected

`func (o *RunnerSummary) SetSelected(v bool)`

SetSelected sets Selected field to given value.

### HasSelected

`func (o *RunnerSummary) HasSelected() bool`

HasSelected returns a boolean if a field has been set.

### GetTagNames

`func (o *RunnerSummary) GetTagNames() []string`

GetTagNames returns the TagNames field if non-nil, zero value otherwise.

### GetTagNamesOk

`func (o *RunnerSummary) GetTagNamesOk() (*[]string, bool)`

GetTagNamesOk returns a tuple with the TagNames field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagNames

`func (o *RunnerSummary) SetTagNames(v []string)`

SetTagNames sets TagNames field to given value.

### HasTagNames

`func (o *RunnerSummary) HasTagNames() bool`

HasTagNames returns a boolean if a field has been set.

### GetUiData

`func (o *RunnerSummary) GetUiData() UiData`

GetUiData returns the UiData field if non-nil, zero value otherwise.

### GetUiDataOk

`func (o *RunnerSummary) GetUiDataOk() (*UiData, bool)`

GetUiDataOk returns a tuple with the UiData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUiData

`func (o *RunnerSummary) SetUiData(v UiData)`

SetUiData sets UiData field to given value.

### HasUiData

`func (o *RunnerSummary) HasUiData() bool`

HasUiData returns a boolean if a field has been set.

### GetRunnerNodeFilter

`func (o *RunnerSummary) GetRunnerNodeFilter() string`

GetRunnerNodeFilter returns the RunnerNodeFilter field if non-nil, zero value otherwise.

### GetRunnerNodeFilterOk

`func (o *RunnerSummary) GetRunnerNodeFilterOk() (*string, bool)`

GetRunnerNodeFilterOk returns a tuple with the RunnerNodeFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerNodeFilter

`func (o *RunnerSummary) SetRunnerNodeFilter(v string)`

SetRunnerNodeFilter sets RunnerNodeFilter field to given value.

### HasRunnerNodeFilter

`func (o *RunnerSummary) HasRunnerNodeFilter() bool`

HasRunnerNodeFilter returns a boolean if a field has been set.

### GetRemoteNodeDispatch

`func (o *RunnerSummary) GetRemoteNodeDispatch() bool`

GetRemoteNodeDispatch returns the RemoteNodeDispatch field if non-nil, zero value otherwise.

### GetRemoteNodeDispatchOk

`func (o *RunnerSummary) GetRemoteNodeDispatchOk() (*bool, bool)`

GetRemoteNodeDispatchOk returns a tuple with the RemoteNodeDispatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoteNodeDispatch

`func (o *RunnerSummary) SetRemoteNodeDispatch(v bool)`

SetRemoteNodeDispatch sets RemoteNodeDispatch field to given value.

### HasRemoteNodeDispatch

`func (o *RunnerSummary) HasRemoteNodeDispatch() bool`

HasRemoteNodeDispatch returns a boolean if a field has been set.

### GetHostname

`func (o *RunnerSummary) GetHostname() string`

GetHostname returns the Hostname field if non-nil, zero value otherwise.

### GetHostnameOk

`func (o *RunnerSummary) GetHostnameOk() (*string, bool)`

GetHostnameOk returns a tuple with the Hostname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostname

`func (o *RunnerSummary) SetHostname(v string)`

SetHostname sets Hostname field to given value.

### HasHostname

`func (o *RunnerSummary) HasHostname() bool`

HasHostname returns a boolean if a field has been set.

### GetOsFamily

`func (o *RunnerSummary) GetOsFamily() string`

GetOsFamily returns the OsFamily field if non-nil, zero value otherwise.

### GetOsFamilyOk

`func (o *RunnerSummary) GetOsFamilyOk() (*string, bool)`

GetOsFamilyOk returns a tuple with the OsFamily field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOsFamily

`func (o *RunnerSummary) SetOsFamily(v string)`

SetOsFamily sets OsFamily field to given value.

### HasOsFamily

`func (o *RunnerSummary) HasOsFamily() bool`

HasOsFamily returns a boolean if a field has been set.

### GetReplicaType

`func (o *RunnerSummary) GetReplicaType() RunnerReplicaType`

GetReplicaType returns the ReplicaType field if non-nil, zero value otherwise.

### GetReplicaTypeOk

`func (o *RunnerSummary) GetReplicaTypeOk() (*RunnerReplicaType, bool)`

GetReplicaTypeOk returns a tuple with the ReplicaType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaType

`func (o *RunnerSummary) SetReplicaType(v RunnerReplicaType)`

SetReplicaType sets ReplicaType field to given value.

### HasReplicaType

`func (o *RunnerSummary) HasReplicaType() bool`

HasReplicaType returns a boolean if a field has been set.

### GetInstallationType

`func (o *RunnerSummary) GetInstallationType() RunnerInstallationType`

GetInstallationType returns the InstallationType field if non-nil, zero value otherwise.

### GetInstallationTypeOk

`func (o *RunnerSummary) GetInstallationTypeOk() (*RunnerInstallationType, bool)`

GetInstallationTypeOk returns a tuple with the InstallationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstallationType

`func (o *RunnerSummary) SetInstallationType(v RunnerInstallationType)`

SetInstallationType sets InstallationType field to given value.

### HasInstallationType

`func (o *RunnerSummary) HasInstallationType() bool`

HasInstallationType returns a boolean if a field has been set.

### GetProviders

`func (o *RunnerSummary) GetProviders() []RunnerProviderSummary`

GetProviders returns the Providers field if non-nil, zero value otherwise.

### GetProvidersOk

`func (o *RunnerSummary) GetProvidersOk() (*[]RunnerProviderSummary, bool)`

GetProvidersOk returns a tuple with the Providers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProviders

`func (o *RunnerSummary) SetProviders(v []RunnerProviderSummary)`

SetProviders sets Providers field to given value.

### HasProviders

`func (o *RunnerSummary) HasProviders() bool`

HasProviders returns a boolean if a field has been set.

### GetRunnerReplicas

`func (o *RunnerSummary) GetRunnerReplicas() int32`

GetRunnerReplicas returns the RunnerReplicas field if non-nil, zero value otherwise.

### GetRunnerReplicasOk

`func (o *RunnerSummary) GetRunnerReplicasOk() (*int32, bool)`

GetRunnerReplicasOk returns a tuple with the RunnerReplicas field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerReplicas

`func (o *RunnerSummary) SetRunnerReplicas(v int32)`

SetRunnerReplicas sets RunnerReplicas field to given value.

### HasRunnerReplicas

`func (o *RunnerSummary) HasRunnerReplicas() bool`

HasRunnerReplicas returns a boolean if a field has been set.

### GetHealthyRunnerReplicas

`func (o *RunnerSummary) GetHealthyRunnerReplicas() int32`

GetHealthyRunnerReplicas returns the HealthyRunnerReplicas field if non-nil, zero value otherwise.

### GetHealthyRunnerReplicasOk

`func (o *RunnerSummary) GetHealthyRunnerReplicasOk() (*int32, bool)`

GetHealthyRunnerReplicasOk returns a tuple with the HealthyRunnerReplicas field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHealthyRunnerReplicas

`func (o *RunnerSummary) SetHealthyRunnerReplicas(v int32)`

SetHealthyRunnerReplicas sets HealthyRunnerReplicas field to given value.

### HasHealthyRunnerReplicas

`func (o *RunnerSummary) HasHealthyRunnerReplicas() bool`

HasHealthyRunnerReplicas returns a boolean if a field has been set.

### GetRunningOperations

`func (o *RunnerSummary) GetRunningOperations() int32`

GetRunningOperations returns the RunningOperations field if non-nil, zero value otherwise.

### GetRunningOperationsOk

`func (o *RunnerSummary) GetRunningOperationsOk() (*int32, bool)`

GetRunningOperationsOk returns a tuple with the RunningOperations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunningOperations

`func (o *RunnerSummary) SetRunningOperations(v int32)`

SetRunningOperations sets RunningOperations field to given value.

### HasRunningOperations

`func (o *RunnerSummary) HasRunningOperations() bool`

HasRunningOperations returns a boolean if a field has been set.

### GetMaxRunningOperations

`func (o *RunnerSummary) GetMaxRunningOperations() int32`

GetMaxRunningOperations returns the MaxRunningOperations field if non-nil, zero value otherwise.

### GetMaxRunningOperationsOk

`func (o *RunnerSummary) GetMaxRunningOperationsOk() (*int32, bool)`

GetMaxRunningOperationsOk returns a tuple with the MaxRunningOperations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxRunningOperations

`func (o *RunnerSummary) SetMaxRunningOperations(v int32)`

SetMaxRunningOperations sets MaxRunningOperations field to given value.

### HasMaxRunningOperations

`func (o *RunnerSummary) HasMaxRunningOperations() bool`

HasMaxRunningOperations returns a boolean if a field has been set.

### GetQueuedOperations

`func (o *RunnerSummary) GetQueuedOperations() int32`

GetQueuedOperations returns the QueuedOperations field if non-nil, zero value otherwise.

### GetQueuedOperationsOk

`func (o *RunnerSummary) GetQueuedOperationsOk() (*int32, bool)`

GetQueuedOperationsOk returns a tuple with the QueuedOperations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedOperations

`func (o *RunnerSummary) SetQueuedOperations(v int32)`

SetQueuedOperations sets QueuedOperations field to given value.

### HasQueuedOperations

`func (o *RunnerSummary) HasQueuedOperations() bool`

HasQueuedOperations returns a boolean if a field has been set.

### GetCompletedOperations

`func (o *RunnerSummary) GetCompletedOperations() int32`

GetCompletedOperations returns the CompletedOperations field if non-nil, zero value otherwise.

### GetCompletedOperationsOk

`func (o *RunnerSummary) GetCompletedOperationsOk() (*int32, bool)`

GetCompletedOperationsOk returns a tuple with the CompletedOperations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedOperations

`func (o *RunnerSummary) SetCompletedOperations(v int32)`

SetCompletedOperations sets CompletedOperations field to given value.

### HasCompletedOperations

`func (o *RunnerSummary) HasCompletedOperations() bool`

HasCompletedOperations returns a boolean if a field has been set.

### GetUptime

`func (o *RunnerSummary) GetUptime() int64`

GetUptime returns the Uptime field if non-nil, zero value otherwise.

### GetUptimeOk

`func (o *RunnerSummary) GetUptimeOk() (*int64, bool)`

GetUptimeOk returns a tuple with the Uptime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUptime

`func (o *RunnerSummary) SetUptime(v int64)`

SetUptime sets Uptime field to given value.

### HasUptime

`func (o *RunnerSummary) HasUptime() bool`

HasUptime returns a boolean if a field has been set.

### GetDateCreated

`func (o *RunnerSummary) GetDateCreated() time.Time`

GetDateCreated returns the DateCreated field if non-nil, zero value otherwise.

### GetDateCreatedOk

`func (o *RunnerSummary) GetDateCreatedOk() (*time.Time, bool)`

GetDateCreatedOk returns a tuple with the DateCreated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateCreated

`func (o *RunnerSummary) SetDateCreated(v time.Time)`

SetDateCreated sets DateCreated field to given value.

### HasDateCreated

`func (o *RunnerSummary) HasDateCreated() bool`

HasDateCreated returns a boolean if a field has been set.

### GetLastUpdated

`func (o *RunnerSummary) GetLastUpdated() time.Time`

GetLastUpdated returns the LastUpdated field if non-nil, zero value otherwise.

### GetLastUpdatedOk

`func (o *RunnerSummary) GetLastUpdatedOk() (*time.Time, bool)`

GetLastUpdatedOk returns a tuple with the LastUpdated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUpdated

`func (o *RunnerSummary) SetLastUpdated(v time.Time)`

SetLastUpdated sets LastUpdated field to given value.

### HasLastUpdated

`func (o *RunnerSummary) HasLastUpdated() bool`

HasLastUpdated returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



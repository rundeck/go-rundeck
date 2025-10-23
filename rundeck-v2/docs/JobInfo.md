# JobInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Group** | Pointer to **string** |  | [optional] 
**Project** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Href** | Pointer to **string** |  | [optional] 
**Permalink** | Pointer to **string** |  | [optional] 
**Scheduled** | Pointer to **bool** |  | [optional] 
**ScheduleEnabled** | Pointer to **bool** |  | [optional] 
**Enabled** | Pointer to **bool** |  | [optional] 
**ServerNodeUUID** | Pointer to **string** |  | [optional] 
**ServerOwner** | Pointer to **bool** |  | [optional] 
**AverageDuration** | Pointer to **int64** |  | [optional] 
**NextScheduledExecution** | Pointer to **time.Time** |  | [optional] 
**FutureScheduledExecutions** | Pointer to [**[]time.Time**](time.Time.md) |  | [optional] 
**ProjectDisableExecutions** | Pointer to **bool** |  | [optional] 
**ProjectDisableSchedule** | Pointer to **bool** |  | [optional] 
**Created** | Pointer to **string** |  | [optional] 
**CreatedBy** | Pointer to **string** |  | [optional] 
**LastModified** | Pointer to **string** |  | [optional] 
**LastModifiedBy** | Pointer to **string** |  | [optional] 

## Methods

### NewJobInfo

`func NewJobInfo() *JobInfo`

NewJobInfo instantiates a new JobInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobInfoWithDefaults

`func NewJobInfoWithDefaults() *JobInfo`

NewJobInfoWithDefaults instantiates a new JobInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *JobInfo) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *JobInfo) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *JobInfo) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *JobInfo) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *JobInfo) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *JobInfo) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *JobInfo) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *JobInfo) HasName() bool`

HasName returns a boolean if a field has been set.

### GetGroup

`func (o *JobInfo) GetGroup() string`

GetGroup returns the Group field if non-nil, zero value otherwise.

### GetGroupOk

`func (o *JobInfo) GetGroupOk() (*string, bool)`

GetGroupOk returns a tuple with the Group field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroup

`func (o *JobInfo) SetGroup(v string)`

SetGroup sets Group field to given value.

### HasGroup

`func (o *JobInfo) HasGroup() bool`

HasGroup returns a boolean if a field has been set.

### GetProject

`func (o *JobInfo) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *JobInfo) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *JobInfo) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *JobInfo) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetDescription

`func (o *JobInfo) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *JobInfo) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *JobInfo) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *JobInfo) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetHref

`func (o *JobInfo) GetHref() string`

GetHref returns the Href field if non-nil, zero value otherwise.

### GetHrefOk

`func (o *JobInfo) GetHrefOk() (*string, bool)`

GetHrefOk returns a tuple with the Href field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHref

`func (o *JobInfo) SetHref(v string)`

SetHref sets Href field to given value.

### HasHref

`func (o *JobInfo) HasHref() bool`

HasHref returns a boolean if a field has been set.

### GetPermalink

`func (o *JobInfo) GetPermalink() string`

GetPermalink returns the Permalink field if non-nil, zero value otherwise.

### GetPermalinkOk

`func (o *JobInfo) GetPermalinkOk() (*string, bool)`

GetPermalinkOk returns a tuple with the Permalink field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPermalink

`func (o *JobInfo) SetPermalink(v string)`

SetPermalink sets Permalink field to given value.

### HasPermalink

`func (o *JobInfo) HasPermalink() bool`

HasPermalink returns a boolean if a field has been set.

### GetScheduled

`func (o *JobInfo) GetScheduled() bool`

GetScheduled returns the Scheduled field if non-nil, zero value otherwise.

### GetScheduledOk

`func (o *JobInfo) GetScheduledOk() (*bool, bool)`

GetScheduledOk returns a tuple with the Scheduled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScheduled

`func (o *JobInfo) SetScheduled(v bool)`

SetScheduled sets Scheduled field to given value.

### HasScheduled

`func (o *JobInfo) HasScheduled() bool`

HasScheduled returns a boolean if a field has been set.

### GetScheduleEnabled

`func (o *JobInfo) GetScheduleEnabled() bool`

GetScheduleEnabled returns the ScheduleEnabled field if non-nil, zero value otherwise.

### GetScheduleEnabledOk

`func (o *JobInfo) GetScheduleEnabledOk() (*bool, bool)`

GetScheduleEnabledOk returns a tuple with the ScheduleEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScheduleEnabled

`func (o *JobInfo) SetScheduleEnabled(v bool)`

SetScheduleEnabled sets ScheduleEnabled field to given value.

### HasScheduleEnabled

`func (o *JobInfo) HasScheduleEnabled() bool`

HasScheduleEnabled returns a boolean if a field has been set.

### GetEnabled

`func (o *JobInfo) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *JobInfo) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *JobInfo) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *JobInfo) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetServerNodeUUID

`func (o *JobInfo) GetServerNodeUUID() string`

GetServerNodeUUID returns the ServerNodeUUID field if non-nil, zero value otherwise.

### GetServerNodeUUIDOk

`func (o *JobInfo) GetServerNodeUUIDOk() (*string, bool)`

GetServerNodeUUIDOk returns a tuple with the ServerNodeUUID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServerNodeUUID

`func (o *JobInfo) SetServerNodeUUID(v string)`

SetServerNodeUUID sets ServerNodeUUID field to given value.

### HasServerNodeUUID

`func (o *JobInfo) HasServerNodeUUID() bool`

HasServerNodeUUID returns a boolean if a field has been set.

### GetServerOwner

`func (o *JobInfo) GetServerOwner() bool`

GetServerOwner returns the ServerOwner field if non-nil, zero value otherwise.

### GetServerOwnerOk

`func (o *JobInfo) GetServerOwnerOk() (*bool, bool)`

GetServerOwnerOk returns a tuple with the ServerOwner field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServerOwner

`func (o *JobInfo) SetServerOwner(v bool)`

SetServerOwner sets ServerOwner field to given value.

### HasServerOwner

`func (o *JobInfo) HasServerOwner() bool`

HasServerOwner returns a boolean if a field has been set.

### GetAverageDuration

`func (o *JobInfo) GetAverageDuration() int64`

GetAverageDuration returns the AverageDuration field if non-nil, zero value otherwise.

### GetAverageDurationOk

`func (o *JobInfo) GetAverageDurationOk() (*int64, bool)`

GetAverageDurationOk returns a tuple with the AverageDuration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAverageDuration

`func (o *JobInfo) SetAverageDuration(v int64)`

SetAverageDuration sets AverageDuration field to given value.

### HasAverageDuration

`func (o *JobInfo) HasAverageDuration() bool`

HasAverageDuration returns a boolean if a field has been set.

### GetNextScheduledExecution

`func (o *JobInfo) GetNextScheduledExecution() time.Time`

GetNextScheduledExecution returns the NextScheduledExecution field if non-nil, zero value otherwise.

### GetNextScheduledExecutionOk

`func (o *JobInfo) GetNextScheduledExecutionOk() (*time.Time, bool)`

GetNextScheduledExecutionOk returns a tuple with the NextScheduledExecution field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextScheduledExecution

`func (o *JobInfo) SetNextScheduledExecution(v time.Time)`

SetNextScheduledExecution sets NextScheduledExecution field to given value.

### HasNextScheduledExecution

`func (o *JobInfo) HasNextScheduledExecution() bool`

HasNextScheduledExecution returns a boolean if a field has been set.

### GetFutureScheduledExecutions

`func (o *JobInfo) GetFutureScheduledExecutions() []time.Time`

GetFutureScheduledExecutions returns the FutureScheduledExecutions field if non-nil, zero value otherwise.

### GetFutureScheduledExecutionsOk

`func (o *JobInfo) GetFutureScheduledExecutionsOk() (*[]time.Time, bool)`

GetFutureScheduledExecutionsOk returns a tuple with the FutureScheduledExecutions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFutureScheduledExecutions

`func (o *JobInfo) SetFutureScheduledExecutions(v []time.Time)`

SetFutureScheduledExecutions sets FutureScheduledExecutions field to given value.

### HasFutureScheduledExecutions

`func (o *JobInfo) HasFutureScheduledExecutions() bool`

HasFutureScheduledExecutions returns a boolean if a field has been set.

### GetProjectDisableExecutions

`func (o *JobInfo) GetProjectDisableExecutions() bool`

GetProjectDisableExecutions returns the ProjectDisableExecutions field if non-nil, zero value otherwise.

### GetProjectDisableExecutionsOk

`func (o *JobInfo) GetProjectDisableExecutionsOk() (*bool, bool)`

GetProjectDisableExecutionsOk returns a tuple with the ProjectDisableExecutions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectDisableExecutions

`func (o *JobInfo) SetProjectDisableExecutions(v bool)`

SetProjectDisableExecutions sets ProjectDisableExecutions field to given value.

### HasProjectDisableExecutions

`func (o *JobInfo) HasProjectDisableExecutions() bool`

HasProjectDisableExecutions returns a boolean if a field has been set.

### GetProjectDisableSchedule

`func (o *JobInfo) GetProjectDisableSchedule() bool`

GetProjectDisableSchedule returns the ProjectDisableSchedule field if non-nil, zero value otherwise.

### GetProjectDisableScheduleOk

`func (o *JobInfo) GetProjectDisableScheduleOk() (*bool, bool)`

GetProjectDisableScheduleOk returns a tuple with the ProjectDisableSchedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectDisableSchedule

`func (o *JobInfo) SetProjectDisableSchedule(v bool)`

SetProjectDisableSchedule sets ProjectDisableSchedule field to given value.

### HasProjectDisableSchedule

`func (o *JobInfo) HasProjectDisableSchedule() bool`

HasProjectDisableSchedule returns a boolean if a field has been set.

### GetCreated

`func (o *JobInfo) GetCreated() string`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *JobInfo) GetCreatedOk() (*string, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *JobInfo) SetCreated(v string)`

SetCreated sets Created field to given value.

### HasCreated

`func (o *JobInfo) HasCreated() bool`

HasCreated returns a boolean if a field has been set.

### GetCreatedBy

`func (o *JobInfo) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *JobInfo) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *JobInfo) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.

### HasCreatedBy

`func (o *JobInfo) HasCreatedBy() bool`

HasCreatedBy returns a boolean if a field has been set.

### GetLastModified

`func (o *JobInfo) GetLastModified() string`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *JobInfo) GetLastModifiedOk() (*string, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *JobInfo) SetLastModified(v string)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *JobInfo) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### GetLastModifiedBy

`func (o *JobInfo) GetLastModifiedBy() string`

GetLastModifiedBy returns the LastModifiedBy field if non-nil, zero value otherwise.

### GetLastModifiedByOk

`func (o *JobInfo) GetLastModifiedByOk() (*string, bool)`

GetLastModifiedByOk returns a tuple with the LastModifiedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModifiedBy

`func (o *JobInfo) SetLastModifiedBy(v string)`

SetLastModifiedBy sets LastModifiedBy field to given value.

### HasLastModifiedBy

`func (o *JobInfo) HasLastModifiedBy() bool`

HasLastModifiedBy returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ScmExportActionItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ItemId** | Pointer to **string** | ID of the repo item, e.g. a file path | [optional] 
**OriginalId** | Pointer to **string** | ID of a repo item if the job was renamed and now is stored at a different repo path, or empty/null | [optional] 
**Job** | Pointer to [**JobReference**](JobReference.md) |  | [optional] 
**Deleted** | Pointer to **bool** | whether the job was deleted and requires deleting the associated repo item | [optional] 
**Renamed** | Pointer to **bool** | boolean if the job was renamed | [optional] 
**Status** | Pointer to **string** | file status String, the same value as in the &#x60;synchState&#x60; of Job Scm Status result. | [optional] 

## Methods

### NewScmExportActionItem

`func NewScmExportActionItem() *ScmExportActionItem`

NewScmExportActionItem instantiates a new ScmExportActionItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmExportActionItemWithDefaults

`func NewScmExportActionItemWithDefaults() *ScmExportActionItem`

NewScmExportActionItemWithDefaults instantiates a new ScmExportActionItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItemId

`func (o *ScmExportActionItem) GetItemId() string`

GetItemId returns the ItemId field if non-nil, zero value otherwise.

### GetItemIdOk

`func (o *ScmExportActionItem) GetItemIdOk() (*string, bool)`

GetItemIdOk returns a tuple with the ItemId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemId

`func (o *ScmExportActionItem) SetItemId(v string)`

SetItemId sets ItemId field to given value.

### HasItemId

`func (o *ScmExportActionItem) HasItemId() bool`

HasItemId returns a boolean if a field has been set.

### GetOriginalId

`func (o *ScmExportActionItem) GetOriginalId() string`

GetOriginalId returns the OriginalId field if non-nil, zero value otherwise.

### GetOriginalIdOk

`func (o *ScmExportActionItem) GetOriginalIdOk() (*string, bool)`

GetOriginalIdOk returns a tuple with the OriginalId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalId

`func (o *ScmExportActionItem) SetOriginalId(v string)`

SetOriginalId sets OriginalId field to given value.

### HasOriginalId

`func (o *ScmExportActionItem) HasOriginalId() bool`

HasOriginalId returns a boolean if a field has been set.

### GetJob

`func (o *ScmExportActionItem) GetJob() JobReference`

GetJob returns the Job field if non-nil, zero value otherwise.

### GetJobOk

`func (o *ScmExportActionItem) GetJobOk() (*JobReference, bool)`

GetJobOk returns a tuple with the Job field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJob

`func (o *ScmExportActionItem) SetJob(v JobReference)`

SetJob sets Job field to given value.

### HasJob

`func (o *ScmExportActionItem) HasJob() bool`

HasJob returns a boolean if a field has been set.

### GetDeleted

`func (o *ScmExportActionItem) GetDeleted() bool`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *ScmExportActionItem) GetDeletedOk() (*bool, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *ScmExportActionItem) SetDeleted(v bool)`

SetDeleted sets Deleted field to given value.

### HasDeleted

`func (o *ScmExportActionItem) HasDeleted() bool`

HasDeleted returns a boolean if a field has been set.

### GetRenamed

`func (o *ScmExportActionItem) GetRenamed() bool`

GetRenamed returns the Renamed field if non-nil, zero value otherwise.

### GetRenamedOk

`func (o *ScmExportActionItem) GetRenamedOk() (*bool, bool)`

GetRenamedOk returns a tuple with the Renamed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenamed

`func (o *ScmExportActionItem) SetRenamed(v bool)`

SetRenamed sets Renamed field to given value.

### HasRenamed

`func (o *ScmExportActionItem) HasRenamed() bool`

HasRenamed returns a boolean if a field has been set.

### GetStatus

`func (o *ScmExportActionItem) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ScmExportActionItem) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ScmExportActionItem) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *ScmExportActionItem) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



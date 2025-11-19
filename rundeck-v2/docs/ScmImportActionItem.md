# ScmImportActionItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ItemId** | Pointer to **string** | ID of the repo item, e.g. a file path | [optional] 
**Job** | Pointer to [**JobReference**](JobReference.md) |  | [optional] 
**Tracked** | Pointer to **bool** | true if there is an associated &#x60;job&#x60; | [optional] 
**Deleted** | Pointer to **bool** | whether the job was deleted on remote and requires to be deleted | [optional] 
**Status** | Pointer to **string** | file status String, the same value as in the &#x60;synchState&#x60; of Job Scm Status result. | [optional] 

## Methods

### NewScmImportActionItem

`func NewScmImportActionItem() *ScmImportActionItem`

NewScmImportActionItem instantiates a new ScmImportActionItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmImportActionItemWithDefaults

`func NewScmImportActionItemWithDefaults() *ScmImportActionItem`

NewScmImportActionItemWithDefaults instantiates a new ScmImportActionItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItemId

`func (o *ScmImportActionItem) GetItemId() string`

GetItemId returns the ItemId field if non-nil, zero value otherwise.

### GetItemIdOk

`func (o *ScmImportActionItem) GetItemIdOk() (*string, bool)`

GetItemIdOk returns a tuple with the ItemId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemId

`func (o *ScmImportActionItem) SetItemId(v string)`

SetItemId sets ItemId field to given value.

### HasItemId

`func (o *ScmImportActionItem) HasItemId() bool`

HasItemId returns a boolean if a field has been set.

### GetJob

`func (o *ScmImportActionItem) GetJob() JobReference`

GetJob returns the Job field if non-nil, zero value otherwise.

### GetJobOk

`func (o *ScmImportActionItem) GetJobOk() (*JobReference, bool)`

GetJobOk returns a tuple with the Job field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJob

`func (o *ScmImportActionItem) SetJob(v JobReference)`

SetJob sets Job field to given value.

### HasJob

`func (o *ScmImportActionItem) HasJob() bool`

HasJob returns a boolean if a field has been set.

### GetTracked

`func (o *ScmImportActionItem) GetTracked() bool`

GetTracked returns the Tracked field if non-nil, zero value otherwise.

### GetTrackedOk

`func (o *ScmImportActionItem) GetTrackedOk() (*bool, bool)`

GetTrackedOk returns a tuple with the Tracked field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTracked

`func (o *ScmImportActionItem) SetTracked(v bool)`

SetTracked sets Tracked field to given value.

### HasTracked

`func (o *ScmImportActionItem) HasTracked() bool`

HasTracked returns a boolean if a field has been set.

### GetDeleted

`func (o *ScmImportActionItem) GetDeleted() bool`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *ScmImportActionItem) GetDeletedOk() (*bool, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *ScmImportActionItem) SetDeleted(v bool)`

SetDeleted sets Deleted field to given value.

### HasDeleted

`func (o *ScmImportActionItem) HasDeleted() bool`

HasDeleted returns a boolean if a field has been set.

### GetStatus

`func (o *ScmImportActionItem) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ScmImportActionItem) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ScmImportActionItem) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *ScmImportActionItem) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



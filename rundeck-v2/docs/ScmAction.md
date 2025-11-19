# ScmAction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Input** | Pointer to **map[string]string** | input fields for the action | [optional] 
**Items** | Pointer to **[]string** | list of selected item IDs | [optional] 
**Jobs** | Pointer to **[]string** | list of selected Job IDs | [optional] 
**Deleted** | Pointer to **[]string** | list of deleted item IDs | [optional] 
**DeletedJobs** | Pointer to **[]string** | list of deleted Job IDs (import) | [optional] 

## Methods

### NewScmAction

`func NewScmAction() *ScmAction`

NewScmAction instantiates a new ScmAction object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmActionWithDefaults

`func NewScmActionWithDefaults() *ScmAction`

NewScmActionWithDefaults instantiates a new ScmAction object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetInput

`func (o *ScmAction) GetInput() map[string]string`

GetInput returns the Input field if non-nil, zero value otherwise.

### GetInputOk

`func (o *ScmAction) GetInputOk() (*map[string]string, bool)`

GetInputOk returns a tuple with the Input field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInput

`func (o *ScmAction) SetInput(v map[string]string)`

SetInput sets Input field to given value.

### HasInput

`func (o *ScmAction) HasInput() bool`

HasInput returns a boolean if a field has been set.

### GetItems

`func (o *ScmAction) GetItems() []string`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *ScmAction) GetItemsOk() (*[]string, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *ScmAction) SetItems(v []string)`

SetItems sets Items field to given value.

### HasItems

`func (o *ScmAction) HasItems() bool`

HasItems returns a boolean if a field has been set.

### GetJobs

`func (o *ScmAction) GetJobs() []string`

GetJobs returns the Jobs field if non-nil, zero value otherwise.

### GetJobsOk

`func (o *ScmAction) GetJobsOk() (*[]string, bool)`

GetJobsOk returns a tuple with the Jobs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobs

`func (o *ScmAction) SetJobs(v []string)`

SetJobs sets Jobs field to given value.

### HasJobs

`func (o *ScmAction) HasJobs() bool`

HasJobs returns a boolean if a field has been set.

### GetDeleted

`func (o *ScmAction) GetDeleted() []string`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *ScmAction) GetDeletedOk() (*[]string, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *ScmAction) SetDeleted(v []string)`

SetDeleted sets Deleted field to given value.

### HasDeleted

`func (o *ScmAction) HasDeleted() bool`

HasDeleted returns a boolean if a field has been set.

### GetDeletedJobs

`func (o *ScmAction) GetDeletedJobs() []string`

GetDeletedJobs returns the DeletedJobs field if non-nil, zero value otherwise.

### GetDeletedJobsOk

`func (o *ScmAction) GetDeletedJobsOk() (*[]string, bool)`

GetDeletedJobsOk returns a tuple with the DeletedJobs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeletedJobs

`func (o *ScmAction) SetDeletedJobs(v []string)`

SetDeletedJobs sets DeletedJobs field to given value.

### HasDeletedJobs

`func (o *ScmAction) HasDeletedJobs() bool`

HasDeletedJobs returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



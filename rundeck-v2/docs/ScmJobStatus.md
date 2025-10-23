# ScmJobStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Project** | Pointer to **string** |  | [optional] 
**Integration** | Pointer to **string** |  | [optional] 
**SynchState** | Pointer to **string** |  | [optional] 
**Message** | Pointer to **string** |  | [optional] 
**Actions** | Pointer to **[]string** |  | [optional] 
**Commit** | Pointer to [**ScmCommit**](ScmCommit.md) |  | [optional] 

## Methods

### NewScmJobStatus

`func NewScmJobStatus() *ScmJobStatus`

NewScmJobStatus instantiates a new ScmJobStatus object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmJobStatusWithDefaults

`func NewScmJobStatusWithDefaults() *ScmJobStatus`

NewScmJobStatusWithDefaults instantiates a new ScmJobStatus object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScmJobStatus) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScmJobStatus) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScmJobStatus) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *ScmJobStatus) HasId() bool`

HasId returns a boolean if a field has been set.

### GetProject

`func (o *ScmJobStatus) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *ScmJobStatus) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *ScmJobStatus) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *ScmJobStatus) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetIntegration

`func (o *ScmJobStatus) GetIntegration() string`

GetIntegration returns the Integration field if non-nil, zero value otherwise.

### GetIntegrationOk

`func (o *ScmJobStatus) GetIntegrationOk() (*string, bool)`

GetIntegrationOk returns a tuple with the Integration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegration

`func (o *ScmJobStatus) SetIntegration(v string)`

SetIntegration sets Integration field to given value.

### HasIntegration

`func (o *ScmJobStatus) HasIntegration() bool`

HasIntegration returns a boolean if a field has been set.

### GetSynchState

`func (o *ScmJobStatus) GetSynchState() string`

GetSynchState returns the SynchState field if non-nil, zero value otherwise.

### GetSynchStateOk

`func (o *ScmJobStatus) GetSynchStateOk() (*string, bool)`

GetSynchStateOk returns a tuple with the SynchState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSynchState

`func (o *ScmJobStatus) SetSynchState(v string)`

SetSynchState sets SynchState field to given value.

### HasSynchState

`func (o *ScmJobStatus) HasSynchState() bool`

HasSynchState returns a boolean if a field has been set.

### GetMessage

`func (o *ScmJobStatus) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ScmJobStatus) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ScmJobStatus) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *ScmJobStatus) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetActions

`func (o *ScmJobStatus) GetActions() []string`

GetActions returns the Actions field if non-nil, zero value otherwise.

### GetActionsOk

`func (o *ScmJobStatus) GetActionsOk() (*[]string, bool)`

GetActionsOk returns a tuple with the Actions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActions

`func (o *ScmJobStatus) SetActions(v []string)`

SetActions sets Actions field to given value.

### HasActions

`func (o *ScmJobStatus) HasActions() bool`

HasActions returns a boolean if a field has been set.

### GetCommit

`func (o *ScmJobStatus) GetCommit() ScmCommit`

GetCommit returns the Commit field if non-nil, zero value otherwise.

### GetCommitOk

`func (o *ScmJobStatus) GetCommitOk() (*ScmCommit, bool)`

GetCommitOk returns a tuple with the Commit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommit

`func (o *ScmJobStatus) SetCommit(v ScmCommit)`

SetCommit sets Commit field to given value.

### HasCommit

`func (o *ScmJobStatus) HasCommit() bool`

HasCommit returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ScmProjectStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Project** | Pointer to **string** |  | [optional] 
**Integration** | Pointer to **string** |  | [optional] 
**SynchState** | Pointer to **string** | Indicates the state.  Import plugin values for &#x60;synchState&#x60;:  * &#x60;CLEAN&#x60; - no changes * &#x60;UNKNOWN&#x60; - status unknown * &#x60;REFRESH_NEEDED&#x60; - plugin needs to refresh * &#x60;IMPORT_NEEDED&#x60; - some changes need to be imported * &#x60;DELETE_NEEDED&#x60; - some jobs need to be deleted  Export plugin values for &#x60;synchState&#x60;:  * &#x60;CLEAN&#x60; - no changes * &#x60;REFRESH_NEEDED&#x60; - plugin needs to refresh * &#x60;EXPORT_NEEDED&#x60; - some changes need to be exported * &#x60;CREATE_NEEDED&#x60; - some jobs need to be added to the repo  | [optional] 
**Message** | Pointer to **string** |  | [optional] 
**Actions** | Pointer to **[]string** | empty, or a list of action ID strings. | [optional] 

## Methods

### NewScmProjectStatus

`func NewScmProjectStatus() *ScmProjectStatus`

NewScmProjectStatus instantiates a new ScmProjectStatus object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmProjectStatusWithDefaults

`func NewScmProjectStatusWithDefaults() *ScmProjectStatus`

NewScmProjectStatusWithDefaults instantiates a new ScmProjectStatus object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProject

`func (o *ScmProjectStatus) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *ScmProjectStatus) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *ScmProjectStatus) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *ScmProjectStatus) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetIntegration

`func (o *ScmProjectStatus) GetIntegration() string`

GetIntegration returns the Integration field if non-nil, zero value otherwise.

### GetIntegrationOk

`func (o *ScmProjectStatus) GetIntegrationOk() (*string, bool)`

GetIntegrationOk returns a tuple with the Integration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegration

`func (o *ScmProjectStatus) SetIntegration(v string)`

SetIntegration sets Integration field to given value.

### HasIntegration

`func (o *ScmProjectStatus) HasIntegration() bool`

HasIntegration returns a boolean if a field has been set.

### GetSynchState

`func (o *ScmProjectStatus) GetSynchState() string`

GetSynchState returns the SynchState field if non-nil, zero value otherwise.

### GetSynchStateOk

`func (o *ScmProjectStatus) GetSynchStateOk() (*string, bool)`

GetSynchStateOk returns a tuple with the SynchState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSynchState

`func (o *ScmProjectStatus) SetSynchState(v string)`

SetSynchState sets SynchState field to given value.

### HasSynchState

`func (o *ScmProjectStatus) HasSynchState() bool`

HasSynchState returns a boolean if a field has been set.

### GetMessage

`func (o *ScmProjectStatus) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ScmProjectStatus) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ScmProjectStatus) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *ScmProjectStatus) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetActions

`func (o *ScmProjectStatus) GetActions() []string`

GetActions returns the Actions field if non-nil, zero value otherwise.

### GetActionsOk

`func (o *ScmProjectStatus) GetActionsOk() (*[]string, bool)`

GetActionsOk returns a tuple with the Actions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActions

`func (o *ScmProjectStatus) SetActions(v []string)`

SetActions sets Actions field to given value.

### HasActions

`func (o *ScmProjectStatus) HasActions() bool`

HasActions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



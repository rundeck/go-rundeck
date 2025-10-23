# ScmJobDiff

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Project** | Pointer to **string** |  | [optional] 
**Integration** | Pointer to **string** |  | [optional] 
**Commit** | Pointer to [**ScmCommit**](ScmCommit.md) |  | [optional] 
**IncomingCommit** | Pointer to [**ScmCommit**](ScmCommit.md) |  | [optional] 
**DiffContent** | Pointer to **string** |  | [optional] 

## Methods

### NewScmJobDiff

`func NewScmJobDiff() *ScmJobDiff`

NewScmJobDiff instantiates a new ScmJobDiff object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmJobDiffWithDefaults

`func NewScmJobDiffWithDefaults() *ScmJobDiff`

NewScmJobDiffWithDefaults instantiates a new ScmJobDiff object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScmJobDiff) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScmJobDiff) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScmJobDiff) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *ScmJobDiff) HasId() bool`

HasId returns a boolean if a field has been set.

### GetProject

`func (o *ScmJobDiff) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *ScmJobDiff) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *ScmJobDiff) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *ScmJobDiff) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetIntegration

`func (o *ScmJobDiff) GetIntegration() string`

GetIntegration returns the Integration field if non-nil, zero value otherwise.

### GetIntegrationOk

`func (o *ScmJobDiff) GetIntegrationOk() (*string, bool)`

GetIntegrationOk returns a tuple with the Integration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegration

`func (o *ScmJobDiff) SetIntegration(v string)`

SetIntegration sets Integration field to given value.

### HasIntegration

`func (o *ScmJobDiff) HasIntegration() bool`

HasIntegration returns a boolean if a field has been set.

### GetCommit

`func (o *ScmJobDiff) GetCommit() ScmCommit`

GetCommit returns the Commit field if non-nil, zero value otherwise.

### GetCommitOk

`func (o *ScmJobDiff) GetCommitOk() (*ScmCommit, bool)`

GetCommitOk returns a tuple with the Commit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommit

`func (o *ScmJobDiff) SetCommit(v ScmCommit)`

SetCommit sets Commit field to given value.

### HasCommit

`func (o *ScmJobDiff) HasCommit() bool`

HasCommit returns a boolean if a field has been set.

### GetIncomingCommit

`func (o *ScmJobDiff) GetIncomingCommit() ScmCommit`

GetIncomingCommit returns the IncomingCommit field if non-nil, zero value otherwise.

### GetIncomingCommitOk

`func (o *ScmJobDiff) GetIncomingCommitOk() (*ScmCommit, bool)`

GetIncomingCommitOk returns a tuple with the IncomingCommit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncomingCommit

`func (o *ScmJobDiff) SetIncomingCommit(v ScmCommit)`

SetIncomingCommit sets IncomingCommit field to given value.

### HasIncomingCommit

`func (o *ScmJobDiff) HasIncomingCommit() bool`

HasIncomingCommit returns a boolean if a field has been set.

### GetDiffContent

`func (o *ScmJobDiff) GetDiffContent() string`

GetDiffContent returns the DiffContent field if non-nil, zero value otherwise.

### GetDiffContentOk

`func (o *ScmJobDiff) GetDiffContentOk() (*string, bool)`

GetDiffContentOk returns a tuple with the DiffContent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiffContent

`func (o *ScmJobDiff) SetDiffContent(v string)`

SetDiffContent sets DiffContent field to given value.

### HasDiffContent

`func (o *ScmJobDiff) HasDiffContent() bool`

HasDiffContent returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CreateProjectRunnerRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Name of the Runner | 
**Description** | **string** | Description of the Runner | 
**TagNames** | Pointer to **string** | Comma separated tags | [optional] 
**AssignedProjects** | Pointer to **map[string]string** | Map of project names to their associated runner roles | [optional] 
**ProjectRunnerAsNode** | Pointer to **map[string]bool** | Map of project names to a boolean indicating if the runner should be associated as a node executor for that project | [optional] 
**InstallationType** | Pointer to **string** | Installation type of the Runner | [optional] 
**ReplicaType** | Pointer to **string** | Replica type of the Runner | [optional] 
**NewRunnerRequest** | Pointer to [**CreateRunnerRequest**](CreateRunnerRequest.md) |  | [optional] 

## Methods

### NewCreateProjectRunnerRequest

`func NewCreateProjectRunnerRequest(name string, description string, ) *CreateProjectRunnerRequest`

NewCreateProjectRunnerRequest instantiates a new CreateProjectRunnerRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateProjectRunnerRequestWithDefaults

`func NewCreateProjectRunnerRequestWithDefaults() *CreateProjectRunnerRequest`

NewCreateProjectRunnerRequestWithDefaults instantiates a new CreateProjectRunnerRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateProjectRunnerRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateProjectRunnerRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateProjectRunnerRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *CreateProjectRunnerRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateProjectRunnerRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateProjectRunnerRequest) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetTagNames

`func (o *CreateProjectRunnerRequest) GetTagNames() string`

GetTagNames returns the TagNames field if non-nil, zero value otherwise.

### GetTagNamesOk

`func (o *CreateProjectRunnerRequest) GetTagNamesOk() (*string, bool)`

GetTagNamesOk returns a tuple with the TagNames field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagNames

`func (o *CreateProjectRunnerRequest) SetTagNames(v string)`

SetTagNames sets TagNames field to given value.

### HasTagNames

`func (o *CreateProjectRunnerRequest) HasTagNames() bool`

HasTagNames returns a boolean if a field has been set.

### GetAssignedProjects

`func (o *CreateProjectRunnerRequest) GetAssignedProjects() map[string]string`

GetAssignedProjects returns the AssignedProjects field if non-nil, zero value otherwise.

### GetAssignedProjectsOk

`func (o *CreateProjectRunnerRequest) GetAssignedProjectsOk() (*map[string]string, bool)`

GetAssignedProjectsOk returns a tuple with the AssignedProjects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssignedProjects

`func (o *CreateProjectRunnerRequest) SetAssignedProjects(v map[string]string)`

SetAssignedProjects sets AssignedProjects field to given value.

### HasAssignedProjects

`func (o *CreateProjectRunnerRequest) HasAssignedProjects() bool`

HasAssignedProjects returns a boolean if a field has been set.

### GetProjectRunnerAsNode

`func (o *CreateProjectRunnerRequest) GetProjectRunnerAsNode() map[string]bool`

GetProjectRunnerAsNode returns the ProjectRunnerAsNode field if non-nil, zero value otherwise.

### GetProjectRunnerAsNodeOk

`func (o *CreateProjectRunnerRequest) GetProjectRunnerAsNodeOk() (*map[string]bool, bool)`

GetProjectRunnerAsNodeOk returns a tuple with the ProjectRunnerAsNode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectRunnerAsNode

`func (o *CreateProjectRunnerRequest) SetProjectRunnerAsNode(v map[string]bool)`

SetProjectRunnerAsNode sets ProjectRunnerAsNode field to given value.

### HasProjectRunnerAsNode

`func (o *CreateProjectRunnerRequest) HasProjectRunnerAsNode() bool`

HasProjectRunnerAsNode returns a boolean if a field has been set.

### GetInstallationType

`func (o *CreateProjectRunnerRequest) GetInstallationType() string`

GetInstallationType returns the InstallationType field if non-nil, zero value otherwise.

### GetInstallationTypeOk

`func (o *CreateProjectRunnerRequest) GetInstallationTypeOk() (*string, bool)`

GetInstallationTypeOk returns a tuple with the InstallationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstallationType

`func (o *CreateProjectRunnerRequest) SetInstallationType(v string)`

SetInstallationType sets InstallationType field to given value.

### HasInstallationType

`func (o *CreateProjectRunnerRequest) HasInstallationType() bool`

HasInstallationType returns a boolean if a field has been set.

### GetReplicaType

`func (o *CreateProjectRunnerRequest) GetReplicaType() string`

GetReplicaType returns the ReplicaType field if non-nil, zero value otherwise.

### GetReplicaTypeOk

`func (o *CreateProjectRunnerRequest) GetReplicaTypeOk() (*string, bool)`

GetReplicaTypeOk returns a tuple with the ReplicaType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaType

`func (o *CreateProjectRunnerRequest) SetReplicaType(v string)`

SetReplicaType sets ReplicaType field to given value.

### HasReplicaType

`func (o *CreateProjectRunnerRequest) HasReplicaType() bool`

HasReplicaType returns a boolean if a field has been set.

### GetNewRunnerRequest

`func (o *CreateProjectRunnerRequest) GetNewRunnerRequest() CreateRunnerRequest`

GetNewRunnerRequest returns the NewRunnerRequest field if non-nil, zero value otherwise.

### GetNewRunnerRequestOk

`func (o *CreateProjectRunnerRequest) GetNewRunnerRequestOk() (*CreateRunnerRequest, bool)`

GetNewRunnerRequestOk returns a tuple with the NewRunnerRequest field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewRunnerRequest

`func (o *CreateProjectRunnerRequest) SetNewRunnerRequest(v CreateRunnerRequest)`

SetNewRunnerRequest sets NewRunnerRequest field to given value.

### HasNewRunnerRequest

`func (o *CreateProjectRunnerRequest) HasNewRunnerRequest() bool`

HasNewRunnerRequest returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



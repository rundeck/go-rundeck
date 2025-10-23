# CreateRunnerRequest

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

## Methods

### NewCreateRunnerRequest

`func NewCreateRunnerRequest(name string, description string, ) *CreateRunnerRequest`

NewCreateRunnerRequest instantiates a new CreateRunnerRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateRunnerRequestWithDefaults

`func NewCreateRunnerRequestWithDefaults() *CreateRunnerRequest`

NewCreateRunnerRequestWithDefaults instantiates a new CreateRunnerRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateRunnerRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateRunnerRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateRunnerRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *CreateRunnerRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateRunnerRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateRunnerRequest) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetTagNames

`func (o *CreateRunnerRequest) GetTagNames() string`

GetTagNames returns the TagNames field if non-nil, zero value otherwise.

### GetTagNamesOk

`func (o *CreateRunnerRequest) GetTagNamesOk() (*string, bool)`

GetTagNamesOk returns a tuple with the TagNames field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagNames

`func (o *CreateRunnerRequest) SetTagNames(v string)`

SetTagNames sets TagNames field to given value.

### HasTagNames

`func (o *CreateRunnerRequest) HasTagNames() bool`

HasTagNames returns a boolean if a field has been set.

### GetAssignedProjects

`func (o *CreateRunnerRequest) GetAssignedProjects() map[string]string`

GetAssignedProjects returns the AssignedProjects field if non-nil, zero value otherwise.

### GetAssignedProjectsOk

`func (o *CreateRunnerRequest) GetAssignedProjectsOk() (*map[string]string, bool)`

GetAssignedProjectsOk returns a tuple with the AssignedProjects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssignedProjects

`func (o *CreateRunnerRequest) SetAssignedProjects(v map[string]string)`

SetAssignedProjects sets AssignedProjects field to given value.

### HasAssignedProjects

`func (o *CreateRunnerRequest) HasAssignedProjects() bool`

HasAssignedProjects returns a boolean if a field has been set.

### GetProjectRunnerAsNode

`func (o *CreateRunnerRequest) GetProjectRunnerAsNode() map[string]bool`

GetProjectRunnerAsNode returns the ProjectRunnerAsNode field if non-nil, zero value otherwise.

### GetProjectRunnerAsNodeOk

`func (o *CreateRunnerRequest) GetProjectRunnerAsNodeOk() (*map[string]bool, bool)`

GetProjectRunnerAsNodeOk returns a tuple with the ProjectRunnerAsNode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectRunnerAsNode

`func (o *CreateRunnerRequest) SetProjectRunnerAsNode(v map[string]bool)`

SetProjectRunnerAsNode sets ProjectRunnerAsNode field to given value.

### HasProjectRunnerAsNode

`func (o *CreateRunnerRequest) HasProjectRunnerAsNode() bool`

HasProjectRunnerAsNode returns a boolean if a field has been set.

### GetInstallationType

`func (o *CreateRunnerRequest) GetInstallationType() string`

GetInstallationType returns the InstallationType field if non-nil, zero value otherwise.

### GetInstallationTypeOk

`func (o *CreateRunnerRequest) GetInstallationTypeOk() (*string, bool)`

GetInstallationTypeOk returns a tuple with the InstallationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstallationType

`func (o *CreateRunnerRequest) SetInstallationType(v string)`

SetInstallationType sets InstallationType field to given value.

### HasInstallationType

`func (o *CreateRunnerRequest) HasInstallationType() bool`

HasInstallationType returns a boolean if a field has been set.

### GetReplicaType

`func (o *CreateRunnerRequest) GetReplicaType() string`

GetReplicaType returns the ReplicaType field if non-nil, zero value otherwise.

### GetReplicaTypeOk

`func (o *CreateRunnerRequest) GetReplicaTypeOk() (*string, bool)`

GetReplicaTypeOk returns a tuple with the ReplicaType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaType

`func (o *CreateRunnerRequest) SetReplicaType(v string)`

SetReplicaType sets ReplicaType field to given value.

### HasReplicaType

`func (o *CreateRunnerRequest) HasReplicaType() bool`

HasReplicaType returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



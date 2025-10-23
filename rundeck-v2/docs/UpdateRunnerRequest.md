# UpdateRunnerRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RunnerId** | **string** |  | 
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**AssignedProjects** | Pointer to **map[string]string** |  | [optional] 
**TagNames** | Pointer to **string** |  | [optional] 
**InstallationType** | Pointer to **string** |  | [optional] 
**ReplicaType** | Pointer to **string** |  | [optional] 

## Methods

### NewUpdateRunnerRequest

`func NewUpdateRunnerRequest(runnerId string, ) *UpdateRunnerRequest`

NewUpdateRunnerRequest instantiates a new UpdateRunnerRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateRunnerRequestWithDefaults

`func NewUpdateRunnerRequestWithDefaults() *UpdateRunnerRequest`

NewUpdateRunnerRequestWithDefaults instantiates a new UpdateRunnerRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRunnerId

`func (o *UpdateRunnerRequest) GetRunnerId() string`

GetRunnerId returns the RunnerId field if non-nil, zero value otherwise.

### GetRunnerIdOk

`func (o *UpdateRunnerRequest) GetRunnerIdOk() (*string, bool)`

GetRunnerIdOk returns a tuple with the RunnerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerId

`func (o *UpdateRunnerRequest) SetRunnerId(v string)`

SetRunnerId sets RunnerId field to given value.


### GetName

`func (o *UpdateRunnerRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateRunnerRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateRunnerRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateRunnerRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *UpdateRunnerRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *UpdateRunnerRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *UpdateRunnerRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *UpdateRunnerRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetAssignedProjects

`func (o *UpdateRunnerRequest) GetAssignedProjects() map[string]string`

GetAssignedProjects returns the AssignedProjects field if non-nil, zero value otherwise.

### GetAssignedProjectsOk

`func (o *UpdateRunnerRequest) GetAssignedProjectsOk() (*map[string]string, bool)`

GetAssignedProjectsOk returns a tuple with the AssignedProjects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssignedProjects

`func (o *UpdateRunnerRequest) SetAssignedProjects(v map[string]string)`

SetAssignedProjects sets AssignedProjects field to given value.

### HasAssignedProjects

`func (o *UpdateRunnerRequest) HasAssignedProjects() bool`

HasAssignedProjects returns a boolean if a field has been set.

### GetTagNames

`func (o *UpdateRunnerRequest) GetTagNames() string`

GetTagNames returns the TagNames field if non-nil, zero value otherwise.

### GetTagNamesOk

`func (o *UpdateRunnerRequest) GetTagNamesOk() (*string, bool)`

GetTagNamesOk returns a tuple with the TagNames field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagNames

`func (o *UpdateRunnerRequest) SetTagNames(v string)`

SetTagNames sets TagNames field to given value.

### HasTagNames

`func (o *UpdateRunnerRequest) HasTagNames() bool`

HasTagNames returns a boolean if a field has been set.

### GetInstallationType

`func (o *UpdateRunnerRequest) GetInstallationType() string`

GetInstallationType returns the InstallationType field if non-nil, zero value otherwise.

### GetInstallationTypeOk

`func (o *UpdateRunnerRequest) GetInstallationTypeOk() (*string, bool)`

GetInstallationTypeOk returns a tuple with the InstallationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstallationType

`func (o *UpdateRunnerRequest) SetInstallationType(v string)`

SetInstallationType sets InstallationType field to given value.

### HasInstallationType

`func (o *UpdateRunnerRequest) HasInstallationType() bool`

HasInstallationType returns a boolean if a field has been set.

### GetReplicaType

`func (o *UpdateRunnerRequest) GetReplicaType() string`

GetReplicaType returns the ReplicaType field if non-nil, zero value otherwise.

### GetReplicaTypeOk

`func (o *UpdateRunnerRequest) GetReplicaTypeOk() (*string, bool)`

GetReplicaTypeOk returns a tuple with the ReplicaType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaType

`func (o *UpdateRunnerRequest) SetReplicaType(v string)`

SetReplicaType sets ReplicaType field to given value.

### HasReplicaType

`func (o *UpdateRunnerRequest) HasReplicaType() bool`

HasReplicaType returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



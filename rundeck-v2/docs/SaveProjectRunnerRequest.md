# SaveProjectRunnerRequest

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
**Data** | Pointer to [**UpdateRunnerRequest**](UpdateRunnerRequest.md) |  | [optional] 

## Methods

### NewSaveProjectRunnerRequest

`func NewSaveProjectRunnerRequest(runnerId string, ) *SaveProjectRunnerRequest`

NewSaveProjectRunnerRequest instantiates a new SaveProjectRunnerRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSaveProjectRunnerRequestWithDefaults

`func NewSaveProjectRunnerRequestWithDefaults() *SaveProjectRunnerRequest`

NewSaveProjectRunnerRequestWithDefaults instantiates a new SaveProjectRunnerRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRunnerId

`func (o *SaveProjectRunnerRequest) GetRunnerId() string`

GetRunnerId returns the RunnerId field if non-nil, zero value otherwise.

### GetRunnerIdOk

`func (o *SaveProjectRunnerRequest) GetRunnerIdOk() (*string, bool)`

GetRunnerIdOk returns a tuple with the RunnerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerId

`func (o *SaveProjectRunnerRequest) SetRunnerId(v string)`

SetRunnerId sets RunnerId field to given value.


### GetName

`func (o *SaveProjectRunnerRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *SaveProjectRunnerRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *SaveProjectRunnerRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *SaveProjectRunnerRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *SaveProjectRunnerRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *SaveProjectRunnerRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *SaveProjectRunnerRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *SaveProjectRunnerRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetAssignedProjects

`func (o *SaveProjectRunnerRequest) GetAssignedProjects() map[string]string`

GetAssignedProjects returns the AssignedProjects field if non-nil, zero value otherwise.

### GetAssignedProjectsOk

`func (o *SaveProjectRunnerRequest) GetAssignedProjectsOk() (*map[string]string, bool)`

GetAssignedProjectsOk returns a tuple with the AssignedProjects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssignedProjects

`func (o *SaveProjectRunnerRequest) SetAssignedProjects(v map[string]string)`

SetAssignedProjects sets AssignedProjects field to given value.

### HasAssignedProjects

`func (o *SaveProjectRunnerRequest) HasAssignedProjects() bool`

HasAssignedProjects returns a boolean if a field has been set.

### GetTagNames

`func (o *SaveProjectRunnerRequest) GetTagNames() string`

GetTagNames returns the TagNames field if non-nil, zero value otherwise.

### GetTagNamesOk

`func (o *SaveProjectRunnerRequest) GetTagNamesOk() (*string, bool)`

GetTagNamesOk returns a tuple with the TagNames field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagNames

`func (o *SaveProjectRunnerRequest) SetTagNames(v string)`

SetTagNames sets TagNames field to given value.

### HasTagNames

`func (o *SaveProjectRunnerRequest) HasTagNames() bool`

HasTagNames returns a boolean if a field has been set.

### GetInstallationType

`func (o *SaveProjectRunnerRequest) GetInstallationType() string`

GetInstallationType returns the InstallationType field if non-nil, zero value otherwise.

### GetInstallationTypeOk

`func (o *SaveProjectRunnerRequest) GetInstallationTypeOk() (*string, bool)`

GetInstallationTypeOk returns a tuple with the InstallationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstallationType

`func (o *SaveProjectRunnerRequest) SetInstallationType(v string)`

SetInstallationType sets InstallationType field to given value.

### HasInstallationType

`func (o *SaveProjectRunnerRequest) HasInstallationType() bool`

HasInstallationType returns a boolean if a field has been set.

### GetReplicaType

`func (o *SaveProjectRunnerRequest) GetReplicaType() string`

GetReplicaType returns the ReplicaType field if non-nil, zero value otherwise.

### GetReplicaTypeOk

`func (o *SaveProjectRunnerRequest) GetReplicaTypeOk() (*string, bool)`

GetReplicaTypeOk returns a tuple with the ReplicaType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaType

`func (o *SaveProjectRunnerRequest) SetReplicaType(v string)`

SetReplicaType sets ReplicaType field to given value.

### HasReplicaType

`func (o *SaveProjectRunnerRequest) HasReplicaType() bool`

HasReplicaType returns a boolean if a field has been set.

### GetData

`func (o *SaveProjectRunnerRequest) GetData() UpdateRunnerRequest`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *SaveProjectRunnerRequest) GetDataOk() (*UpdateRunnerRequest, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *SaveProjectRunnerRequest) SetData(v UpdateRunnerRequest)`

SetData sets Data field to given value.

### HasData

`func (o *SaveProjectRunnerRequest) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



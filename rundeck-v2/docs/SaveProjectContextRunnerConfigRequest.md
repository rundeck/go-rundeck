# SaveProjectContextRunnerConfigRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Project** | Pointer to **string** |  | [optional] 
**Automatic** | Pointer to **bool** |  | [optional] 
**RunnerConfigRequest** | Pointer to [**SaveProjectRunnerConfigRequest**](SaveProjectRunnerConfigRequest.md) |  | [optional] 

## Methods

### NewSaveProjectContextRunnerConfigRequest

`func NewSaveProjectContextRunnerConfigRequest() *SaveProjectContextRunnerConfigRequest`

NewSaveProjectContextRunnerConfigRequest instantiates a new SaveProjectContextRunnerConfigRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSaveProjectContextRunnerConfigRequestWithDefaults

`func NewSaveProjectContextRunnerConfigRequestWithDefaults() *SaveProjectContextRunnerConfigRequest`

NewSaveProjectContextRunnerConfigRequestWithDefaults instantiates a new SaveProjectContextRunnerConfigRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProject

`func (o *SaveProjectContextRunnerConfigRequest) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *SaveProjectContextRunnerConfigRequest) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *SaveProjectContextRunnerConfigRequest) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *SaveProjectContextRunnerConfigRequest) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetAutomatic

`func (o *SaveProjectContextRunnerConfigRequest) GetAutomatic() bool`

GetAutomatic returns the Automatic field if non-nil, zero value otherwise.

### GetAutomaticOk

`func (o *SaveProjectContextRunnerConfigRequest) GetAutomaticOk() (*bool, bool)`

GetAutomaticOk returns a tuple with the Automatic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutomatic

`func (o *SaveProjectContextRunnerConfigRequest) SetAutomatic(v bool)`

SetAutomatic sets Automatic field to given value.

### HasAutomatic

`func (o *SaveProjectContextRunnerConfigRequest) HasAutomatic() bool`

HasAutomatic returns a boolean if a field has been set.

### GetRunnerConfigRequest

`func (o *SaveProjectContextRunnerConfigRequest) GetRunnerConfigRequest() SaveProjectRunnerConfigRequest`

GetRunnerConfigRequest returns the RunnerConfigRequest field if non-nil, zero value otherwise.

### GetRunnerConfigRequestOk

`func (o *SaveProjectContextRunnerConfigRequest) GetRunnerConfigRequestOk() (*SaveProjectRunnerConfigRequest, bool)`

GetRunnerConfigRequestOk returns a tuple with the RunnerConfigRequest field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerConfigRequest

`func (o *SaveProjectContextRunnerConfigRequest) SetRunnerConfigRequest(v SaveProjectRunnerConfigRequest)`

SetRunnerConfigRequest sets RunnerConfigRequest field to given value.

### HasRunnerConfigRequest

`func (o *SaveProjectContextRunnerConfigRequest) HasRunnerConfigRequest() bool`

HasRunnerConfigRequest returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



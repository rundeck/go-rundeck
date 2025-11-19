# SaveProjectRunnerConfigRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Project** | Pointer to **string** |  | [optional] 
**Automatic** | Pointer to **bool** |  | [optional] 

## Methods

### NewSaveProjectRunnerConfigRequest

`func NewSaveProjectRunnerConfigRequest() *SaveProjectRunnerConfigRequest`

NewSaveProjectRunnerConfigRequest instantiates a new SaveProjectRunnerConfigRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSaveProjectRunnerConfigRequestWithDefaults

`func NewSaveProjectRunnerConfigRequestWithDefaults() *SaveProjectRunnerConfigRequest`

NewSaveProjectRunnerConfigRequestWithDefaults instantiates a new SaveProjectRunnerConfigRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProject

`func (o *SaveProjectRunnerConfigRequest) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *SaveProjectRunnerConfigRequest) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *SaveProjectRunnerConfigRequest) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *SaveProjectRunnerConfigRequest) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetAutomatic

`func (o *SaveProjectRunnerConfigRequest) GetAutomatic() bool`

GetAutomatic returns the Automatic field if non-nil, zero value otherwise.

### GetAutomaticOk

`func (o *SaveProjectRunnerConfigRequest) GetAutomaticOk() (*bool, bool)`

GetAutomaticOk returns a tuple with the Automatic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutomatic

`func (o *SaveProjectRunnerConfigRequest) SetAutomatic(v bool)`

SetAutomatic sets Automatic field to given value.

### HasAutomatic

`func (o *SaveProjectRunnerConfigRequest) HasAutomatic() bool`

HasAutomatic returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



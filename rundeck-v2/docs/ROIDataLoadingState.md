# ROIDataLoadingState

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**State** | Pointer to **string** | The state of asynch loading of the remote file, one of AVAILABLE_REMOTE or PENDING_LOCAL | [optional] 

## Methods

### NewROIDataLoadingState

`func NewROIDataLoadingState() *ROIDataLoadingState`

NewROIDataLoadingState instantiates a new ROIDataLoadingState object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewROIDataLoadingStateWithDefaults

`func NewROIDataLoadingStateWithDefaults() *ROIDataLoadingState`

NewROIDataLoadingStateWithDefaults instantiates a new ROIDataLoadingState object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetState

`func (o *ROIDataLoadingState) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ROIDataLoadingState) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ROIDataLoadingState) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *ROIDataLoadingState) HasState() bool`

HasState returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ResultDataLoadingState

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**State** | Pointer to **string** | The state of asynch loading of the remote file, one of AVAILABLE_REMOTE or PENDING_LOCAL | [optional] 

## Methods

### NewResultDataLoadingState

`func NewResultDataLoadingState() *ResultDataLoadingState`

NewResultDataLoadingState instantiates a new ResultDataLoadingState object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResultDataLoadingStateWithDefaults

`func NewResultDataLoadingStateWithDefaults() *ResultDataLoadingState`

NewResultDataLoadingStateWithDefaults instantiates a new ResultDataLoadingState object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetState

`func (o *ResultDataLoadingState) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ResultDataLoadingState) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ResultDataLoadingState) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *ResultDataLoadingState) HasState() bool`

HasState returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



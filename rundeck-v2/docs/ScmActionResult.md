# ScmActionResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | Pointer to **string** | Status message | [optional] 
**Success** | Pointer to **bool** | true if successful, false otherwise | [optional] 
**NextAction** | Pointer to **string** | Name of the next &#x60;action&#x60; that should be invoked. | [optional] 
**ValidationErrors** | Pointer to **map[string]string** | Validation errors, keyed by input field name. | [optional] 

## Methods

### NewScmActionResult

`func NewScmActionResult() *ScmActionResult`

NewScmActionResult instantiates a new ScmActionResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmActionResultWithDefaults

`func NewScmActionResultWithDefaults() *ScmActionResult`

NewScmActionResultWithDefaults instantiates a new ScmActionResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *ScmActionResult) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ScmActionResult) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ScmActionResult) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *ScmActionResult) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetSuccess

`func (o *ScmActionResult) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *ScmActionResult) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *ScmActionResult) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *ScmActionResult) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetNextAction

`func (o *ScmActionResult) GetNextAction() string`

GetNextAction returns the NextAction field if non-nil, zero value otherwise.

### GetNextActionOk

`func (o *ScmActionResult) GetNextActionOk() (*string, bool)`

GetNextActionOk returns a tuple with the NextAction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextAction

`func (o *ScmActionResult) SetNextAction(v string)`

SetNextAction sets NextAction field to given value.

### HasNextAction

`func (o *ScmActionResult) HasNextAction() bool`

HasNextAction returns a boolean if a field has been set.

### GetValidationErrors

`func (o *ScmActionResult) GetValidationErrors() map[string]string`

GetValidationErrors returns the ValidationErrors field if non-nil, zero value otherwise.

### GetValidationErrorsOk

`func (o *ScmActionResult) GetValidationErrorsOk() (*map[string]string, bool)`

GetValidationErrorsOk returns a tuple with the ValidationErrors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValidationErrors

`func (o *ScmActionResult) SetValidationErrors(v map[string]string)`

SetValidationErrors sets ValidationErrors field to given value.

### HasValidationErrors

`func (o *ScmActionResult) HasValidationErrors() bool`

HasValidationErrors returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



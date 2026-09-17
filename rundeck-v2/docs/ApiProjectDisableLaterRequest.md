# ApiProjectDisableLaterRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | Pointer to **string** | Time duration expression.  A series of: an integer followed by a unit.  Units: * &#x60;s&#x60; - seconds (default) * &#x60;m&#x60; - minutes * &#x60;h&#x60; - hours * &#x60;d&#x60; - days * &#x60;w&#x60; - weeks * &#x60;y&#x60; - years.  Examples: &#x60;1d12h&#x60;, &#x60;3600&#x60; (defaults to seconds), &#x60;15m30s&#x60;.  | [optional] 
**Type** | Pointer to **string** | Mode to change, one of &#x60;executions&#x60; or &#x60;schedule&#x60; | [optional] 
**Command** | Pointer to [**ProjectExecutionModeLaterCommand**](ProjectExecutionModeLaterCommand.md) |  | [optional] 

## Methods

### NewApiProjectDisableLaterRequest

`func NewApiProjectDisableLaterRequest() *ApiProjectDisableLaterRequest`

NewApiProjectDisableLaterRequest instantiates a new ApiProjectDisableLaterRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiProjectDisableLaterRequestWithDefaults

`func NewApiProjectDisableLaterRequestWithDefaults() *ApiProjectDisableLaterRequest`

NewApiProjectDisableLaterRequestWithDefaults instantiates a new ApiProjectDisableLaterRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *ApiProjectDisableLaterRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ApiProjectDisableLaterRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ApiProjectDisableLaterRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *ApiProjectDisableLaterRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetType

`func (o *ApiProjectDisableLaterRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ApiProjectDisableLaterRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ApiProjectDisableLaterRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ApiProjectDisableLaterRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetCommand

`func (o *ApiProjectDisableLaterRequest) GetCommand() ProjectExecutionModeLaterCommand`

GetCommand returns the Command field if non-nil, zero value otherwise.

### GetCommandOk

`func (o *ApiProjectDisableLaterRequest) GetCommandOk() (*ProjectExecutionModeLaterCommand, bool)`

GetCommandOk returns a tuple with the Command field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommand

`func (o *ApiProjectDisableLaterRequest) SetCommand(v ProjectExecutionModeLaterCommand)`

SetCommand sets Command field to given value.

### HasCommand

`func (o *ApiProjectDisableLaterRequest) HasCommand() bool`

HasCommand returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



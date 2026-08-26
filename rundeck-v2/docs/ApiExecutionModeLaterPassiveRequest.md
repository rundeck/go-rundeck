# ApiExecutionModeLaterPassiveRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | Pointer to **string** | Time duration expression.  A series of: an integer followed by a unit.  Units: * &#x60;s&#x60; - seconds (default) * &#x60;m&#x60; - minutes * &#x60;h&#x60; - hours * &#x60;d&#x60; - days * &#x60;w&#x60; - weeks * &#x60;y&#x60; - years.  Examples: &#x60;1d12h&#x60;, &#x60;3600&#x60; (defaults to seconds), &#x60;15m30s&#x60;.  | [optional] 
**Command** | Pointer to [**ExecutionModeLaterCommand**](ExecutionModeLaterCommand.md) |  | [optional] 

## Methods

### NewApiExecutionModeLaterPassiveRequest

`func NewApiExecutionModeLaterPassiveRequest() *ApiExecutionModeLaterPassiveRequest`

NewApiExecutionModeLaterPassiveRequest instantiates a new ApiExecutionModeLaterPassiveRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiExecutionModeLaterPassiveRequestWithDefaults

`func NewApiExecutionModeLaterPassiveRequestWithDefaults() *ApiExecutionModeLaterPassiveRequest`

NewApiExecutionModeLaterPassiveRequestWithDefaults instantiates a new ApiExecutionModeLaterPassiveRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *ApiExecutionModeLaterPassiveRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ApiExecutionModeLaterPassiveRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ApiExecutionModeLaterPassiveRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *ApiExecutionModeLaterPassiveRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetCommand

`func (o *ApiExecutionModeLaterPassiveRequest) GetCommand() ExecutionModeLaterCommand`

GetCommand returns the Command field if non-nil, zero value otherwise.

### GetCommandOk

`func (o *ApiExecutionModeLaterPassiveRequest) GetCommandOk() (*ExecutionModeLaterCommand, bool)`

GetCommandOk returns a tuple with the Command field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommand

`func (o *ApiExecutionModeLaterPassiveRequest) SetCommand(v ExecutionModeLaterCommand)`

SetCommand sets Command field to given value.

### HasCommand

`func (o *ApiExecutionModeLaterPassiveRequest) HasCommand() bool`

HasCommand returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



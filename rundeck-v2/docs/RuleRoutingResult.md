# RuleRoutingResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RuleEvaluation** | Pointer to [**RuleEvaluation**](RuleEvaluation.md) |  | [optional] 
**JobRunStatus** | Pointer to [**JobRunStatus**](JobRunStatus.md) |  | [optional] 
**JobId** | Pointer to **string** |  | [optional] 
**ExecutionId** | Pointer to **string** |  | [optional] 
**ErrorMsg** | Pointer to **string** |  | [optional] 
**RenderedOptions** | Pointer to **map[string]string** |  | [optional] 

## Methods

### NewRuleRoutingResult

`func NewRuleRoutingResult() *RuleRoutingResult`

NewRuleRoutingResult instantiates a new RuleRoutingResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRuleRoutingResultWithDefaults

`func NewRuleRoutingResultWithDefaults() *RuleRoutingResult`

NewRuleRoutingResultWithDefaults instantiates a new RuleRoutingResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRuleEvaluation

`func (o *RuleRoutingResult) GetRuleEvaluation() RuleEvaluation`

GetRuleEvaluation returns the RuleEvaluation field if non-nil, zero value otherwise.

### GetRuleEvaluationOk

`func (o *RuleRoutingResult) GetRuleEvaluationOk() (*RuleEvaluation, bool)`

GetRuleEvaluationOk returns a tuple with the RuleEvaluation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleEvaluation

`func (o *RuleRoutingResult) SetRuleEvaluation(v RuleEvaluation)`

SetRuleEvaluation sets RuleEvaluation field to given value.

### HasRuleEvaluation

`func (o *RuleRoutingResult) HasRuleEvaluation() bool`

HasRuleEvaluation returns a boolean if a field has been set.

### GetJobRunStatus

`func (o *RuleRoutingResult) GetJobRunStatus() JobRunStatus`

GetJobRunStatus returns the JobRunStatus field if non-nil, zero value otherwise.

### GetJobRunStatusOk

`func (o *RuleRoutingResult) GetJobRunStatusOk() (*JobRunStatus, bool)`

GetJobRunStatusOk returns a tuple with the JobRunStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobRunStatus

`func (o *RuleRoutingResult) SetJobRunStatus(v JobRunStatus)`

SetJobRunStatus sets JobRunStatus field to given value.

### HasJobRunStatus

`func (o *RuleRoutingResult) HasJobRunStatus() bool`

HasJobRunStatus returns a boolean if a field has been set.

### GetJobId

`func (o *RuleRoutingResult) GetJobId() string`

GetJobId returns the JobId field if non-nil, zero value otherwise.

### GetJobIdOk

`func (o *RuleRoutingResult) GetJobIdOk() (*string, bool)`

GetJobIdOk returns a tuple with the JobId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobId

`func (o *RuleRoutingResult) SetJobId(v string)`

SetJobId sets JobId field to given value.

### HasJobId

`func (o *RuleRoutingResult) HasJobId() bool`

HasJobId returns a boolean if a field has been set.

### GetExecutionId

`func (o *RuleRoutingResult) GetExecutionId() string`

GetExecutionId returns the ExecutionId field if non-nil, zero value otherwise.

### GetExecutionIdOk

`func (o *RuleRoutingResult) GetExecutionIdOk() (*string, bool)`

GetExecutionIdOk returns a tuple with the ExecutionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutionId

`func (o *RuleRoutingResult) SetExecutionId(v string)`

SetExecutionId sets ExecutionId field to given value.

### HasExecutionId

`func (o *RuleRoutingResult) HasExecutionId() bool`

HasExecutionId returns a boolean if a field has been set.

### GetErrorMsg

`func (o *RuleRoutingResult) GetErrorMsg() string`

GetErrorMsg returns the ErrorMsg field if non-nil, zero value otherwise.

### GetErrorMsgOk

`func (o *RuleRoutingResult) GetErrorMsgOk() (*string, bool)`

GetErrorMsgOk returns a tuple with the ErrorMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorMsg

`func (o *RuleRoutingResult) SetErrorMsg(v string)`

SetErrorMsg sets ErrorMsg field to given value.

### HasErrorMsg

`func (o *RuleRoutingResult) HasErrorMsg() bool`

HasErrorMsg returns a boolean if a field has been set.

### GetRenderedOptions

`func (o *RuleRoutingResult) GetRenderedOptions() map[string]string`

GetRenderedOptions returns the RenderedOptions field if non-nil, zero value otherwise.

### GetRenderedOptionsOk

`func (o *RuleRoutingResult) GetRenderedOptionsOk() (*map[string]string, bool)`

GetRenderedOptionsOk returns a tuple with the RenderedOptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenderedOptions

`func (o *RuleRoutingResult) SetRenderedOptions(v map[string]string)`

SetRenderedOptions sets RenderedOptions field to given value.

### HasRenderedOptions

`func (o *RuleRoutingResult) HasRenderedOptions() bool`

HasRenderedOptions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



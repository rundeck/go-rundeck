# ConditionEvaluation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Satisfied** | Pointer to **bool** |  | [optional] 
**Value** | Pointer to **map[string]interface{}** |  | [optional] 
**Condition** | Pointer to [**Condition**](Condition.md) |  | [optional] 
**Error** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewConditionEvaluation

`func NewConditionEvaluation() *ConditionEvaluation`

NewConditionEvaluation instantiates a new ConditionEvaluation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConditionEvaluationWithDefaults

`func NewConditionEvaluationWithDefaults() *ConditionEvaluation`

NewConditionEvaluationWithDefaults instantiates a new ConditionEvaluation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSatisfied

`func (o *ConditionEvaluation) GetSatisfied() bool`

GetSatisfied returns the Satisfied field if non-nil, zero value otherwise.

### GetSatisfiedOk

`func (o *ConditionEvaluation) GetSatisfiedOk() (*bool, bool)`

GetSatisfiedOk returns a tuple with the Satisfied field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSatisfied

`func (o *ConditionEvaluation) SetSatisfied(v bool)`

SetSatisfied sets Satisfied field to given value.

### HasSatisfied

`func (o *ConditionEvaluation) HasSatisfied() bool`

HasSatisfied returns a boolean if a field has been set.

### GetValue

`func (o *ConditionEvaluation) GetValue() map[string]interface{}`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ConditionEvaluation) GetValueOk() (*map[string]interface{}, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ConditionEvaluation) SetValue(v map[string]interface{})`

SetValue sets Value field to given value.

### HasValue

`func (o *ConditionEvaluation) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetCondition

`func (o *ConditionEvaluation) GetCondition() Condition`

GetCondition returns the Condition field if non-nil, zero value otherwise.

### GetConditionOk

`func (o *ConditionEvaluation) GetConditionOk() (*Condition, bool)`

GetConditionOk returns a tuple with the Condition field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCondition

`func (o *ConditionEvaluation) SetCondition(v Condition)`

SetCondition sets Condition field to given value.

### HasCondition

`func (o *ConditionEvaluation) HasCondition() bool`

HasCondition returns a boolean if a field has been set.

### GetError

`func (o *ConditionEvaluation) GetError() map[string]interface{}`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *ConditionEvaluation) GetErrorOk() (*map[string]interface{}, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *ConditionEvaluation) SetError(v map[string]interface{})`

SetError sets Error field to given value.

### HasError

`func (o *ConditionEvaluation) HasError() bool`

HasError returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



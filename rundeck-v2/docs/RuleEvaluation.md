# RuleEvaluation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Satisfied** | Pointer to **bool** |  | [optional] 
**Rule** | Pointer to [**RoutingRule**](RoutingRule.md) |  | [optional] 
**ConditionEvaluations** | Pointer to [**[]ConditionEvaluation**](ConditionEvaluation.md) |  | [optional] 

## Methods

### NewRuleEvaluation

`func NewRuleEvaluation() *RuleEvaluation`

NewRuleEvaluation instantiates a new RuleEvaluation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRuleEvaluationWithDefaults

`func NewRuleEvaluationWithDefaults() *RuleEvaluation`

NewRuleEvaluationWithDefaults instantiates a new RuleEvaluation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSatisfied

`func (o *RuleEvaluation) GetSatisfied() bool`

GetSatisfied returns the Satisfied field if non-nil, zero value otherwise.

### GetSatisfiedOk

`func (o *RuleEvaluation) GetSatisfiedOk() (*bool, bool)`

GetSatisfiedOk returns a tuple with the Satisfied field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSatisfied

`func (o *RuleEvaluation) SetSatisfied(v bool)`

SetSatisfied sets Satisfied field to given value.

### HasSatisfied

`func (o *RuleEvaluation) HasSatisfied() bool`

HasSatisfied returns a boolean if a field has been set.

### GetRule

`func (o *RuleEvaluation) GetRule() RoutingRule`

GetRule returns the Rule field if non-nil, zero value otherwise.

### GetRuleOk

`func (o *RuleEvaluation) GetRuleOk() (*RoutingRule, bool)`

GetRuleOk returns a tuple with the Rule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRule

`func (o *RuleEvaluation) SetRule(v RoutingRule)`

SetRule sets Rule field to given value.

### HasRule

`func (o *RuleEvaluation) HasRule() bool`

HasRule returns a boolean if a field has been set.

### GetConditionEvaluations

`func (o *RuleEvaluation) GetConditionEvaluations() []ConditionEvaluation`

GetConditionEvaluations returns the ConditionEvaluations field if non-nil, zero value otherwise.

### GetConditionEvaluationsOk

`func (o *RuleEvaluation) GetConditionEvaluationsOk() (*[]ConditionEvaluation, bool)`

GetConditionEvaluationsOk returns a tuple with the ConditionEvaluations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConditionEvaluations

`func (o *RuleEvaluation) SetConditionEvaluations(v []ConditionEvaluation)`

SetConditionEvaluations sets ConditionEvaluations field to given value.

### HasConditionEvaluations

`func (o *RuleEvaluation) HasConditionEvaluations() bool`

HasConditionEvaluations returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



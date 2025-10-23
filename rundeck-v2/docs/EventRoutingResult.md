# EventRoutingResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Event** | Pointer to [**RouterEvent**](RouterEvent.md) |  | [optional] 
**RuleRoutingResults** | Pointer to [**[]RuleRoutingResult**](RuleRoutingResult.md) |  | [optional] 

## Methods

### NewEventRoutingResult

`func NewEventRoutingResult() *EventRoutingResult`

NewEventRoutingResult instantiates a new EventRoutingResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEventRoutingResultWithDefaults

`func NewEventRoutingResultWithDefaults() *EventRoutingResult`

NewEventRoutingResultWithDefaults instantiates a new EventRoutingResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEvent

`func (o *EventRoutingResult) GetEvent() RouterEvent`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *EventRoutingResult) GetEventOk() (*RouterEvent, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *EventRoutingResult) SetEvent(v RouterEvent)`

SetEvent sets Event field to given value.

### HasEvent

`func (o *EventRoutingResult) HasEvent() bool`

HasEvent returns a boolean if a field has been set.

### GetRuleRoutingResults

`func (o *EventRoutingResult) GetRuleRoutingResults() []RuleRoutingResult`

GetRuleRoutingResults returns the RuleRoutingResults field if non-nil, zero value otherwise.

### GetRuleRoutingResultsOk

`func (o *EventRoutingResult) GetRuleRoutingResultsOk() (*[]RuleRoutingResult, bool)`

GetRuleRoutingResultsOk returns a tuple with the RuleRoutingResults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleRoutingResults

`func (o *EventRoutingResult) SetRuleRoutingResults(v []RuleRoutingResult)`

SetRuleRoutingResults sets RuleRoutingResults field to given value.

### HasRuleRoutingResults

`func (o *EventRoutingResult) HasRuleRoutingResults() bool`

HasRuleRoutingResults returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



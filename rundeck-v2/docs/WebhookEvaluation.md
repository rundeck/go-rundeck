# WebhookEvaluation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Time** | Pointer to **time.Time** |  | [optional] 
**Event** | Pointer to **map[string]interface{}** |  | [optional] 
**BatchKey** | Pointer to **string** |  | [optional] 
**Error** | Pointer to **string** |  | [optional] 
**RoutingResults** | Pointer to [**[]EventRoutingResult**](EventRoutingResult.md) |  | [optional] 

## Methods

### NewWebhookEvaluation

`func NewWebhookEvaluation() *WebhookEvaluation`

NewWebhookEvaluation instantiates a new WebhookEvaluation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookEvaluationWithDefaults

`func NewWebhookEvaluationWithDefaults() *WebhookEvaluation`

NewWebhookEvaluationWithDefaults instantiates a new WebhookEvaluation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *WebhookEvaluation) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *WebhookEvaluation) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *WebhookEvaluation) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *WebhookEvaluation) HasId() bool`

HasId returns a boolean if a field has been set.

### GetTime

`func (o *WebhookEvaluation) GetTime() time.Time`

GetTime returns the Time field if non-nil, zero value otherwise.

### GetTimeOk

`func (o *WebhookEvaluation) GetTimeOk() (*time.Time, bool)`

GetTimeOk returns a tuple with the Time field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTime

`func (o *WebhookEvaluation) SetTime(v time.Time)`

SetTime sets Time field to given value.

### HasTime

`func (o *WebhookEvaluation) HasTime() bool`

HasTime returns a boolean if a field has been set.

### GetEvent

`func (o *WebhookEvaluation) GetEvent() map[string]interface{}`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *WebhookEvaluation) GetEventOk() (*map[string]interface{}, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *WebhookEvaluation) SetEvent(v map[string]interface{})`

SetEvent sets Event field to given value.

### HasEvent

`func (o *WebhookEvaluation) HasEvent() bool`

HasEvent returns a boolean if a field has been set.

### GetBatchKey

`func (o *WebhookEvaluation) GetBatchKey() string`

GetBatchKey returns the BatchKey field if non-nil, zero value otherwise.

### GetBatchKeyOk

`func (o *WebhookEvaluation) GetBatchKeyOk() (*string, bool)`

GetBatchKeyOk returns a tuple with the BatchKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBatchKey

`func (o *WebhookEvaluation) SetBatchKey(v string)`

SetBatchKey sets BatchKey field to given value.

### HasBatchKey

`func (o *WebhookEvaluation) HasBatchKey() bool`

HasBatchKey returns a boolean if a field has been set.

### GetError

`func (o *WebhookEvaluation) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *WebhookEvaluation) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *WebhookEvaluation) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *WebhookEvaluation) HasError() bool`

HasError returns a boolean if a field has been set.

### GetRoutingResults

`func (o *WebhookEvaluation) GetRoutingResults() []EventRoutingResult`

GetRoutingResults returns the RoutingResults field if non-nil, zero value otherwise.

### GetRoutingResultsOk

`func (o *WebhookEvaluation) GetRoutingResultsOk() (*[]EventRoutingResult, bool)`

GetRoutingResultsOk returns a tuple with the RoutingResults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoutingResults

`func (o *WebhookEvaluation) SetRoutingResults(v []EventRoutingResult)`

SetRoutingResults sets RoutingResults field to given value.

### HasRoutingResults

`func (o *WebhookEvaluation) HasRoutingResults() bool`

HasRoutingResults returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



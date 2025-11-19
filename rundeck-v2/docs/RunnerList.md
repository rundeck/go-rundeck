# RunnerList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Runners** | Pointer to [**[]RunnerSummary**](RunnerSummary.md) |  | [optional] 

## Methods

### NewRunnerList

`func NewRunnerList() *RunnerList`

NewRunnerList instantiates a new RunnerList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRunnerListWithDefaults

`func NewRunnerListWithDefaults() *RunnerList`

NewRunnerListWithDefaults instantiates a new RunnerList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRunners

`func (o *RunnerList) GetRunners() []RunnerSummary`

GetRunners returns the Runners field if non-nil, zero value otherwise.

### GetRunnersOk

`func (o *RunnerList) GetRunnersOk() (*[]RunnerSummary, bool)`

GetRunnersOk returns a tuple with the Runners field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunners

`func (o *RunnerList) SetRunners(v []RunnerSummary)`

SetRunners sets Runners field to given value.

### HasRunners

`func (o *RunnerList) HasRunners() bool`

HasRunners returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



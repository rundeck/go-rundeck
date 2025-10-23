# UpdateRunnerNodeDispatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RunnerId** | **string** |  | 
**RunnerAsNodeEnabled** | Pointer to **bool** |  | [optional] 
**RemoteNodeDispatch** | Pointer to **bool** |  | [optional] 
**RunnerNodeFilter** | Pointer to **string** |  | [optional] 

## Methods

### NewUpdateRunnerNodeDispatchRequest

`func NewUpdateRunnerNodeDispatchRequest(runnerId string, ) *UpdateRunnerNodeDispatchRequest`

NewUpdateRunnerNodeDispatchRequest instantiates a new UpdateRunnerNodeDispatchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateRunnerNodeDispatchRequestWithDefaults

`func NewUpdateRunnerNodeDispatchRequestWithDefaults() *UpdateRunnerNodeDispatchRequest`

NewUpdateRunnerNodeDispatchRequestWithDefaults instantiates a new UpdateRunnerNodeDispatchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRunnerId

`func (o *UpdateRunnerNodeDispatchRequest) GetRunnerId() string`

GetRunnerId returns the RunnerId field if non-nil, zero value otherwise.

### GetRunnerIdOk

`func (o *UpdateRunnerNodeDispatchRequest) GetRunnerIdOk() (*string, bool)`

GetRunnerIdOk returns a tuple with the RunnerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerId

`func (o *UpdateRunnerNodeDispatchRequest) SetRunnerId(v string)`

SetRunnerId sets RunnerId field to given value.


### GetRunnerAsNodeEnabled

`func (o *UpdateRunnerNodeDispatchRequest) GetRunnerAsNodeEnabled() bool`

GetRunnerAsNodeEnabled returns the RunnerAsNodeEnabled field if non-nil, zero value otherwise.

### GetRunnerAsNodeEnabledOk

`func (o *UpdateRunnerNodeDispatchRequest) GetRunnerAsNodeEnabledOk() (*bool, bool)`

GetRunnerAsNodeEnabledOk returns a tuple with the RunnerAsNodeEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerAsNodeEnabled

`func (o *UpdateRunnerNodeDispatchRequest) SetRunnerAsNodeEnabled(v bool)`

SetRunnerAsNodeEnabled sets RunnerAsNodeEnabled field to given value.

### HasRunnerAsNodeEnabled

`func (o *UpdateRunnerNodeDispatchRequest) HasRunnerAsNodeEnabled() bool`

HasRunnerAsNodeEnabled returns a boolean if a field has been set.

### GetRemoteNodeDispatch

`func (o *UpdateRunnerNodeDispatchRequest) GetRemoteNodeDispatch() bool`

GetRemoteNodeDispatch returns the RemoteNodeDispatch field if non-nil, zero value otherwise.

### GetRemoteNodeDispatchOk

`func (o *UpdateRunnerNodeDispatchRequest) GetRemoteNodeDispatchOk() (*bool, bool)`

GetRemoteNodeDispatchOk returns a tuple with the RemoteNodeDispatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoteNodeDispatch

`func (o *UpdateRunnerNodeDispatchRequest) SetRemoteNodeDispatch(v bool)`

SetRemoteNodeDispatch sets RemoteNodeDispatch field to given value.

### HasRemoteNodeDispatch

`func (o *UpdateRunnerNodeDispatchRequest) HasRemoteNodeDispatch() bool`

HasRemoteNodeDispatch returns a boolean if a field has been set.

### GetRunnerNodeFilter

`func (o *UpdateRunnerNodeDispatchRequest) GetRunnerNodeFilter() string`

GetRunnerNodeFilter returns the RunnerNodeFilter field if non-nil, zero value otherwise.

### GetRunnerNodeFilterOk

`func (o *UpdateRunnerNodeDispatchRequest) GetRunnerNodeFilterOk() (*string, bool)`

GetRunnerNodeFilterOk returns a tuple with the RunnerNodeFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerNodeFilter

`func (o *UpdateRunnerNodeDispatchRequest) SetRunnerNodeFilter(v string)`

SetRunnerNodeFilter sets RunnerNodeFilter field to given value.

### HasRunnerNodeFilter

`func (o *UpdateRunnerNodeDispatchRequest) HasRunnerNodeFilter() bool`

HasRunnerNodeFilter returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



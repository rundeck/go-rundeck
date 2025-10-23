# SaveProjectRunnerNodeDispatchSettingsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RunnerId** | **string** |  | 
**RunnerAsNodeEnabled** | Pointer to **bool** |  | [optional] 
**RemoteNodeDispatch** | Pointer to **bool** |  | [optional] 
**RunnerNodeFilter** | Pointer to **string** |  | [optional] 
**Data** | Pointer to [**UpdateRunnerNodeDispatchRequest**](UpdateRunnerNodeDispatchRequest.md) |  | [optional] 

## Methods

### NewSaveProjectRunnerNodeDispatchSettingsRequest

`func NewSaveProjectRunnerNodeDispatchSettingsRequest(runnerId string, ) *SaveProjectRunnerNodeDispatchSettingsRequest`

NewSaveProjectRunnerNodeDispatchSettingsRequest instantiates a new SaveProjectRunnerNodeDispatchSettingsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSaveProjectRunnerNodeDispatchSettingsRequestWithDefaults

`func NewSaveProjectRunnerNodeDispatchSettingsRequestWithDefaults() *SaveProjectRunnerNodeDispatchSettingsRequest`

NewSaveProjectRunnerNodeDispatchSettingsRequestWithDefaults instantiates a new SaveProjectRunnerNodeDispatchSettingsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRunnerId

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetRunnerId() string`

GetRunnerId returns the RunnerId field if non-nil, zero value otherwise.

### GetRunnerIdOk

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetRunnerIdOk() (*string, bool)`

GetRunnerIdOk returns a tuple with the RunnerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerId

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) SetRunnerId(v string)`

SetRunnerId sets RunnerId field to given value.


### GetRunnerAsNodeEnabled

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetRunnerAsNodeEnabled() bool`

GetRunnerAsNodeEnabled returns the RunnerAsNodeEnabled field if non-nil, zero value otherwise.

### GetRunnerAsNodeEnabledOk

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetRunnerAsNodeEnabledOk() (*bool, bool)`

GetRunnerAsNodeEnabledOk returns a tuple with the RunnerAsNodeEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerAsNodeEnabled

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) SetRunnerAsNodeEnabled(v bool)`

SetRunnerAsNodeEnabled sets RunnerAsNodeEnabled field to given value.

### HasRunnerAsNodeEnabled

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) HasRunnerAsNodeEnabled() bool`

HasRunnerAsNodeEnabled returns a boolean if a field has been set.

### GetRemoteNodeDispatch

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetRemoteNodeDispatch() bool`

GetRemoteNodeDispatch returns the RemoteNodeDispatch field if non-nil, zero value otherwise.

### GetRemoteNodeDispatchOk

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetRemoteNodeDispatchOk() (*bool, bool)`

GetRemoteNodeDispatchOk returns a tuple with the RemoteNodeDispatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoteNodeDispatch

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) SetRemoteNodeDispatch(v bool)`

SetRemoteNodeDispatch sets RemoteNodeDispatch field to given value.

### HasRemoteNodeDispatch

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) HasRemoteNodeDispatch() bool`

HasRemoteNodeDispatch returns a boolean if a field has been set.

### GetRunnerNodeFilter

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetRunnerNodeFilter() string`

GetRunnerNodeFilter returns the RunnerNodeFilter field if non-nil, zero value otherwise.

### GetRunnerNodeFilterOk

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetRunnerNodeFilterOk() (*string, bool)`

GetRunnerNodeFilterOk returns a tuple with the RunnerNodeFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerNodeFilter

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) SetRunnerNodeFilter(v string)`

SetRunnerNodeFilter sets RunnerNodeFilter field to given value.

### HasRunnerNodeFilter

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) HasRunnerNodeFilter() bool`

HasRunnerNodeFilter returns a boolean if a field has been set.

### GetData

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetData() UpdateRunnerNodeDispatchRequest`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) GetDataOk() (*UpdateRunnerNodeDispatchRequest, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) SetData(v UpdateRunnerNodeDispatchRequest)`

SetData sets Data field to given value.

### HasData

`func (o *SaveProjectRunnerNodeDispatchSettingsRequest) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# PingResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RunnerId** | Pointer to **string** |  | [optional] 
**Completed** | Pointer to **bool** |  | [optional] 
**Message** | Pointer to **string** |  | [optional] 
**Iserror** | Pointer to **bool** |  | [optional] 

## Methods

### NewPingResponse

`func NewPingResponse() *PingResponse`

NewPingResponse instantiates a new PingResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPingResponseWithDefaults

`func NewPingResponseWithDefaults() *PingResponse`

NewPingResponseWithDefaults instantiates a new PingResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRunnerId

`func (o *PingResponse) GetRunnerId() string`

GetRunnerId returns the RunnerId field if non-nil, zero value otherwise.

### GetRunnerIdOk

`func (o *PingResponse) GetRunnerIdOk() (*string, bool)`

GetRunnerIdOk returns a tuple with the RunnerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerId

`func (o *PingResponse) SetRunnerId(v string)`

SetRunnerId sets RunnerId field to given value.

### HasRunnerId

`func (o *PingResponse) HasRunnerId() bool`

HasRunnerId returns a boolean if a field has been set.

### GetCompleted

`func (o *PingResponse) GetCompleted() bool`

GetCompleted returns the Completed field if non-nil, zero value otherwise.

### GetCompletedOk

`func (o *PingResponse) GetCompletedOk() (*bool, bool)`

GetCompletedOk returns a tuple with the Completed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompleted

`func (o *PingResponse) SetCompleted(v bool)`

SetCompleted sets Completed field to given value.

### HasCompleted

`func (o *PingResponse) HasCompleted() bool`

HasCompleted returns a boolean if a field has been set.

### GetMessage

`func (o *PingResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *PingResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *PingResponse) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *PingResponse) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetIserror

`func (o *PingResponse) GetIserror() bool`

GetIserror returns the Iserror field if non-nil, zero value otherwise.

### GetIserrorOk

`func (o *PingResponse) GetIserrorOk() (*bool, bool)`

GetIserrorOk returns a tuple with the Iserror field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIserror

`func (o *PingResponse) SetIserror(v bool)`

SetIserror sets Iserror field to given value.

### HasIserror

`func (o *PingResponse) HasIserror() bool`

HasIserror returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Throwable

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | Pointer to **string** |  | [optional] 
**LocalizedMessage** | Pointer to **string** |  | [optional] 
**Cause** | Pointer to [**Throwable**](Throwable.md) |  | [optional] 
**StackTrace** | Pointer to [**[]StackTraceElement**](StackTraceElement.md) |  | [optional] 
**Suppressed** | Pointer to [**[]Throwable**](Throwable.md) |  | [optional] 

## Methods

### NewThrowable

`func NewThrowable() *Throwable`

NewThrowable instantiates a new Throwable object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewThrowableWithDefaults

`func NewThrowableWithDefaults() *Throwable`

NewThrowableWithDefaults instantiates a new Throwable object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *Throwable) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *Throwable) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *Throwable) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *Throwable) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetLocalizedMessage

`func (o *Throwable) GetLocalizedMessage() string`

GetLocalizedMessage returns the LocalizedMessage field if non-nil, zero value otherwise.

### GetLocalizedMessageOk

`func (o *Throwable) GetLocalizedMessageOk() (*string, bool)`

GetLocalizedMessageOk returns a tuple with the LocalizedMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocalizedMessage

`func (o *Throwable) SetLocalizedMessage(v string)`

SetLocalizedMessage sets LocalizedMessage field to given value.

### HasLocalizedMessage

`func (o *Throwable) HasLocalizedMessage() bool`

HasLocalizedMessage returns a boolean if a field has been set.

### GetCause

`func (o *Throwable) GetCause() Throwable`

GetCause returns the Cause field if non-nil, zero value otherwise.

### GetCauseOk

`func (o *Throwable) GetCauseOk() (*Throwable, bool)`

GetCauseOk returns a tuple with the Cause field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCause

`func (o *Throwable) SetCause(v Throwable)`

SetCause sets Cause field to given value.

### HasCause

`func (o *Throwable) HasCause() bool`

HasCause returns a boolean if a field has been set.

### GetStackTrace

`func (o *Throwable) GetStackTrace() []StackTraceElement`

GetStackTrace returns the StackTrace field if non-nil, zero value otherwise.

### GetStackTraceOk

`func (o *Throwable) GetStackTraceOk() (*[]StackTraceElement, bool)`

GetStackTraceOk returns a tuple with the StackTrace field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStackTrace

`func (o *Throwable) SetStackTrace(v []StackTraceElement)`

SetStackTrace sets StackTrace field to given value.

### HasStackTrace

`func (o *Throwable) HasStackTrace() bool`

HasStackTrace returns a boolean if a field has been set.

### GetSuppressed

`func (o *Throwable) GetSuppressed() []Throwable`

GetSuppressed returns the Suppressed field if non-nil, zero value otherwise.

### GetSuppressedOk

`func (o *Throwable) GetSuppressedOk() (*[]Throwable, bool)`

GetSuppressedOk returns a tuple with the Suppressed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuppressed

`func (o *Throwable) SetSuppressed(v []Throwable)`

SetSuppressed sets Suppressed field to given value.

### HasSuppressed

`func (o *Throwable) HasSuppressed() bool`

HasSuppressed returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



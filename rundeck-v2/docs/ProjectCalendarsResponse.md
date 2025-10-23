# ProjectCalendarsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Calendar** | Pointer to [**Calendar**](Calendar.md) |  | [optional] 
**Msg** | Pointer to **string** |  | [optional] 
**Saved** | Pointer to **bool** |  | [optional] 

## Methods

### NewProjectCalendarsResponse

`func NewProjectCalendarsResponse() *ProjectCalendarsResponse`

NewProjectCalendarsResponse instantiates a new ProjectCalendarsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProjectCalendarsResponseWithDefaults

`func NewProjectCalendarsResponseWithDefaults() *ProjectCalendarsResponse`

NewProjectCalendarsResponseWithDefaults instantiates a new ProjectCalendarsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCalendar

`func (o *ProjectCalendarsResponse) GetCalendar() Calendar`

GetCalendar returns the Calendar field if non-nil, zero value otherwise.

### GetCalendarOk

`func (o *ProjectCalendarsResponse) GetCalendarOk() (*Calendar, bool)`

GetCalendarOk returns a tuple with the Calendar field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCalendar

`func (o *ProjectCalendarsResponse) SetCalendar(v Calendar)`

SetCalendar sets Calendar field to given value.

### HasCalendar

`func (o *ProjectCalendarsResponse) HasCalendar() bool`

HasCalendar returns a boolean if a field has been set.

### GetMsg

`func (o *ProjectCalendarsResponse) GetMsg() string`

GetMsg returns the Msg field if non-nil, zero value otherwise.

### GetMsgOk

`func (o *ProjectCalendarsResponse) GetMsgOk() (*string, bool)`

GetMsgOk returns a tuple with the Msg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMsg

`func (o *ProjectCalendarsResponse) SetMsg(v string)`

SetMsg sets Msg field to given value.

### HasMsg

`func (o *ProjectCalendarsResponse) HasMsg() bool`

HasMsg returns a boolean if a field has been set.

### GetSaved

`func (o *ProjectCalendarsResponse) GetSaved() bool`

GetSaved returns the Saved field if non-nil, zero value otherwise.

### GetSavedOk

`func (o *ProjectCalendarsResponse) GetSavedOk() (*bool, bool)`

GetSavedOk returns a tuple with the Saved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSaved

`func (o *ProjectCalendarsResponse) SetSaved(v bool)`

SetSaved sets Saved field to given value.

### HasSaved

`func (o *ProjectCalendarsResponse) HasSaved() bool`

HasSaved returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



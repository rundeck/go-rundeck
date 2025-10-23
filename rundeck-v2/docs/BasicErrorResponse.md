# BasicErrorResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | Pointer to **bool** |  | [optional] 
**Apiversion** | Pointer to **int32** |  | [optional] 
**ErrorCode** | Pointer to **string** |  | [optional] 
**Message** | Pointer to **string** |  | [optional] 

## Methods

### NewBasicErrorResponse

`func NewBasicErrorResponse() *BasicErrorResponse`

NewBasicErrorResponse instantiates a new BasicErrorResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBasicErrorResponseWithDefaults

`func NewBasicErrorResponseWithDefaults() *BasicErrorResponse`

NewBasicErrorResponseWithDefaults instantiates a new BasicErrorResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *BasicErrorResponse) GetError() bool`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *BasicErrorResponse) GetErrorOk() (*bool, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *BasicErrorResponse) SetError(v bool)`

SetError sets Error field to given value.

### HasError

`func (o *BasicErrorResponse) HasError() bool`

HasError returns a boolean if a field has been set.

### GetApiversion

`func (o *BasicErrorResponse) GetApiversion() int32`

GetApiversion returns the Apiversion field if non-nil, zero value otherwise.

### GetApiversionOk

`func (o *BasicErrorResponse) GetApiversionOk() (*int32, bool)`

GetApiversionOk returns a tuple with the Apiversion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiversion

`func (o *BasicErrorResponse) SetApiversion(v int32)`

SetApiversion sets Apiversion field to given value.

### HasApiversion

`func (o *BasicErrorResponse) HasApiversion() bool`

HasApiversion returns a boolean if a field has been set.

### GetErrorCode

`func (o *BasicErrorResponse) GetErrorCode() string`

GetErrorCode returns the ErrorCode field if non-nil, zero value otherwise.

### GetErrorCodeOk

`func (o *BasicErrorResponse) GetErrorCodeOk() (*string, bool)`

GetErrorCodeOk returns a tuple with the ErrorCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCode

`func (o *BasicErrorResponse) SetErrorCode(v string)`

SetErrorCode sets ErrorCode field to given value.

### HasErrorCode

`func (o *BasicErrorResponse) HasErrorCode() bool`

HasErrorCode returns a boolean if a field has been set.

### GetMessage

`func (o *BasicErrorResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *BasicErrorResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *BasicErrorResponse) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *BasicErrorResponse) HasMessage() bool`

HasMessage returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



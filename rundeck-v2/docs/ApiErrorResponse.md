# ApiErrorResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | Pointer to **bool** | Always true to indicate an error response | [optional] 
**Apiversion** | Pointer to **int32** | Rundeck / Runbook Automation API version number | [optional] 
**ErrorCode** | Pointer to **string** | Error code (HTTP status or custom error code) | [optional] 
**Message** | Pointer to **string** | Human-readable error message | [optional] 
**ErrorMessage** | Pointer to **string** |  | [optional] 

## Methods

### NewApiErrorResponse

`func NewApiErrorResponse() *ApiErrorResponse`

NewApiErrorResponse instantiates a new ApiErrorResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiErrorResponseWithDefaults

`func NewApiErrorResponseWithDefaults() *ApiErrorResponse`

NewApiErrorResponseWithDefaults instantiates a new ApiErrorResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *ApiErrorResponse) GetError() bool`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *ApiErrorResponse) GetErrorOk() (*bool, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *ApiErrorResponse) SetError(v bool)`

SetError sets Error field to given value.

### HasError

`func (o *ApiErrorResponse) HasError() bool`

HasError returns a boolean if a field has been set.

### GetApiversion

`func (o *ApiErrorResponse) GetApiversion() int32`

GetApiversion returns the Apiversion field if non-nil, zero value otherwise.

### GetApiversionOk

`func (o *ApiErrorResponse) GetApiversionOk() (*int32, bool)`

GetApiversionOk returns a tuple with the Apiversion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiversion

`func (o *ApiErrorResponse) SetApiversion(v int32)`

SetApiversion sets Apiversion field to given value.

### HasApiversion

`func (o *ApiErrorResponse) HasApiversion() bool`

HasApiversion returns a boolean if a field has been set.

### GetErrorCode

`func (o *ApiErrorResponse) GetErrorCode() string`

GetErrorCode returns the ErrorCode field if non-nil, zero value otherwise.

### GetErrorCodeOk

`func (o *ApiErrorResponse) GetErrorCodeOk() (*string, bool)`

GetErrorCodeOk returns a tuple with the ErrorCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCode

`func (o *ApiErrorResponse) SetErrorCode(v string)`

SetErrorCode sets ErrorCode field to given value.

### HasErrorCode

`func (o *ApiErrorResponse) HasErrorCode() bool`

HasErrorCode returns a boolean if a field has been set.

### GetMessage

`func (o *ApiErrorResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ApiErrorResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ApiErrorResponse) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *ApiErrorResponse) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetErrorMessage

`func (o *ApiErrorResponse) GetErrorMessage() string`

GetErrorMessage returns the ErrorMessage field if non-nil, zero value otherwise.

### GetErrorMessageOk

`func (o *ApiErrorResponse) GetErrorMessageOk() (*string, bool)`

GetErrorMessageOk returns a tuple with the ErrorMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorMessage

`func (o *ApiErrorResponse) SetErrorMessage(v string)`

SetErrorMessage sets ErrorMessage field to given value.

### HasErrorMessage

`func (o *ApiErrorResponse) HasErrorMessage() bool`

HasErrorMessage returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



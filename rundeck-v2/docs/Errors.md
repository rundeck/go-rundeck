# Errors

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ObjectName** | Pointer to **string** |  | [optional] 
**NestedPath** | Pointer to **string** |  | [optional] 
**ErrorCount** | Pointer to **int32** |  | [optional] 
**AllErrors** | Pointer to [**[]ObjectError**](ObjectError.md) |  | [optional] 
**GlobalErrorCount** | Pointer to **int32** |  | [optional] 
**GlobalErrors** | Pointer to [**[]ObjectError**](ObjectError.md) |  | [optional] 
**GlobalError** | Pointer to [**ObjectError**](ObjectError.md) |  | [optional] 
**FieldErrorCount** | Pointer to **int32** |  | [optional] 
**FieldErrors** | Pointer to [**[]FieldError**](FieldError.md) |  | [optional] 
**FieldError** | Pointer to [**FieldError**](FieldError.md) |  | [optional] 

## Methods

### NewErrors

`func NewErrors() *Errors`

NewErrors instantiates a new Errors object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewErrorsWithDefaults

`func NewErrorsWithDefaults() *Errors`

NewErrorsWithDefaults instantiates a new Errors object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObjectName

`func (o *Errors) GetObjectName() string`

GetObjectName returns the ObjectName field if non-nil, zero value otherwise.

### GetObjectNameOk

`func (o *Errors) GetObjectNameOk() (*string, bool)`

GetObjectNameOk returns a tuple with the ObjectName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObjectName

`func (o *Errors) SetObjectName(v string)`

SetObjectName sets ObjectName field to given value.

### HasObjectName

`func (o *Errors) HasObjectName() bool`

HasObjectName returns a boolean if a field has been set.

### GetNestedPath

`func (o *Errors) GetNestedPath() string`

GetNestedPath returns the NestedPath field if non-nil, zero value otherwise.

### GetNestedPathOk

`func (o *Errors) GetNestedPathOk() (*string, bool)`

GetNestedPathOk returns a tuple with the NestedPath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNestedPath

`func (o *Errors) SetNestedPath(v string)`

SetNestedPath sets NestedPath field to given value.

### HasNestedPath

`func (o *Errors) HasNestedPath() bool`

HasNestedPath returns a boolean if a field has been set.

### GetErrorCount

`func (o *Errors) GetErrorCount() int32`

GetErrorCount returns the ErrorCount field if non-nil, zero value otherwise.

### GetErrorCountOk

`func (o *Errors) GetErrorCountOk() (*int32, bool)`

GetErrorCountOk returns a tuple with the ErrorCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCount

`func (o *Errors) SetErrorCount(v int32)`

SetErrorCount sets ErrorCount field to given value.

### HasErrorCount

`func (o *Errors) HasErrorCount() bool`

HasErrorCount returns a boolean if a field has been set.

### GetAllErrors

`func (o *Errors) GetAllErrors() []ObjectError`

GetAllErrors returns the AllErrors field if non-nil, zero value otherwise.

### GetAllErrorsOk

`func (o *Errors) GetAllErrorsOk() (*[]ObjectError, bool)`

GetAllErrorsOk returns a tuple with the AllErrors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllErrors

`func (o *Errors) SetAllErrors(v []ObjectError)`

SetAllErrors sets AllErrors field to given value.

### HasAllErrors

`func (o *Errors) HasAllErrors() bool`

HasAllErrors returns a boolean if a field has been set.

### GetGlobalErrorCount

`func (o *Errors) GetGlobalErrorCount() int32`

GetGlobalErrorCount returns the GlobalErrorCount field if non-nil, zero value otherwise.

### GetGlobalErrorCountOk

`func (o *Errors) GetGlobalErrorCountOk() (*int32, bool)`

GetGlobalErrorCountOk returns a tuple with the GlobalErrorCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGlobalErrorCount

`func (o *Errors) SetGlobalErrorCount(v int32)`

SetGlobalErrorCount sets GlobalErrorCount field to given value.

### HasGlobalErrorCount

`func (o *Errors) HasGlobalErrorCount() bool`

HasGlobalErrorCount returns a boolean if a field has been set.

### GetGlobalErrors

`func (o *Errors) GetGlobalErrors() []ObjectError`

GetGlobalErrors returns the GlobalErrors field if non-nil, zero value otherwise.

### GetGlobalErrorsOk

`func (o *Errors) GetGlobalErrorsOk() (*[]ObjectError, bool)`

GetGlobalErrorsOk returns a tuple with the GlobalErrors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGlobalErrors

`func (o *Errors) SetGlobalErrors(v []ObjectError)`

SetGlobalErrors sets GlobalErrors field to given value.

### HasGlobalErrors

`func (o *Errors) HasGlobalErrors() bool`

HasGlobalErrors returns a boolean if a field has been set.

### GetGlobalError

`func (o *Errors) GetGlobalError() ObjectError`

GetGlobalError returns the GlobalError field if non-nil, zero value otherwise.

### GetGlobalErrorOk

`func (o *Errors) GetGlobalErrorOk() (*ObjectError, bool)`

GetGlobalErrorOk returns a tuple with the GlobalError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGlobalError

`func (o *Errors) SetGlobalError(v ObjectError)`

SetGlobalError sets GlobalError field to given value.

### HasGlobalError

`func (o *Errors) HasGlobalError() bool`

HasGlobalError returns a boolean if a field has been set.

### GetFieldErrorCount

`func (o *Errors) GetFieldErrorCount() int32`

GetFieldErrorCount returns the FieldErrorCount field if non-nil, zero value otherwise.

### GetFieldErrorCountOk

`func (o *Errors) GetFieldErrorCountOk() (*int32, bool)`

GetFieldErrorCountOk returns a tuple with the FieldErrorCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFieldErrorCount

`func (o *Errors) SetFieldErrorCount(v int32)`

SetFieldErrorCount sets FieldErrorCount field to given value.

### HasFieldErrorCount

`func (o *Errors) HasFieldErrorCount() bool`

HasFieldErrorCount returns a boolean if a field has been set.

### GetFieldErrors

`func (o *Errors) GetFieldErrors() []FieldError`

GetFieldErrors returns the FieldErrors field if non-nil, zero value otherwise.

### GetFieldErrorsOk

`func (o *Errors) GetFieldErrorsOk() (*[]FieldError, bool)`

GetFieldErrorsOk returns a tuple with the FieldErrors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFieldErrors

`func (o *Errors) SetFieldErrors(v []FieldError)`

SetFieldErrors sets FieldErrors field to given value.

### HasFieldErrors

`func (o *Errors) HasFieldErrors() bool`

HasFieldErrors returns a boolean if a field has been set.

### GetFieldError

`func (o *Errors) GetFieldError() FieldError`

GetFieldError returns the FieldError field if non-nil, zero value otherwise.

### GetFieldErrorOk

`func (o *Errors) GetFieldErrorOk() (*FieldError, bool)`

GetFieldErrorOk returns a tuple with the FieldError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFieldError

`func (o *Errors) SetFieldError(v FieldError)`

SetFieldError sets FieldError field to given value.

### HasFieldError

`func (o *Errors) HasFieldError() bool`

HasFieldError returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



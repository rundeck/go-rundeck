# FieldError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **string** |  | 
**Codes** | Pointer to **[]string** |  | [optional] 
**Arguments** | Pointer to **[]map[string]interface{}** |  | [optional] 
**DefaultMessage** | Pointer to **string** |  | [optional] 
**ObjectName** | **string** |  | 
**Field** | **string** |  | 
**RejectedValue** | Pointer to **map[string]interface{}** |  | [optional] 
**BindingFailure** | Pointer to **bool** |  | [optional] 

## Methods

### NewFieldError

`func NewFieldError(code string, objectName string, field string, ) *FieldError`

NewFieldError instantiates a new FieldError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFieldErrorWithDefaults

`func NewFieldErrorWithDefaults() *FieldError`

NewFieldErrorWithDefaults instantiates a new FieldError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *FieldError) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *FieldError) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *FieldError) SetCode(v string)`

SetCode sets Code field to given value.


### GetCodes

`func (o *FieldError) GetCodes() []string`

GetCodes returns the Codes field if non-nil, zero value otherwise.

### GetCodesOk

`func (o *FieldError) GetCodesOk() (*[]string, bool)`

GetCodesOk returns a tuple with the Codes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCodes

`func (o *FieldError) SetCodes(v []string)`

SetCodes sets Codes field to given value.

### HasCodes

`func (o *FieldError) HasCodes() bool`

HasCodes returns a boolean if a field has been set.

### GetArguments

`func (o *FieldError) GetArguments() []map[string]interface{}`

GetArguments returns the Arguments field if non-nil, zero value otherwise.

### GetArgumentsOk

`func (o *FieldError) GetArgumentsOk() (*[]map[string]interface{}, bool)`

GetArgumentsOk returns a tuple with the Arguments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArguments

`func (o *FieldError) SetArguments(v []map[string]interface{})`

SetArguments sets Arguments field to given value.

### HasArguments

`func (o *FieldError) HasArguments() bool`

HasArguments returns a boolean if a field has been set.

### GetDefaultMessage

`func (o *FieldError) GetDefaultMessage() string`

GetDefaultMessage returns the DefaultMessage field if non-nil, zero value otherwise.

### GetDefaultMessageOk

`func (o *FieldError) GetDefaultMessageOk() (*string, bool)`

GetDefaultMessageOk returns a tuple with the DefaultMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultMessage

`func (o *FieldError) SetDefaultMessage(v string)`

SetDefaultMessage sets DefaultMessage field to given value.

### HasDefaultMessage

`func (o *FieldError) HasDefaultMessage() bool`

HasDefaultMessage returns a boolean if a field has been set.

### GetObjectName

`func (o *FieldError) GetObjectName() string`

GetObjectName returns the ObjectName field if non-nil, zero value otherwise.

### GetObjectNameOk

`func (o *FieldError) GetObjectNameOk() (*string, bool)`

GetObjectNameOk returns a tuple with the ObjectName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObjectName

`func (o *FieldError) SetObjectName(v string)`

SetObjectName sets ObjectName field to given value.


### GetField

`func (o *FieldError) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *FieldError) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *FieldError) SetField(v string)`

SetField sets Field field to given value.


### GetRejectedValue

`func (o *FieldError) GetRejectedValue() map[string]interface{}`

GetRejectedValue returns the RejectedValue field if non-nil, zero value otherwise.

### GetRejectedValueOk

`func (o *FieldError) GetRejectedValueOk() (*map[string]interface{}, bool)`

GetRejectedValueOk returns a tuple with the RejectedValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRejectedValue

`func (o *FieldError) SetRejectedValue(v map[string]interface{})`

SetRejectedValue sets RejectedValue field to given value.

### HasRejectedValue

`func (o *FieldError) HasRejectedValue() bool`

HasRejectedValue returns a boolean if a field has been set.

### GetBindingFailure

`func (o *FieldError) GetBindingFailure() bool`

GetBindingFailure returns the BindingFailure field if non-nil, zero value otherwise.

### GetBindingFailureOk

`func (o *FieldError) GetBindingFailureOk() (*bool, bool)`

GetBindingFailureOk returns a tuple with the BindingFailure field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBindingFailure

`func (o *FieldError) SetBindingFailure(v bool)`

SetBindingFailure sets BindingFailure field to given value.

### HasBindingFailure

`func (o *FieldError) HasBindingFailure() bool`

HasBindingFailure returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



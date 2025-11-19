# FieldError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BindingFailure** | Pointer to **bool** |  | [optional] 
**RejectedValue** | Pointer to **map[string]interface{}** |  | [optional] 
**Field** | **string** |  | 

## Methods

### NewFieldError

`func NewFieldError(field string, ) *FieldError`

NewFieldError instantiates a new FieldError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFieldErrorWithDefaults

`func NewFieldErrorWithDefaults() *FieldError`

NewFieldErrorWithDefaults instantiates a new FieldError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

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



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



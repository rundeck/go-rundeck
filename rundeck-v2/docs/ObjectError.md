# ObjectError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | Pointer to **string** |  | [optional] 
**Codes** | Pointer to **[]string** |  | [optional] 
**DefaultMessage** | Pointer to **string** |  | [optional] 
**Arguments** | Pointer to **[]map[string]interface{}** |  | [optional] 
**ObjectName** | **string** |  | 

## Methods

### NewObjectError

`func NewObjectError(objectName string, ) *ObjectError`

NewObjectError instantiates a new ObjectError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewObjectErrorWithDefaults

`func NewObjectErrorWithDefaults() *ObjectError`

NewObjectErrorWithDefaults instantiates a new ObjectError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *ObjectError) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *ObjectError) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *ObjectError) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *ObjectError) HasCode() bool`

HasCode returns a boolean if a field has been set.

### GetCodes

`func (o *ObjectError) GetCodes() []string`

GetCodes returns the Codes field if non-nil, zero value otherwise.

### GetCodesOk

`func (o *ObjectError) GetCodesOk() (*[]string, bool)`

GetCodesOk returns a tuple with the Codes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCodes

`func (o *ObjectError) SetCodes(v []string)`

SetCodes sets Codes field to given value.

### HasCodes

`func (o *ObjectError) HasCodes() bool`

HasCodes returns a boolean if a field has been set.

### GetDefaultMessage

`func (o *ObjectError) GetDefaultMessage() string`

GetDefaultMessage returns the DefaultMessage field if non-nil, zero value otherwise.

### GetDefaultMessageOk

`func (o *ObjectError) GetDefaultMessageOk() (*string, bool)`

GetDefaultMessageOk returns a tuple with the DefaultMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultMessage

`func (o *ObjectError) SetDefaultMessage(v string)`

SetDefaultMessage sets DefaultMessage field to given value.

### HasDefaultMessage

`func (o *ObjectError) HasDefaultMessage() bool`

HasDefaultMessage returns a boolean if a field has been set.

### GetArguments

`func (o *ObjectError) GetArguments() []map[string]interface{}`

GetArguments returns the Arguments field if non-nil, zero value otherwise.

### GetArgumentsOk

`func (o *ObjectError) GetArgumentsOk() (*[]map[string]interface{}, bool)`

GetArgumentsOk returns a tuple with the Arguments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArguments

`func (o *ObjectError) SetArguments(v []map[string]interface{})`

SetArguments sets Arguments field to given value.

### HasArguments

`func (o *ObjectError) HasArguments() bool`

HasArguments returns a boolean if a field has been set.

### GetObjectName

`func (o *ObjectError) GetObjectName() string`

GetObjectName returns the ObjectName field if non-nil, zero value otherwise.

### GetObjectNameOk

`func (o *ObjectError) GetObjectNameOk() (*string, bool)`

GetObjectNameOk returns a tuple with the ObjectName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObjectName

`func (o *ObjectError) SetObjectName(v string)`

SetObjectName sets ObjectName field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# StackTraceElement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileName** | Pointer to **string** |  | [optional] 
**LineNumber** | Pointer to **int32** |  | [optional] 
**ModuleName** | Pointer to **string** |  | [optional] 
**ModuleVersion** | Pointer to **string** |  | [optional] 
**ClassLoaderName** | Pointer to **string** |  | [optional] 
**ClassName** | Pointer to **string** |  | [optional] 
**MethodName** | Pointer to **string** |  | [optional] 
**NativeMethod** | Pointer to **bool** |  | [optional] 

## Methods

### NewStackTraceElement

`func NewStackTraceElement() *StackTraceElement`

NewStackTraceElement instantiates a new StackTraceElement object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStackTraceElementWithDefaults

`func NewStackTraceElementWithDefaults() *StackTraceElement`

NewStackTraceElementWithDefaults instantiates a new StackTraceElement object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileName

`func (o *StackTraceElement) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *StackTraceElement) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *StackTraceElement) SetFileName(v string)`

SetFileName sets FileName field to given value.

### HasFileName

`func (o *StackTraceElement) HasFileName() bool`

HasFileName returns a boolean if a field has been set.

### GetLineNumber

`func (o *StackTraceElement) GetLineNumber() int32`

GetLineNumber returns the LineNumber field if non-nil, zero value otherwise.

### GetLineNumberOk

`func (o *StackTraceElement) GetLineNumberOk() (*int32, bool)`

GetLineNumberOk returns a tuple with the LineNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLineNumber

`func (o *StackTraceElement) SetLineNumber(v int32)`

SetLineNumber sets LineNumber field to given value.

### HasLineNumber

`func (o *StackTraceElement) HasLineNumber() bool`

HasLineNumber returns a boolean if a field has been set.

### GetModuleName

`func (o *StackTraceElement) GetModuleName() string`

GetModuleName returns the ModuleName field if non-nil, zero value otherwise.

### GetModuleNameOk

`func (o *StackTraceElement) GetModuleNameOk() (*string, bool)`

GetModuleNameOk returns a tuple with the ModuleName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModuleName

`func (o *StackTraceElement) SetModuleName(v string)`

SetModuleName sets ModuleName field to given value.

### HasModuleName

`func (o *StackTraceElement) HasModuleName() bool`

HasModuleName returns a boolean if a field has been set.

### GetModuleVersion

`func (o *StackTraceElement) GetModuleVersion() string`

GetModuleVersion returns the ModuleVersion field if non-nil, zero value otherwise.

### GetModuleVersionOk

`func (o *StackTraceElement) GetModuleVersionOk() (*string, bool)`

GetModuleVersionOk returns a tuple with the ModuleVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModuleVersion

`func (o *StackTraceElement) SetModuleVersion(v string)`

SetModuleVersion sets ModuleVersion field to given value.

### HasModuleVersion

`func (o *StackTraceElement) HasModuleVersion() bool`

HasModuleVersion returns a boolean if a field has been set.

### GetClassLoaderName

`func (o *StackTraceElement) GetClassLoaderName() string`

GetClassLoaderName returns the ClassLoaderName field if non-nil, zero value otherwise.

### GetClassLoaderNameOk

`func (o *StackTraceElement) GetClassLoaderNameOk() (*string, bool)`

GetClassLoaderNameOk returns a tuple with the ClassLoaderName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClassLoaderName

`func (o *StackTraceElement) SetClassLoaderName(v string)`

SetClassLoaderName sets ClassLoaderName field to given value.

### HasClassLoaderName

`func (o *StackTraceElement) HasClassLoaderName() bool`

HasClassLoaderName returns a boolean if a field has been set.

### GetClassName

`func (o *StackTraceElement) GetClassName() string`

GetClassName returns the ClassName field if non-nil, zero value otherwise.

### GetClassNameOk

`func (o *StackTraceElement) GetClassNameOk() (*string, bool)`

GetClassNameOk returns a tuple with the ClassName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClassName

`func (o *StackTraceElement) SetClassName(v string)`

SetClassName sets ClassName field to given value.

### HasClassName

`func (o *StackTraceElement) HasClassName() bool`

HasClassName returns a boolean if a field has been set.

### GetMethodName

`func (o *StackTraceElement) GetMethodName() string`

GetMethodName returns the MethodName field if non-nil, zero value otherwise.

### GetMethodNameOk

`func (o *StackTraceElement) GetMethodNameOk() (*string, bool)`

GetMethodNameOk returns a tuple with the MethodName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMethodName

`func (o *StackTraceElement) SetMethodName(v string)`

SetMethodName sets MethodName field to given value.

### HasMethodName

`func (o *StackTraceElement) HasMethodName() bool`

HasMethodName returns a boolean if a field has been set.

### GetNativeMethod

`func (o *StackTraceElement) GetNativeMethod() bool`

GetNativeMethod returns the NativeMethod field if non-nil, zero value otherwise.

### GetNativeMethodOk

`func (o *StackTraceElement) GetNativeMethodOk() (*bool, bool)`

GetNativeMethodOk returns a tuple with the NativeMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNativeMethod

`func (o *StackTraceElement) SetNativeMethod(v bool)`

SetNativeMethod sets NativeMethod field to given value.

### HasNativeMethod

`func (o *StackTraceElement) HasNativeMethod() bool`

HasNativeMethod returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



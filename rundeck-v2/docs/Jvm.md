# Jvm

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Vendor** | Pointer to **string** |  | [optional] 
**Version** | Pointer to **string** |  | [optional] 
**ImplementationVersion** | Pointer to **string** |  | [optional] 

## Methods

### NewJvm

`func NewJvm() *Jvm`

NewJvm instantiates a new Jvm object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJvmWithDefaults

`func NewJvmWithDefaults() *Jvm`

NewJvmWithDefaults instantiates a new Jvm object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Jvm) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Jvm) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Jvm) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Jvm) HasName() bool`

HasName returns a boolean if a field has been set.

### GetVendor

`func (o *Jvm) GetVendor() string`

GetVendor returns the Vendor field if non-nil, zero value otherwise.

### GetVendorOk

`func (o *Jvm) GetVendorOk() (*string, bool)`

GetVendorOk returns a tuple with the Vendor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVendor

`func (o *Jvm) SetVendor(v string)`

SetVendor sets Vendor field to given value.

### HasVendor

`func (o *Jvm) HasVendor() bool`

HasVendor returns a boolean if a field has been set.

### GetVersion

`func (o *Jvm) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *Jvm) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *Jvm) SetVersion(v string)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *Jvm) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### GetImplementationVersion

`func (o *Jvm) GetImplementationVersion() string`

GetImplementationVersion returns the ImplementationVersion field if non-nil, zero value otherwise.

### GetImplementationVersionOk

`func (o *Jvm) GetImplementationVersionOk() (*string, bool)`

GetImplementationVersionOk returns a tuple with the ImplementationVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImplementationVersion

`func (o *Jvm) SetImplementationVersion(v string)`

SetImplementationVersion sets ImplementationVersion field to given value.

### HasImplementationVersion

`func (o *Jvm) HasImplementationVersion() bool`

HasImplementationVersion returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# LicenseEntitlement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to [**LicenseEntitlementDescription**](LicenseEntitlementDescription.md) |  | [optional] 
**Value** | Pointer to **map[string]string** |  | [optional] 

## Methods

### NewLicenseEntitlement

`func NewLicenseEntitlement() *LicenseEntitlement`

NewLicenseEntitlement instantiates a new LicenseEntitlement object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseEntitlementWithDefaults

`func NewLicenseEntitlementWithDefaults() *LicenseEntitlement`

NewLicenseEntitlementWithDefaults instantiates a new LicenseEntitlement object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *LicenseEntitlement) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *LicenseEntitlement) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *LicenseEntitlement) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *LicenseEntitlement) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *LicenseEntitlement) GetDescription() LicenseEntitlementDescription`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *LicenseEntitlement) GetDescriptionOk() (*LicenseEntitlementDescription, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *LicenseEntitlement) SetDescription(v LicenseEntitlementDescription)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *LicenseEntitlement) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetValue

`func (o *LicenseEntitlement) GetValue() map[string]string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *LicenseEntitlement) GetValueOk() (*map[string]string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *LicenseEntitlement) SetValue(v map[string]string)`

SetValue sets Value field to given value.

### HasValue

`func (o *LicenseEntitlement) HasValue() bool`

HasValue returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



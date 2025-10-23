# Manifest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Enabled** | Pointer to **bool** |  | [optional] 
**Tours** | Pointer to [**[]Tour**](Tour.md) |  | [optional] 

## Methods

### NewManifest

`func NewManifest() *Manifest`

NewManifest instantiates a new Manifest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewManifestWithDefaults

`func NewManifestWithDefaults() *Manifest`

NewManifestWithDefaults instantiates a new Manifest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Manifest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Manifest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Manifest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Manifest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetEnabled

`func (o *Manifest) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *Manifest) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *Manifest) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *Manifest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetTours

`func (o *Manifest) GetTours() []Tour`

GetTours returns the Tours field if non-nil, zero value otherwise.

### GetToursOk

`func (o *Manifest) GetToursOk() (*[]Tour, bool)`

GetToursOk returns a tuple with the Tours field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTours

`func (o *Manifest) SetTours(v []Tour)`

SetTours sets Tours field to given value.

### HasTours

`func (o *Manifest) HasTours() bool`

HasTours returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



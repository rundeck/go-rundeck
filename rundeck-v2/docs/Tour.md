# Tour

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Key** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Enabled** | Pointer to **bool** |  | [optional] 
**Steps** | Pointer to [**[]Step**](Step.md) |  | [optional] 

## Methods

### NewTour

`func NewTour() *Tour`

NewTour instantiates a new Tour object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTourWithDefaults

`func NewTourWithDefaults() *Tour`

NewTourWithDefaults instantiates a new Tour object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Tour) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Tour) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Tour) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Tour) HasName() bool`

HasName returns a boolean if a field has been set.

### GetKey

`func (o *Tour) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *Tour) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *Tour) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *Tour) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetDescription

`func (o *Tour) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Tour) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Tour) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Tour) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetEnabled

`func (o *Tour) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *Tour) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *Tour) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *Tour) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetSteps

`func (o *Tour) GetSteps() []Step`

GetSteps returns the Steps field if non-nil, zero value otherwise.

### GetStepsOk

`func (o *Tour) GetStepsOk() (*[]Step, bool)`

GetStepsOk returns a tuple with the Steps field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSteps

`func (o *Tour) SetSteps(v []Step)`

SetSteps sets Steps field to given value.

### HasSteps

`func (o *Tour) HasSteps() bool`

HasSteps returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



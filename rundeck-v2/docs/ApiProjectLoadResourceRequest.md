# ApiProjectLoadResourceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Enabled** | Pointer to **bool** |  | [optional] 
**Tours** | Pointer to [**[]Tour**](Tour.md) |  | [optional] 
**Key** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Steps** | Pointer to [**[]Step**](Step.md) |  | [optional] 

## Methods

### NewApiProjectLoadResourceRequest

`func NewApiProjectLoadResourceRequest() *ApiProjectLoadResourceRequest`

NewApiProjectLoadResourceRequest instantiates a new ApiProjectLoadResourceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiProjectLoadResourceRequestWithDefaults

`func NewApiProjectLoadResourceRequestWithDefaults() *ApiProjectLoadResourceRequest`

NewApiProjectLoadResourceRequestWithDefaults instantiates a new ApiProjectLoadResourceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *ApiProjectLoadResourceRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApiProjectLoadResourceRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApiProjectLoadResourceRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ApiProjectLoadResourceRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetEnabled

`func (o *ApiProjectLoadResourceRequest) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *ApiProjectLoadResourceRequest) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *ApiProjectLoadResourceRequest) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *ApiProjectLoadResourceRequest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetTours

`func (o *ApiProjectLoadResourceRequest) GetTours() []Tour`

GetTours returns the Tours field if non-nil, zero value otherwise.

### GetToursOk

`func (o *ApiProjectLoadResourceRequest) GetToursOk() (*[]Tour, bool)`

GetToursOk returns a tuple with the Tours field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTours

`func (o *ApiProjectLoadResourceRequest) SetTours(v []Tour)`

SetTours sets Tours field to given value.

### HasTours

`func (o *ApiProjectLoadResourceRequest) HasTours() bool`

HasTours returns a boolean if a field has been set.

### GetKey

`func (o *ApiProjectLoadResourceRequest) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *ApiProjectLoadResourceRequest) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *ApiProjectLoadResourceRequest) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *ApiProjectLoadResourceRequest) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetDescription

`func (o *ApiProjectLoadResourceRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ApiProjectLoadResourceRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ApiProjectLoadResourceRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ApiProjectLoadResourceRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetSteps

`func (o *ApiProjectLoadResourceRequest) GetSteps() []Step`

GetSteps returns the Steps field if non-nil, zero value otherwise.

### GetStepsOk

`func (o *ApiProjectLoadResourceRequest) GetStepsOk() (*[]Step, bool)`

GetStepsOk returns a tuple with the Steps field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSteps

`func (o *ApiProjectLoadResourceRequest) SetSteps(v []Step)`

SetSteps sets Steps field to given value.

### HasSteps

`func (o *ApiProjectLoadResourceRequest) HasSteps() bool`

HasSteps returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



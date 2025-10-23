# OptionValidateResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Valid** | Pointer to **bool** |  | [optional] 
**Messages** | Pointer to **map[string][]string** | Mapping of input key to list of validation error messages | [optional] 

## Methods

### NewOptionValidateResponse

`func NewOptionValidateResponse() *OptionValidateResponse`

NewOptionValidateResponse instantiates a new OptionValidateResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOptionValidateResponseWithDefaults

`func NewOptionValidateResponseWithDefaults() *OptionValidateResponse`

NewOptionValidateResponseWithDefaults instantiates a new OptionValidateResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValid

`func (o *OptionValidateResponse) GetValid() bool`

GetValid returns the Valid field if non-nil, zero value otherwise.

### GetValidOk

`func (o *OptionValidateResponse) GetValidOk() (*bool, bool)`

GetValidOk returns a tuple with the Valid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValid

`func (o *OptionValidateResponse) SetValid(v bool)`

SetValid sets Valid field to given value.

### HasValid

`func (o *OptionValidateResponse) HasValid() bool`

HasValid returns a boolean if a field has been set.

### GetMessages

`func (o *OptionValidateResponse) GetMessages() map[string][]string`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *OptionValidateResponse) GetMessagesOk() (*map[string][]string, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *OptionValidateResponse) SetMessages(v map[string][]string)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *OptionValidateResponse) HasMessages() bool`

HasMessages returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



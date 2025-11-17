# ApiValidateOptionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** |  | [optional] 
**StoragePath** | Pointer to **string** |  | [optional] 
**ValuesUrl** | Pointer to **string** |  | [optional] 
**Value** | Pointer to **string** |  | [optional] 
**Values** | Pointer to **[]string** |  | [optional] 
**Secure** | Pointer to **bool** |  | [optional] 
**ValueExposed** | Pointer to **bool** |  | [optional] 
**ValuesType** | Pointer to **string** |  | [optional] 
**RemoteUrlAuthenticationType** | Pointer to **string** |  | [optional] 
**ConfigRemoteUrl** | Pointer to **map[string]interface{}** |  | [optional] 
**OptionType** | Pointer to **string** |  | [optional] 
**DefaultStoragePath** | Pointer to **string** |  | [optional] 
**RealValuesUrl** | Pointer to **string** |  | [optional] 
**DefaultValue** | Pointer to **string** |  | [optional] 
**ValuesList** | Pointer to **string** |  | [optional] 
**OptionValues** | Pointer to **[]string** |  | [optional] 
**SecureInput** | Pointer to **bool** |  | [optional] 
**SecureExposed** | Pointer to **bool** |  | [optional] 
**OptionData** | Pointer to [**OptionValidateRequest**](OptionValidateRequest.md) |  | [optional] 

## Methods

### NewApiValidateOptionRequest

`func NewApiValidateOptionRequest() *ApiValidateOptionRequest`

NewApiValidateOptionRequest instantiates a new ApiValidateOptionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiValidateOptionRequestWithDefaults

`func NewApiValidateOptionRequestWithDefaults() *ApiValidateOptionRequest`

NewApiValidateOptionRequestWithDefaults instantiates a new ApiValidateOptionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *ApiValidateOptionRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ApiValidateOptionRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ApiValidateOptionRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ApiValidateOptionRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetStoragePath

`func (o *ApiValidateOptionRequest) GetStoragePath() string`

GetStoragePath returns the StoragePath field if non-nil, zero value otherwise.

### GetStoragePathOk

`func (o *ApiValidateOptionRequest) GetStoragePathOk() (*string, bool)`

GetStoragePathOk returns a tuple with the StoragePath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStoragePath

`func (o *ApiValidateOptionRequest) SetStoragePath(v string)`

SetStoragePath sets StoragePath field to given value.

### HasStoragePath

`func (o *ApiValidateOptionRequest) HasStoragePath() bool`

HasStoragePath returns a boolean if a field has been set.

### GetValuesUrl

`func (o *ApiValidateOptionRequest) GetValuesUrl() string`

GetValuesUrl returns the ValuesUrl field if non-nil, zero value otherwise.

### GetValuesUrlOk

`func (o *ApiValidateOptionRequest) GetValuesUrlOk() (*string, bool)`

GetValuesUrlOk returns a tuple with the ValuesUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesUrl

`func (o *ApiValidateOptionRequest) SetValuesUrl(v string)`

SetValuesUrl sets ValuesUrl field to given value.

### HasValuesUrl

`func (o *ApiValidateOptionRequest) HasValuesUrl() bool`

HasValuesUrl returns a boolean if a field has been set.

### GetValue

`func (o *ApiValidateOptionRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ApiValidateOptionRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ApiValidateOptionRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *ApiValidateOptionRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetValues

`func (o *ApiValidateOptionRequest) GetValues() []string`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *ApiValidateOptionRequest) GetValuesOk() (*[]string, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *ApiValidateOptionRequest) SetValues(v []string)`

SetValues sets Values field to given value.

### HasValues

`func (o *ApiValidateOptionRequest) HasValues() bool`

HasValues returns a boolean if a field has been set.

### GetSecure

`func (o *ApiValidateOptionRequest) GetSecure() bool`

GetSecure returns the Secure field if non-nil, zero value otherwise.

### GetSecureOk

`func (o *ApiValidateOptionRequest) GetSecureOk() (*bool, bool)`

GetSecureOk returns a tuple with the Secure field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecure

`func (o *ApiValidateOptionRequest) SetSecure(v bool)`

SetSecure sets Secure field to given value.

### HasSecure

`func (o *ApiValidateOptionRequest) HasSecure() bool`

HasSecure returns a boolean if a field has been set.

### GetValueExposed

`func (o *ApiValidateOptionRequest) GetValueExposed() bool`

GetValueExposed returns the ValueExposed field if non-nil, zero value otherwise.

### GetValueExposedOk

`func (o *ApiValidateOptionRequest) GetValueExposedOk() (*bool, bool)`

GetValueExposedOk returns a tuple with the ValueExposed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValueExposed

`func (o *ApiValidateOptionRequest) SetValueExposed(v bool)`

SetValueExposed sets ValueExposed field to given value.

### HasValueExposed

`func (o *ApiValidateOptionRequest) HasValueExposed() bool`

HasValueExposed returns a boolean if a field has been set.

### GetValuesType

`func (o *ApiValidateOptionRequest) GetValuesType() string`

GetValuesType returns the ValuesType field if non-nil, zero value otherwise.

### GetValuesTypeOk

`func (o *ApiValidateOptionRequest) GetValuesTypeOk() (*string, bool)`

GetValuesTypeOk returns a tuple with the ValuesType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesType

`func (o *ApiValidateOptionRequest) SetValuesType(v string)`

SetValuesType sets ValuesType field to given value.

### HasValuesType

`func (o *ApiValidateOptionRequest) HasValuesType() bool`

HasValuesType returns a boolean if a field has been set.

### GetRemoteUrlAuthenticationType

`func (o *ApiValidateOptionRequest) GetRemoteUrlAuthenticationType() string`

GetRemoteUrlAuthenticationType returns the RemoteUrlAuthenticationType field if non-nil, zero value otherwise.

### GetRemoteUrlAuthenticationTypeOk

`func (o *ApiValidateOptionRequest) GetRemoteUrlAuthenticationTypeOk() (*string, bool)`

GetRemoteUrlAuthenticationTypeOk returns a tuple with the RemoteUrlAuthenticationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoteUrlAuthenticationType

`func (o *ApiValidateOptionRequest) SetRemoteUrlAuthenticationType(v string)`

SetRemoteUrlAuthenticationType sets RemoteUrlAuthenticationType field to given value.

### HasRemoteUrlAuthenticationType

`func (o *ApiValidateOptionRequest) HasRemoteUrlAuthenticationType() bool`

HasRemoteUrlAuthenticationType returns a boolean if a field has been set.

### GetConfigRemoteUrl

`func (o *ApiValidateOptionRequest) GetConfigRemoteUrl() map[string]interface{}`

GetConfigRemoteUrl returns the ConfigRemoteUrl field if non-nil, zero value otherwise.

### GetConfigRemoteUrlOk

`func (o *ApiValidateOptionRequest) GetConfigRemoteUrlOk() (*map[string]interface{}, bool)`

GetConfigRemoteUrlOk returns a tuple with the ConfigRemoteUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigRemoteUrl

`func (o *ApiValidateOptionRequest) SetConfigRemoteUrl(v map[string]interface{})`

SetConfigRemoteUrl sets ConfigRemoteUrl field to given value.

### HasConfigRemoteUrl

`func (o *ApiValidateOptionRequest) HasConfigRemoteUrl() bool`

HasConfigRemoteUrl returns a boolean if a field has been set.

### GetOptionType

`func (o *ApiValidateOptionRequest) GetOptionType() string`

GetOptionType returns the OptionType field if non-nil, zero value otherwise.

### GetOptionTypeOk

`func (o *ApiValidateOptionRequest) GetOptionTypeOk() (*string, bool)`

GetOptionTypeOk returns a tuple with the OptionType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionType

`func (o *ApiValidateOptionRequest) SetOptionType(v string)`

SetOptionType sets OptionType field to given value.

### HasOptionType

`func (o *ApiValidateOptionRequest) HasOptionType() bool`

HasOptionType returns a boolean if a field has been set.

### GetDefaultStoragePath

`func (o *ApiValidateOptionRequest) GetDefaultStoragePath() string`

GetDefaultStoragePath returns the DefaultStoragePath field if non-nil, zero value otherwise.

### GetDefaultStoragePathOk

`func (o *ApiValidateOptionRequest) GetDefaultStoragePathOk() (*string, bool)`

GetDefaultStoragePathOk returns a tuple with the DefaultStoragePath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultStoragePath

`func (o *ApiValidateOptionRequest) SetDefaultStoragePath(v string)`

SetDefaultStoragePath sets DefaultStoragePath field to given value.

### HasDefaultStoragePath

`func (o *ApiValidateOptionRequest) HasDefaultStoragePath() bool`

HasDefaultStoragePath returns a boolean if a field has been set.

### GetRealValuesUrl

`func (o *ApiValidateOptionRequest) GetRealValuesUrl() string`

GetRealValuesUrl returns the RealValuesUrl field if non-nil, zero value otherwise.

### GetRealValuesUrlOk

`func (o *ApiValidateOptionRequest) GetRealValuesUrlOk() (*string, bool)`

GetRealValuesUrlOk returns a tuple with the RealValuesUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRealValuesUrl

`func (o *ApiValidateOptionRequest) SetRealValuesUrl(v string)`

SetRealValuesUrl sets RealValuesUrl field to given value.

### HasRealValuesUrl

`func (o *ApiValidateOptionRequest) HasRealValuesUrl() bool`

HasRealValuesUrl returns a boolean if a field has been set.

### GetDefaultValue

`func (o *ApiValidateOptionRequest) GetDefaultValue() string`

GetDefaultValue returns the DefaultValue field if non-nil, zero value otherwise.

### GetDefaultValueOk

`func (o *ApiValidateOptionRequest) GetDefaultValueOk() (*string, bool)`

GetDefaultValueOk returns a tuple with the DefaultValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultValue

`func (o *ApiValidateOptionRequest) SetDefaultValue(v string)`

SetDefaultValue sets DefaultValue field to given value.

### HasDefaultValue

`func (o *ApiValidateOptionRequest) HasDefaultValue() bool`

HasDefaultValue returns a boolean if a field has been set.

### GetValuesList

`func (o *ApiValidateOptionRequest) GetValuesList() string`

GetValuesList returns the ValuesList field if non-nil, zero value otherwise.

### GetValuesListOk

`func (o *ApiValidateOptionRequest) GetValuesListOk() (*string, bool)`

GetValuesListOk returns a tuple with the ValuesList field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesList

`func (o *ApiValidateOptionRequest) SetValuesList(v string)`

SetValuesList sets ValuesList field to given value.

### HasValuesList

`func (o *ApiValidateOptionRequest) HasValuesList() bool`

HasValuesList returns a boolean if a field has been set.

### GetOptionValues

`func (o *ApiValidateOptionRequest) GetOptionValues() []string`

GetOptionValues returns the OptionValues field if non-nil, zero value otherwise.

### GetOptionValuesOk

`func (o *ApiValidateOptionRequest) GetOptionValuesOk() (*[]string, bool)`

GetOptionValuesOk returns a tuple with the OptionValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionValues

`func (o *ApiValidateOptionRequest) SetOptionValues(v []string)`

SetOptionValues sets OptionValues field to given value.

### HasOptionValues

`func (o *ApiValidateOptionRequest) HasOptionValues() bool`

HasOptionValues returns a boolean if a field has been set.

### GetSecureInput

`func (o *ApiValidateOptionRequest) GetSecureInput() bool`

GetSecureInput returns the SecureInput field if non-nil, zero value otherwise.

### GetSecureInputOk

`func (o *ApiValidateOptionRequest) GetSecureInputOk() (*bool, bool)`

GetSecureInputOk returns a tuple with the SecureInput field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecureInput

`func (o *ApiValidateOptionRequest) SetSecureInput(v bool)`

SetSecureInput sets SecureInput field to given value.

### HasSecureInput

`func (o *ApiValidateOptionRequest) HasSecureInput() bool`

HasSecureInput returns a boolean if a field has been set.

### GetSecureExposed

`func (o *ApiValidateOptionRequest) GetSecureExposed() bool`

GetSecureExposed returns the SecureExposed field if non-nil, zero value otherwise.

### GetSecureExposedOk

`func (o *ApiValidateOptionRequest) GetSecureExposedOk() (*bool, bool)`

GetSecureExposedOk returns a tuple with the SecureExposed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecureExposed

`func (o *ApiValidateOptionRequest) SetSecureExposed(v bool)`

SetSecureExposed sets SecureExposed field to given value.

### HasSecureExposed

`func (o *ApiValidateOptionRequest) HasSecureExposed() bool`

HasSecureExposed returns a boolean if a field has been set.

### GetOptionData

`func (o *ApiValidateOptionRequest) GetOptionData() OptionValidateRequest`

GetOptionData returns the OptionData field if non-nil, zero value otherwise.

### GetOptionDataOk

`func (o *ApiValidateOptionRequest) GetOptionDataOk() (*OptionValidateRequest, bool)`

GetOptionDataOk returns a tuple with the OptionData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionData

`func (o *ApiValidateOptionRequest) SetOptionData(v OptionValidateRequest)`

SetOptionData sets OptionData field to given value.

### HasOptionData

`func (o *ApiValidateOptionRequest) HasOptionData() bool`

HasOptionData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



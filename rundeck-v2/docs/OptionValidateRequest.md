# OptionValidateRequest

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

## Methods

### NewOptionValidateRequest

`func NewOptionValidateRequest() *OptionValidateRequest`

NewOptionValidateRequest instantiates a new OptionValidateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOptionValidateRequestWithDefaults

`func NewOptionValidateRequestWithDefaults() *OptionValidateRequest`

NewOptionValidateRequestWithDefaults instantiates a new OptionValidateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *OptionValidateRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *OptionValidateRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *OptionValidateRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *OptionValidateRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetStoragePath

`func (o *OptionValidateRequest) GetStoragePath() string`

GetStoragePath returns the StoragePath field if non-nil, zero value otherwise.

### GetStoragePathOk

`func (o *OptionValidateRequest) GetStoragePathOk() (*string, bool)`

GetStoragePathOk returns a tuple with the StoragePath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStoragePath

`func (o *OptionValidateRequest) SetStoragePath(v string)`

SetStoragePath sets StoragePath field to given value.

### HasStoragePath

`func (o *OptionValidateRequest) HasStoragePath() bool`

HasStoragePath returns a boolean if a field has been set.

### GetValuesUrl

`func (o *OptionValidateRequest) GetValuesUrl() string`

GetValuesUrl returns the ValuesUrl field if non-nil, zero value otherwise.

### GetValuesUrlOk

`func (o *OptionValidateRequest) GetValuesUrlOk() (*string, bool)`

GetValuesUrlOk returns a tuple with the ValuesUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesUrl

`func (o *OptionValidateRequest) SetValuesUrl(v string)`

SetValuesUrl sets ValuesUrl field to given value.

### HasValuesUrl

`func (o *OptionValidateRequest) HasValuesUrl() bool`

HasValuesUrl returns a boolean if a field has been set.

### GetValue

`func (o *OptionValidateRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *OptionValidateRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *OptionValidateRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *OptionValidateRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetValues

`func (o *OptionValidateRequest) GetValues() []string`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *OptionValidateRequest) GetValuesOk() (*[]string, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *OptionValidateRequest) SetValues(v []string)`

SetValues sets Values field to given value.

### HasValues

`func (o *OptionValidateRequest) HasValues() bool`

HasValues returns a boolean if a field has been set.

### GetSecure

`func (o *OptionValidateRequest) GetSecure() bool`

GetSecure returns the Secure field if non-nil, zero value otherwise.

### GetSecureOk

`func (o *OptionValidateRequest) GetSecureOk() (*bool, bool)`

GetSecureOk returns a tuple with the Secure field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecure

`func (o *OptionValidateRequest) SetSecure(v bool)`

SetSecure sets Secure field to given value.

### HasSecure

`func (o *OptionValidateRequest) HasSecure() bool`

HasSecure returns a boolean if a field has been set.

### GetValueExposed

`func (o *OptionValidateRequest) GetValueExposed() bool`

GetValueExposed returns the ValueExposed field if non-nil, zero value otherwise.

### GetValueExposedOk

`func (o *OptionValidateRequest) GetValueExposedOk() (*bool, bool)`

GetValueExposedOk returns a tuple with the ValueExposed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValueExposed

`func (o *OptionValidateRequest) SetValueExposed(v bool)`

SetValueExposed sets ValueExposed field to given value.

### HasValueExposed

`func (o *OptionValidateRequest) HasValueExposed() bool`

HasValueExposed returns a boolean if a field has been set.

### GetValuesType

`func (o *OptionValidateRequest) GetValuesType() string`

GetValuesType returns the ValuesType field if non-nil, zero value otherwise.

### GetValuesTypeOk

`func (o *OptionValidateRequest) GetValuesTypeOk() (*string, bool)`

GetValuesTypeOk returns a tuple with the ValuesType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesType

`func (o *OptionValidateRequest) SetValuesType(v string)`

SetValuesType sets ValuesType field to given value.

### HasValuesType

`func (o *OptionValidateRequest) HasValuesType() bool`

HasValuesType returns a boolean if a field has been set.

### GetRemoteUrlAuthenticationType

`func (o *OptionValidateRequest) GetRemoteUrlAuthenticationType() string`

GetRemoteUrlAuthenticationType returns the RemoteUrlAuthenticationType field if non-nil, zero value otherwise.

### GetRemoteUrlAuthenticationTypeOk

`func (o *OptionValidateRequest) GetRemoteUrlAuthenticationTypeOk() (*string, bool)`

GetRemoteUrlAuthenticationTypeOk returns a tuple with the RemoteUrlAuthenticationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoteUrlAuthenticationType

`func (o *OptionValidateRequest) SetRemoteUrlAuthenticationType(v string)`

SetRemoteUrlAuthenticationType sets RemoteUrlAuthenticationType field to given value.

### HasRemoteUrlAuthenticationType

`func (o *OptionValidateRequest) HasRemoteUrlAuthenticationType() bool`

HasRemoteUrlAuthenticationType returns a boolean if a field has been set.

### GetConfigRemoteUrl

`func (o *OptionValidateRequest) GetConfigRemoteUrl() map[string]interface{}`

GetConfigRemoteUrl returns the ConfigRemoteUrl field if non-nil, zero value otherwise.

### GetConfigRemoteUrlOk

`func (o *OptionValidateRequest) GetConfigRemoteUrlOk() (*map[string]interface{}, bool)`

GetConfigRemoteUrlOk returns a tuple with the ConfigRemoteUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigRemoteUrl

`func (o *OptionValidateRequest) SetConfigRemoteUrl(v map[string]interface{})`

SetConfigRemoteUrl sets ConfigRemoteUrl field to given value.

### HasConfigRemoteUrl

`func (o *OptionValidateRequest) HasConfigRemoteUrl() bool`

HasConfigRemoteUrl returns a boolean if a field has been set.

### GetOptionType

`func (o *OptionValidateRequest) GetOptionType() string`

GetOptionType returns the OptionType field if non-nil, zero value otherwise.

### GetOptionTypeOk

`func (o *OptionValidateRequest) GetOptionTypeOk() (*string, bool)`

GetOptionTypeOk returns a tuple with the OptionType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionType

`func (o *OptionValidateRequest) SetOptionType(v string)`

SetOptionType sets OptionType field to given value.

### HasOptionType

`func (o *OptionValidateRequest) HasOptionType() bool`

HasOptionType returns a boolean if a field has been set.

### GetDefaultStoragePath

`func (o *OptionValidateRequest) GetDefaultStoragePath() string`

GetDefaultStoragePath returns the DefaultStoragePath field if non-nil, zero value otherwise.

### GetDefaultStoragePathOk

`func (o *OptionValidateRequest) GetDefaultStoragePathOk() (*string, bool)`

GetDefaultStoragePathOk returns a tuple with the DefaultStoragePath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultStoragePath

`func (o *OptionValidateRequest) SetDefaultStoragePath(v string)`

SetDefaultStoragePath sets DefaultStoragePath field to given value.

### HasDefaultStoragePath

`func (o *OptionValidateRequest) HasDefaultStoragePath() bool`

HasDefaultStoragePath returns a boolean if a field has been set.

### GetRealValuesUrl

`func (o *OptionValidateRequest) GetRealValuesUrl() string`

GetRealValuesUrl returns the RealValuesUrl field if non-nil, zero value otherwise.

### GetRealValuesUrlOk

`func (o *OptionValidateRequest) GetRealValuesUrlOk() (*string, bool)`

GetRealValuesUrlOk returns a tuple with the RealValuesUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRealValuesUrl

`func (o *OptionValidateRequest) SetRealValuesUrl(v string)`

SetRealValuesUrl sets RealValuesUrl field to given value.

### HasRealValuesUrl

`func (o *OptionValidateRequest) HasRealValuesUrl() bool`

HasRealValuesUrl returns a boolean if a field has been set.

### GetDefaultValue

`func (o *OptionValidateRequest) GetDefaultValue() string`

GetDefaultValue returns the DefaultValue field if non-nil, zero value otherwise.

### GetDefaultValueOk

`func (o *OptionValidateRequest) GetDefaultValueOk() (*string, bool)`

GetDefaultValueOk returns a tuple with the DefaultValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultValue

`func (o *OptionValidateRequest) SetDefaultValue(v string)`

SetDefaultValue sets DefaultValue field to given value.

### HasDefaultValue

`func (o *OptionValidateRequest) HasDefaultValue() bool`

HasDefaultValue returns a boolean if a field has been set.

### GetValuesList

`func (o *OptionValidateRequest) GetValuesList() string`

GetValuesList returns the ValuesList field if non-nil, zero value otherwise.

### GetValuesListOk

`func (o *OptionValidateRequest) GetValuesListOk() (*string, bool)`

GetValuesListOk returns a tuple with the ValuesList field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesList

`func (o *OptionValidateRequest) SetValuesList(v string)`

SetValuesList sets ValuesList field to given value.

### HasValuesList

`func (o *OptionValidateRequest) HasValuesList() bool`

HasValuesList returns a boolean if a field has been set.

### GetOptionValues

`func (o *OptionValidateRequest) GetOptionValues() []string`

GetOptionValues returns the OptionValues field if non-nil, zero value otherwise.

### GetOptionValuesOk

`func (o *OptionValidateRequest) GetOptionValuesOk() (*[]string, bool)`

GetOptionValuesOk returns a tuple with the OptionValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionValues

`func (o *OptionValidateRequest) SetOptionValues(v []string)`

SetOptionValues sets OptionValues field to given value.

### HasOptionValues

`func (o *OptionValidateRequest) HasOptionValues() bool`

HasOptionValues returns a boolean if a field has been set.

### GetSecureInput

`func (o *OptionValidateRequest) GetSecureInput() bool`

GetSecureInput returns the SecureInput field if non-nil, zero value otherwise.

### GetSecureInputOk

`func (o *OptionValidateRequest) GetSecureInputOk() (*bool, bool)`

GetSecureInputOk returns a tuple with the SecureInput field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecureInput

`func (o *OptionValidateRequest) SetSecureInput(v bool)`

SetSecureInput sets SecureInput field to given value.

### HasSecureInput

`func (o *OptionValidateRequest) HasSecureInput() bool`

HasSecureInput returns a boolean if a field has been set.

### GetSecureExposed

`func (o *OptionValidateRequest) GetSecureExposed() bool`

GetSecureExposed returns the SecureExposed field if non-nil, zero value otherwise.

### GetSecureExposedOk

`func (o *OptionValidateRequest) GetSecureExposedOk() (*bool, bool)`

GetSecureExposedOk returns a tuple with the SecureExposed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecureExposed

`func (o *OptionValidateRequest) SetSecureExposed(v bool)`

SetSecureExposed sets SecureExposed field to given value.

### HasSecureExposed

`func (o *OptionValidateRequest) HasSecureExposed() bool`

HasSecureExposed returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



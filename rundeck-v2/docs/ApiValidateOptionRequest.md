# ApiValidateOptionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ValuesFromPlugin** | Pointer to [**[]RdOptionValue**](RdOptionValue.md) |  | [optional] 
**OptionValues** | Pointer to **[]string** |  | [optional] 
**ConfigMap** | Pointer to **map[string]map[string]interface{}** |  | [optional] 
**Errors** | Pointer to [**Errors**](Errors.md) |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**SortIndex** | Pointer to **int32** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**DefaultValue** | Pointer to **string** |  | [optional] 
**DefaultStoragePath** | Pointer to **string** |  | [optional] 
**Enforced** | Pointer to **bool** |  | [optional] 
**Required** | Pointer to **bool** |  | [optional] 
**IsDate** | Pointer to **bool** |  | [optional] 
**DateFormat** | Pointer to **string** |  | [optional] 
**Label** | Pointer to **string** |  | [optional] 
**RealValuesUrl** | Pointer to **string** |  | [optional] 
**Regex** | Pointer to **string** |  | [optional] 
**ValuesList** | Pointer to **string** |  | [optional] 
**ValuesListDelimiter** | Pointer to **string** |  | [optional] 
**Multivalued** | Pointer to **bool** |  | [optional] 
**Delimiter** | Pointer to **string** |  | [optional] 
**SecureInput** | Pointer to **bool** |  | [optional] 
**SecureExposed** | Pointer to **bool** |  | [optional] 
**OptionType** | Pointer to **string** |  | [optional] 
**MultivalueAllSelected** | Pointer to **bool** |  | [optional] 
**OptionValuesPluginType** | Pointer to **string** |  | [optional] 
**Hidden** | Pointer to **bool** |  | [optional] 
**SortValues** | Pointer to **bool** |  | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**StoragePath** | Pointer to **string** |  | [optional] 
**ValuesUrl** | Pointer to **string** |  | [optional] 
**Value** | Pointer to **string** |  | [optional] 
**Values** | Pointer to **[]string** |  | [optional] 
**Secure** | Pointer to **bool** |  | [optional] 
**ValueExposed** | Pointer to **bool** |  | [optional] 
**ValuesType** | Pointer to **string** |  | [optional] 
**RemoteUrlAuthenticationType** | Pointer to **string** |  | [optional] 
**ConfigRemoteUrl** | Pointer to **map[string]map[string]interface{}** |  | [optional] 
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

### GetValuesFromPlugin

`func (o *ApiValidateOptionRequest) GetValuesFromPlugin() []RdOptionValue`

GetValuesFromPlugin returns the ValuesFromPlugin field if non-nil, zero value otherwise.

### GetValuesFromPluginOk

`func (o *ApiValidateOptionRequest) GetValuesFromPluginOk() (*[]RdOptionValue, bool)`

GetValuesFromPluginOk returns a tuple with the ValuesFromPlugin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesFromPlugin

`func (o *ApiValidateOptionRequest) SetValuesFromPlugin(v []RdOptionValue)`

SetValuesFromPlugin sets ValuesFromPlugin field to given value.

### HasValuesFromPlugin

`func (o *ApiValidateOptionRequest) HasValuesFromPlugin() bool`

HasValuesFromPlugin returns a boolean if a field has been set.

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

### GetConfigMap

`func (o *ApiValidateOptionRequest) GetConfigMap() map[string]map[string]interface{}`

GetConfigMap returns the ConfigMap field if non-nil, zero value otherwise.

### GetConfigMapOk

`func (o *ApiValidateOptionRequest) GetConfigMapOk() (*map[string]map[string]interface{}, bool)`

GetConfigMapOk returns a tuple with the ConfigMap field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigMap

`func (o *ApiValidateOptionRequest) SetConfigMap(v map[string]map[string]interface{})`

SetConfigMap sets ConfigMap field to given value.

### HasConfigMap

`func (o *ApiValidateOptionRequest) HasConfigMap() bool`

HasConfigMap returns a boolean if a field has been set.

### GetErrors

`func (o *ApiValidateOptionRequest) GetErrors() Errors`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *ApiValidateOptionRequest) GetErrorsOk() (*Errors, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *ApiValidateOptionRequest) SetErrors(v Errors)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *ApiValidateOptionRequest) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetName

`func (o *ApiValidateOptionRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApiValidateOptionRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApiValidateOptionRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ApiValidateOptionRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetSortIndex

`func (o *ApiValidateOptionRequest) GetSortIndex() int32`

GetSortIndex returns the SortIndex field if non-nil, zero value otherwise.

### GetSortIndexOk

`func (o *ApiValidateOptionRequest) GetSortIndexOk() (*int32, bool)`

GetSortIndexOk returns a tuple with the SortIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortIndex

`func (o *ApiValidateOptionRequest) SetSortIndex(v int32)`

SetSortIndex sets SortIndex field to given value.

### HasSortIndex

`func (o *ApiValidateOptionRequest) HasSortIndex() bool`

HasSortIndex returns a boolean if a field has been set.

### GetDescription

`func (o *ApiValidateOptionRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ApiValidateOptionRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ApiValidateOptionRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ApiValidateOptionRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

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

### GetEnforced

`func (o *ApiValidateOptionRequest) GetEnforced() bool`

GetEnforced returns the Enforced field if non-nil, zero value otherwise.

### GetEnforcedOk

`func (o *ApiValidateOptionRequest) GetEnforcedOk() (*bool, bool)`

GetEnforcedOk returns a tuple with the Enforced field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnforced

`func (o *ApiValidateOptionRequest) SetEnforced(v bool)`

SetEnforced sets Enforced field to given value.

### HasEnforced

`func (o *ApiValidateOptionRequest) HasEnforced() bool`

HasEnforced returns a boolean if a field has been set.

### GetRequired

`func (o *ApiValidateOptionRequest) GetRequired() bool`

GetRequired returns the Required field if non-nil, zero value otherwise.

### GetRequiredOk

`func (o *ApiValidateOptionRequest) GetRequiredOk() (*bool, bool)`

GetRequiredOk returns a tuple with the Required field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequired

`func (o *ApiValidateOptionRequest) SetRequired(v bool)`

SetRequired sets Required field to given value.

### HasRequired

`func (o *ApiValidateOptionRequest) HasRequired() bool`

HasRequired returns a boolean if a field has been set.

### GetIsDate

`func (o *ApiValidateOptionRequest) GetIsDate() bool`

GetIsDate returns the IsDate field if non-nil, zero value otherwise.

### GetIsDateOk

`func (o *ApiValidateOptionRequest) GetIsDateOk() (*bool, bool)`

GetIsDateOk returns a tuple with the IsDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDate

`func (o *ApiValidateOptionRequest) SetIsDate(v bool)`

SetIsDate sets IsDate field to given value.

### HasIsDate

`func (o *ApiValidateOptionRequest) HasIsDate() bool`

HasIsDate returns a boolean if a field has been set.

### GetDateFormat

`func (o *ApiValidateOptionRequest) GetDateFormat() string`

GetDateFormat returns the DateFormat field if non-nil, zero value otherwise.

### GetDateFormatOk

`func (o *ApiValidateOptionRequest) GetDateFormatOk() (*string, bool)`

GetDateFormatOk returns a tuple with the DateFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateFormat

`func (o *ApiValidateOptionRequest) SetDateFormat(v string)`

SetDateFormat sets DateFormat field to given value.

### HasDateFormat

`func (o *ApiValidateOptionRequest) HasDateFormat() bool`

HasDateFormat returns a boolean if a field has been set.

### GetLabel

`func (o *ApiValidateOptionRequest) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *ApiValidateOptionRequest) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *ApiValidateOptionRequest) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *ApiValidateOptionRequest) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

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

### GetRegex

`func (o *ApiValidateOptionRequest) GetRegex() string`

GetRegex returns the Regex field if non-nil, zero value otherwise.

### GetRegexOk

`func (o *ApiValidateOptionRequest) GetRegexOk() (*string, bool)`

GetRegexOk returns a tuple with the Regex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegex

`func (o *ApiValidateOptionRequest) SetRegex(v string)`

SetRegex sets Regex field to given value.

### HasRegex

`func (o *ApiValidateOptionRequest) HasRegex() bool`

HasRegex returns a boolean if a field has been set.

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

### GetValuesListDelimiter

`func (o *ApiValidateOptionRequest) GetValuesListDelimiter() string`

GetValuesListDelimiter returns the ValuesListDelimiter field if non-nil, zero value otherwise.

### GetValuesListDelimiterOk

`func (o *ApiValidateOptionRequest) GetValuesListDelimiterOk() (*string, bool)`

GetValuesListDelimiterOk returns a tuple with the ValuesListDelimiter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesListDelimiter

`func (o *ApiValidateOptionRequest) SetValuesListDelimiter(v string)`

SetValuesListDelimiter sets ValuesListDelimiter field to given value.

### HasValuesListDelimiter

`func (o *ApiValidateOptionRequest) HasValuesListDelimiter() bool`

HasValuesListDelimiter returns a boolean if a field has been set.

### GetMultivalued

`func (o *ApiValidateOptionRequest) GetMultivalued() bool`

GetMultivalued returns the Multivalued field if non-nil, zero value otherwise.

### GetMultivaluedOk

`func (o *ApiValidateOptionRequest) GetMultivaluedOk() (*bool, bool)`

GetMultivaluedOk returns a tuple with the Multivalued field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMultivalued

`func (o *ApiValidateOptionRequest) SetMultivalued(v bool)`

SetMultivalued sets Multivalued field to given value.

### HasMultivalued

`func (o *ApiValidateOptionRequest) HasMultivalued() bool`

HasMultivalued returns a boolean if a field has been set.

### GetDelimiter

`func (o *ApiValidateOptionRequest) GetDelimiter() string`

GetDelimiter returns the Delimiter field if non-nil, zero value otherwise.

### GetDelimiterOk

`func (o *ApiValidateOptionRequest) GetDelimiterOk() (*string, bool)`

GetDelimiterOk returns a tuple with the Delimiter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDelimiter

`func (o *ApiValidateOptionRequest) SetDelimiter(v string)`

SetDelimiter sets Delimiter field to given value.

### HasDelimiter

`func (o *ApiValidateOptionRequest) HasDelimiter() bool`

HasDelimiter returns a boolean if a field has been set.

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

### GetMultivalueAllSelected

`func (o *ApiValidateOptionRequest) GetMultivalueAllSelected() bool`

GetMultivalueAllSelected returns the MultivalueAllSelected field if non-nil, zero value otherwise.

### GetMultivalueAllSelectedOk

`func (o *ApiValidateOptionRequest) GetMultivalueAllSelectedOk() (*bool, bool)`

GetMultivalueAllSelectedOk returns a tuple with the MultivalueAllSelected field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMultivalueAllSelected

`func (o *ApiValidateOptionRequest) SetMultivalueAllSelected(v bool)`

SetMultivalueAllSelected sets MultivalueAllSelected field to given value.

### HasMultivalueAllSelected

`func (o *ApiValidateOptionRequest) HasMultivalueAllSelected() bool`

HasMultivalueAllSelected returns a boolean if a field has been set.

### GetOptionValuesPluginType

`func (o *ApiValidateOptionRequest) GetOptionValuesPluginType() string`

GetOptionValuesPluginType returns the OptionValuesPluginType field if non-nil, zero value otherwise.

### GetOptionValuesPluginTypeOk

`func (o *ApiValidateOptionRequest) GetOptionValuesPluginTypeOk() (*string, bool)`

GetOptionValuesPluginTypeOk returns a tuple with the OptionValuesPluginType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionValuesPluginType

`func (o *ApiValidateOptionRequest) SetOptionValuesPluginType(v string)`

SetOptionValuesPluginType sets OptionValuesPluginType field to given value.

### HasOptionValuesPluginType

`func (o *ApiValidateOptionRequest) HasOptionValuesPluginType() bool`

HasOptionValuesPluginType returns a boolean if a field has been set.

### GetHidden

`func (o *ApiValidateOptionRequest) GetHidden() bool`

GetHidden returns the Hidden field if non-nil, zero value otherwise.

### GetHiddenOk

`func (o *ApiValidateOptionRequest) GetHiddenOk() (*bool, bool)`

GetHiddenOk returns a tuple with the Hidden field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHidden

`func (o *ApiValidateOptionRequest) SetHidden(v bool)`

SetHidden sets Hidden field to given value.

### HasHidden

`func (o *ApiValidateOptionRequest) HasHidden() bool`

HasHidden returns a boolean if a field has been set.

### GetSortValues

`func (o *ApiValidateOptionRequest) GetSortValues() bool`

GetSortValues returns the SortValues field if non-nil, zero value otherwise.

### GetSortValuesOk

`func (o *ApiValidateOptionRequest) GetSortValuesOk() (*bool, bool)`

GetSortValuesOk returns a tuple with the SortValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortValues

`func (o *ApiValidateOptionRequest) SetSortValues(v bool)`

SetSortValues sets SortValues field to given value.

### HasSortValues

`func (o *ApiValidateOptionRequest) HasSortValues() bool`

HasSortValues returns a boolean if a field has been set.

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

`func (o *ApiValidateOptionRequest) GetConfigRemoteUrl() map[string]map[string]interface{}`

GetConfigRemoteUrl returns the ConfigRemoteUrl field if non-nil, zero value otherwise.

### GetConfigRemoteUrlOk

`func (o *ApiValidateOptionRequest) GetConfigRemoteUrlOk() (*map[string]map[string]interface{}, bool)`

GetConfigRemoteUrlOk returns a tuple with the ConfigRemoteUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigRemoteUrl

`func (o *ApiValidateOptionRequest) SetConfigRemoteUrl(v map[string]map[string]interface{})`

SetConfigRemoteUrl sets ConfigRemoteUrl field to given value.

### HasConfigRemoteUrl

`func (o *ApiValidateOptionRequest) HasConfigRemoteUrl() bool`

HasConfigRemoteUrl returns a boolean if a field has been set.

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



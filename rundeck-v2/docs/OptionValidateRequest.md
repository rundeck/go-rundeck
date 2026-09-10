# OptionValidateRequest

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

### GetValuesFromPlugin

`func (o *OptionValidateRequest) GetValuesFromPlugin() []RdOptionValue`

GetValuesFromPlugin returns the ValuesFromPlugin field if non-nil, zero value otherwise.

### GetValuesFromPluginOk

`func (o *OptionValidateRequest) GetValuesFromPluginOk() (*[]RdOptionValue, bool)`

GetValuesFromPluginOk returns a tuple with the ValuesFromPlugin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesFromPlugin

`func (o *OptionValidateRequest) SetValuesFromPlugin(v []RdOptionValue)`

SetValuesFromPlugin sets ValuesFromPlugin field to given value.

### HasValuesFromPlugin

`func (o *OptionValidateRequest) HasValuesFromPlugin() bool`

HasValuesFromPlugin returns a boolean if a field has been set.

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

### GetConfigMap

`func (o *OptionValidateRequest) GetConfigMap() map[string]map[string]interface{}`

GetConfigMap returns the ConfigMap field if non-nil, zero value otherwise.

### GetConfigMapOk

`func (o *OptionValidateRequest) GetConfigMapOk() (*map[string]map[string]interface{}, bool)`

GetConfigMapOk returns a tuple with the ConfigMap field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigMap

`func (o *OptionValidateRequest) SetConfigMap(v map[string]map[string]interface{})`

SetConfigMap sets ConfigMap field to given value.

### HasConfigMap

`func (o *OptionValidateRequest) HasConfigMap() bool`

HasConfigMap returns a boolean if a field has been set.

### GetErrors

`func (o *OptionValidateRequest) GetErrors() Errors`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *OptionValidateRequest) GetErrorsOk() (*Errors, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *OptionValidateRequest) SetErrors(v Errors)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *OptionValidateRequest) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetName

`func (o *OptionValidateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *OptionValidateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *OptionValidateRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *OptionValidateRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetSortIndex

`func (o *OptionValidateRequest) GetSortIndex() int32`

GetSortIndex returns the SortIndex field if non-nil, zero value otherwise.

### GetSortIndexOk

`func (o *OptionValidateRequest) GetSortIndexOk() (*int32, bool)`

GetSortIndexOk returns a tuple with the SortIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortIndex

`func (o *OptionValidateRequest) SetSortIndex(v int32)`

SetSortIndex sets SortIndex field to given value.

### HasSortIndex

`func (o *OptionValidateRequest) HasSortIndex() bool`

HasSortIndex returns a boolean if a field has been set.

### GetDescription

`func (o *OptionValidateRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *OptionValidateRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *OptionValidateRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *OptionValidateRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

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

### GetEnforced

`func (o *OptionValidateRequest) GetEnforced() bool`

GetEnforced returns the Enforced field if non-nil, zero value otherwise.

### GetEnforcedOk

`func (o *OptionValidateRequest) GetEnforcedOk() (*bool, bool)`

GetEnforcedOk returns a tuple with the Enforced field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnforced

`func (o *OptionValidateRequest) SetEnforced(v bool)`

SetEnforced sets Enforced field to given value.

### HasEnforced

`func (o *OptionValidateRequest) HasEnforced() bool`

HasEnforced returns a boolean if a field has been set.

### GetRequired

`func (o *OptionValidateRequest) GetRequired() bool`

GetRequired returns the Required field if non-nil, zero value otherwise.

### GetRequiredOk

`func (o *OptionValidateRequest) GetRequiredOk() (*bool, bool)`

GetRequiredOk returns a tuple with the Required field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequired

`func (o *OptionValidateRequest) SetRequired(v bool)`

SetRequired sets Required field to given value.

### HasRequired

`func (o *OptionValidateRequest) HasRequired() bool`

HasRequired returns a boolean if a field has been set.

### GetIsDate

`func (o *OptionValidateRequest) GetIsDate() bool`

GetIsDate returns the IsDate field if non-nil, zero value otherwise.

### GetIsDateOk

`func (o *OptionValidateRequest) GetIsDateOk() (*bool, bool)`

GetIsDateOk returns a tuple with the IsDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDate

`func (o *OptionValidateRequest) SetIsDate(v bool)`

SetIsDate sets IsDate field to given value.

### HasIsDate

`func (o *OptionValidateRequest) HasIsDate() bool`

HasIsDate returns a boolean if a field has been set.

### GetDateFormat

`func (o *OptionValidateRequest) GetDateFormat() string`

GetDateFormat returns the DateFormat field if non-nil, zero value otherwise.

### GetDateFormatOk

`func (o *OptionValidateRequest) GetDateFormatOk() (*string, bool)`

GetDateFormatOk returns a tuple with the DateFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateFormat

`func (o *OptionValidateRequest) SetDateFormat(v string)`

SetDateFormat sets DateFormat field to given value.

### HasDateFormat

`func (o *OptionValidateRequest) HasDateFormat() bool`

HasDateFormat returns a boolean if a field has been set.

### GetLabel

`func (o *OptionValidateRequest) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *OptionValidateRequest) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *OptionValidateRequest) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *OptionValidateRequest) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

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

### GetRegex

`func (o *OptionValidateRequest) GetRegex() string`

GetRegex returns the Regex field if non-nil, zero value otherwise.

### GetRegexOk

`func (o *OptionValidateRequest) GetRegexOk() (*string, bool)`

GetRegexOk returns a tuple with the Regex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegex

`func (o *OptionValidateRequest) SetRegex(v string)`

SetRegex sets Regex field to given value.

### HasRegex

`func (o *OptionValidateRequest) HasRegex() bool`

HasRegex returns a boolean if a field has been set.

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

### GetValuesListDelimiter

`func (o *OptionValidateRequest) GetValuesListDelimiter() string`

GetValuesListDelimiter returns the ValuesListDelimiter field if non-nil, zero value otherwise.

### GetValuesListDelimiterOk

`func (o *OptionValidateRequest) GetValuesListDelimiterOk() (*string, bool)`

GetValuesListDelimiterOk returns a tuple with the ValuesListDelimiter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesListDelimiter

`func (o *OptionValidateRequest) SetValuesListDelimiter(v string)`

SetValuesListDelimiter sets ValuesListDelimiter field to given value.

### HasValuesListDelimiter

`func (o *OptionValidateRequest) HasValuesListDelimiter() bool`

HasValuesListDelimiter returns a boolean if a field has been set.

### GetMultivalued

`func (o *OptionValidateRequest) GetMultivalued() bool`

GetMultivalued returns the Multivalued field if non-nil, zero value otherwise.

### GetMultivaluedOk

`func (o *OptionValidateRequest) GetMultivaluedOk() (*bool, bool)`

GetMultivaluedOk returns a tuple with the Multivalued field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMultivalued

`func (o *OptionValidateRequest) SetMultivalued(v bool)`

SetMultivalued sets Multivalued field to given value.

### HasMultivalued

`func (o *OptionValidateRequest) HasMultivalued() bool`

HasMultivalued returns a boolean if a field has been set.

### GetDelimiter

`func (o *OptionValidateRequest) GetDelimiter() string`

GetDelimiter returns the Delimiter field if non-nil, zero value otherwise.

### GetDelimiterOk

`func (o *OptionValidateRequest) GetDelimiterOk() (*string, bool)`

GetDelimiterOk returns a tuple with the Delimiter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDelimiter

`func (o *OptionValidateRequest) SetDelimiter(v string)`

SetDelimiter sets Delimiter field to given value.

### HasDelimiter

`func (o *OptionValidateRequest) HasDelimiter() bool`

HasDelimiter returns a boolean if a field has been set.

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

### GetMultivalueAllSelected

`func (o *OptionValidateRequest) GetMultivalueAllSelected() bool`

GetMultivalueAllSelected returns the MultivalueAllSelected field if non-nil, zero value otherwise.

### GetMultivalueAllSelectedOk

`func (o *OptionValidateRequest) GetMultivalueAllSelectedOk() (*bool, bool)`

GetMultivalueAllSelectedOk returns a tuple with the MultivalueAllSelected field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMultivalueAllSelected

`func (o *OptionValidateRequest) SetMultivalueAllSelected(v bool)`

SetMultivalueAllSelected sets MultivalueAllSelected field to given value.

### HasMultivalueAllSelected

`func (o *OptionValidateRequest) HasMultivalueAllSelected() bool`

HasMultivalueAllSelected returns a boolean if a field has been set.

### GetOptionValuesPluginType

`func (o *OptionValidateRequest) GetOptionValuesPluginType() string`

GetOptionValuesPluginType returns the OptionValuesPluginType field if non-nil, zero value otherwise.

### GetOptionValuesPluginTypeOk

`func (o *OptionValidateRequest) GetOptionValuesPluginTypeOk() (*string, bool)`

GetOptionValuesPluginTypeOk returns a tuple with the OptionValuesPluginType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionValuesPluginType

`func (o *OptionValidateRequest) SetOptionValuesPluginType(v string)`

SetOptionValuesPluginType sets OptionValuesPluginType field to given value.

### HasOptionValuesPluginType

`func (o *OptionValidateRequest) HasOptionValuesPluginType() bool`

HasOptionValuesPluginType returns a boolean if a field has been set.

### GetHidden

`func (o *OptionValidateRequest) GetHidden() bool`

GetHidden returns the Hidden field if non-nil, zero value otherwise.

### GetHiddenOk

`func (o *OptionValidateRequest) GetHiddenOk() (*bool, bool)`

GetHiddenOk returns a tuple with the Hidden field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHidden

`func (o *OptionValidateRequest) SetHidden(v bool)`

SetHidden sets Hidden field to given value.

### HasHidden

`func (o *OptionValidateRequest) HasHidden() bool`

HasHidden returns a boolean if a field has been set.

### GetSortValues

`func (o *OptionValidateRequest) GetSortValues() bool`

GetSortValues returns the SortValues field if non-nil, zero value otherwise.

### GetSortValuesOk

`func (o *OptionValidateRequest) GetSortValuesOk() (*bool, bool)`

GetSortValuesOk returns a tuple with the SortValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortValues

`func (o *OptionValidateRequest) SetSortValues(v bool)`

SetSortValues sets SortValues field to given value.

### HasSortValues

`func (o *OptionValidateRequest) HasSortValues() bool`

HasSortValues returns a boolean if a field has been set.

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

`func (o *OptionValidateRequest) GetConfigRemoteUrl() map[string]map[string]interface{}`

GetConfigRemoteUrl returns the ConfigRemoteUrl field if non-nil, zero value otherwise.

### GetConfigRemoteUrlOk

`func (o *OptionValidateRequest) GetConfigRemoteUrlOk() (*map[string]map[string]interface{}, bool)`

GetConfigRemoteUrlOk returns a tuple with the ConfigRemoteUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigRemoteUrl

`func (o *OptionValidateRequest) SetConfigRemoteUrl(v map[string]map[string]interface{})`

SetConfigRemoteUrl sets ConfigRemoteUrl field to given value.

### HasConfigRemoteUrl

`func (o *OptionValidateRequest) HasConfigRemoteUrl() bool`

HasConfigRemoteUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



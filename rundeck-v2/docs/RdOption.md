# RdOption

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

## Methods

### NewRdOption

`func NewRdOption() *RdOption`

NewRdOption instantiates a new RdOption object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRdOptionWithDefaults

`func NewRdOptionWithDefaults() *RdOption`

NewRdOptionWithDefaults instantiates a new RdOption object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValuesFromPlugin

`func (o *RdOption) GetValuesFromPlugin() []RdOptionValue`

GetValuesFromPlugin returns the ValuesFromPlugin field if non-nil, zero value otherwise.

### GetValuesFromPluginOk

`func (o *RdOption) GetValuesFromPluginOk() (*[]RdOptionValue, bool)`

GetValuesFromPluginOk returns a tuple with the ValuesFromPlugin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesFromPlugin

`func (o *RdOption) SetValuesFromPlugin(v []RdOptionValue)`

SetValuesFromPlugin sets ValuesFromPlugin field to given value.

### HasValuesFromPlugin

`func (o *RdOption) HasValuesFromPlugin() bool`

HasValuesFromPlugin returns a boolean if a field has been set.

### GetOptionValues

`func (o *RdOption) GetOptionValues() []string`

GetOptionValues returns the OptionValues field if non-nil, zero value otherwise.

### GetOptionValuesOk

`func (o *RdOption) GetOptionValuesOk() (*[]string, bool)`

GetOptionValuesOk returns a tuple with the OptionValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionValues

`func (o *RdOption) SetOptionValues(v []string)`

SetOptionValues sets OptionValues field to given value.

### HasOptionValues

`func (o *RdOption) HasOptionValues() bool`

HasOptionValues returns a boolean if a field has been set.

### GetConfigMap

`func (o *RdOption) GetConfigMap() map[string]map[string]interface{}`

GetConfigMap returns the ConfigMap field if non-nil, zero value otherwise.

### GetConfigMapOk

`func (o *RdOption) GetConfigMapOk() (*map[string]map[string]interface{}, bool)`

GetConfigMapOk returns a tuple with the ConfigMap field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigMap

`func (o *RdOption) SetConfigMap(v map[string]map[string]interface{})`

SetConfigMap sets ConfigMap field to given value.

### HasConfigMap

`func (o *RdOption) HasConfigMap() bool`

HasConfigMap returns a boolean if a field has been set.

### GetErrors

`func (o *RdOption) GetErrors() Errors`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *RdOption) GetErrorsOk() (*Errors, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *RdOption) SetErrors(v Errors)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *RdOption) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetName

`func (o *RdOption) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *RdOption) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *RdOption) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *RdOption) HasName() bool`

HasName returns a boolean if a field has been set.

### GetSortIndex

`func (o *RdOption) GetSortIndex() int32`

GetSortIndex returns the SortIndex field if non-nil, zero value otherwise.

### GetSortIndexOk

`func (o *RdOption) GetSortIndexOk() (*int32, bool)`

GetSortIndexOk returns a tuple with the SortIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortIndex

`func (o *RdOption) SetSortIndex(v int32)`

SetSortIndex sets SortIndex field to given value.

### HasSortIndex

`func (o *RdOption) HasSortIndex() bool`

HasSortIndex returns a boolean if a field has been set.

### GetDescription

`func (o *RdOption) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *RdOption) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *RdOption) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *RdOption) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetDefaultValue

`func (o *RdOption) GetDefaultValue() string`

GetDefaultValue returns the DefaultValue field if non-nil, zero value otherwise.

### GetDefaultValueOk

`func (o *RdOption) GetDefaultValueOk() (*string, bool)`

GetDefaultValueOk returns a tuple with the DefaultValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultValue

`func (o *RdOption) SetDefaultValue(v string)`

SetDefaultValue sets DefaultValue field to given value.

### HasDefaultValue

`func (o *RdOption) HasDefaultValue() bool`

HasDefaultValue returns a boolean if a field has been set.

### GetDefaultStoragePath

`func (o *RdOption) GetDefaultStoragePath() string`

GetDefaultStoragePath returns the DefaultStoragePath field if non-nil, zero value otherwise.

### GetDefaultStoragePathOk

`func (o *RdOption) GetDefaultStoragePathOk() (*string, bool)`

GetDefaultStoragePathOk returns a tuple with the DefaultStoragePath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultStoragePath

`func (o *RdOption) SetDefaultStoragePath(v string)`

SetDefaultStoragePath sets DefaultStoragePath field to given value.

### HasDefaultStoragePath

`func (o *RdOption) HasDefaultStoragePath() bool`

HasDefaultStoragePath returns a boolean if a field has been set.

### GetEnforced

`func (o *RdOption) GetEnforced() bool`

GetEnforced returns the Enforced field if non-nil, zero value otherwise.

### GetEnforcedOk

`func (o *RdOption) GetEnforcedOk() (*bool, bool)`

GetEnforcedOk returns a tuple with the Enforced field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnforced

`func (o *RdOption) SetEnforced(v bool)`

SetEnforced sets Enforced field to given value.

### HasEnforced

`func (o *RdOption) HasEnforced() bool`

HasEnforced returns a boolean if a field has been set.

### GetRequired

`func (o *RdOption) GetRequired() bool`

GetRequired returns the Required field if non-nil, zero value otherwise.

### GetRequiredOk

`func (o *RdOption) GetRequiredOk() (*bool, bool)`

GetRequiredOk returns a tuple with the Required field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequired

`func (o *RdOption) SetRequired(v bool)`

SetRequired sets Required field to given value.

### HasRequired

`func (o *RdOption) HasRequired() bool`

HasRequired returns a boolean if a field has been set.

### GetIsDate

`func (o *RdOption) GetIsDate() bool`

GetIsDate returns the IsDate field if non-nil, zero value otherwise.

### GetIsDateOk

`func (o *RdOption) GetIsDateOk() (*bool, bool)`

GetIsDateOk returns a tuple with the IsDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDate

`func (o *RdOption) SetIsDate(v bool)`

SetIsDate sets IsDate field to given value.

### HasIsDate

`func (o *RdOption) HasIsDate() bool`

HasIsDate returns a boolean if a field has been set.

### GetDateFormat

`func (o *RdOption) GetDateFormat() string`

GetDateFormat returns the DateFormat field if non-nil, zero value otherwise.

### GetDateFormatOk

`func (o *RdOption) GetDateFormatOk() (*string, bool)`

GetDateFormatOk returns a tuple with the DateFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateFormat

`func (o *RdOption) SetDateFormat(v string)`

SetDateFormat sets DateFormat field to given value.

### HasDateFormat

`func (o *RdOption) HasDateFormat() bool`

HasDateFormat returns a boolean if a field has been set.

### GetLabel

`func (o *RdOption) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *RdOption) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *RdOption) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *RdOption) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### GetRealValuesUrl

`func (o *RdOption) GetRealValuesUrl() string`

GetRealValuesUrl returns the RealValuesUrl field if non-nil, zero value otherwise.

### GetRealValuesUrlOk

`func (o *RdOption) GetRealValuesUrlOk() (*string, bool)`

GetRealValuesUrlOk returns a tuple with the RealValuesUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRealValuesUrl

`func (o *RdOption) SetRealValuesUrl(v string)`

SetRealValuesUrl sets RealValuesUrl field to given value.

### HasRealValuesUrl

`func (o *RdOption) HasRealValuesUrl() bool`

HasRealValuesUrl returns a boolean if a field has been set.

### GetRegex

`func (o *RdOption) GetRegex() string`

GetRegex returns the Regex field if non-nil, zero value otherwise.

### GetRegexOk

`func (o *RdOption) GetRegexOk() (*string, bool)`

GetRegexOk returns a tuple with the Regex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegex

`func (o *RdOption) SetRegex(v string)`

SetRegex sets Regex field to given value.

### HasRegex

`func (o *RdOption) HasRegex() bool`

HasRegex returns a boolean if a field has been set.

### GetValuesList

`func (o *RdOption) GetValuesList() string`

GetValuesList returns the ValuesList field if non-nil, zero value otherwise.

### GetValuesListOk

`func (o *RdOption) GetValuesListOk() (*string, bool)`

GetValuesListOk returns a tuple with the ValuesList field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesList

`func (o *RdOption) SetValuesList(v string)`

SetValuesList sets ValuesList field to given value.

### HasValuesList

`func (o *RdOption) HasValuesList() bool`

HasValuesList returns a boolean if a field has been set.

### GetValuesListDelimiter

`func (o *RdOption) GetValuesListDelimiter() string`

GetValuesListDelimiter returns the ValuesListDelimiter field if non-nil, zero value otherwise.

### GetValuesListDelimiterOk

`func (o *RdOption) GetValuesListDelimiterOk() (*string, bool)`

GetValuesListDelimiterOk returns a tuple with the ValuesListDelimiter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValuesListDelimiter

`func (o *RdOption) SetValuesListDelimiter(v string)`

SetValuesListDelimiter sets ValuesListDelimiter field to given value.

### HasValuesListDelimiter

`func (o *RdOption) HasValuesListDelimiter() bool`

HasValuesListDelimiter returns a boolean if a field has been set.

### GetMultivalued

`func (o *RdOption) GetMultivalued() bool`

GetMultivalued returns the Multivalued field if non-nil, zero value otherwise.

### GetMultivaluedOk

`func (o *RdOption) GetMultivaluedOk() (*bool, bool)`

GetMultivaluedOk returns a tuple with the Multivalued field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMultivalued

`func (o *RdOption) SetMultivalued(v bool)`

SetMultivalued sets Multivalued field to given value.

### HasMultivalued

`func (o *RdOption) HasMultivalued() bool`

HasMultivalued returns a boolean if a field has been set.

### GetDelimiter

`func (o *RdOption) GetDelimiter() string`

GetDelimiter returns the Delimiter field if non-nil, zero value otherwise.

### GetDelimiterOk

`func (o *RdOption) GetDelimiterOk() (*string, bool)`

GetDelimiterOk returns a tuple with the Delimiter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDelimiter

`func (o *RdOption) SetDelimiter(v string)`

SetDelimiter sets Delimiter field to given value.

### HasDelimiter

`func (o *RdOption) HasDelimiter() bool`

HasDelimiter returns a boolean if a field has been set.

### GetSecureInput

`func (o *RdOption) GetSecureInput() bool`

GetSecureInput returns the SecureInput field if non-nil, zero value otherwise.

### GetSecureInputOk

`func (o *RdOption) GetSecureInputOk() (*bool, bool)`

GetSecureInputOk returns a tuple with the SecureInput field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecureInput

`func (o *RdOption) SetSecureInput(v bool)`

SetSecureInput sets SecureInput field to given value.

### HasSecureInput

`func (o *RdOption) HasSecureInput() bool`

HasSecureInput returns a boolean if a field has been set.

### GetSecureExposed

`func (o *RdOption) GetSecureExposed() bool`

GetSecureExposed returns the SecureExposed field if non-nil, zero value otherwise.

### GetSecureExposedOk

`func (o *RdOption) GetSecureExposedOk() (*bool, bool)`

GetSecureExposedOk returns a tuple with the SecureExposed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecureExposed

`func (o *RdOption) SetSecureExposed(v bool)`

SetSecureExposed sets SecureExposed field to given value.

### HasSecureExposed

`func (o *RdOption) HasSecureExposed() bool`

HasSecureExposed returns a boolean if a field has been set.

### GetOptionType

`func (o *RdOption) GetOptionType() string`

GetOptionType returns the OptionType field if non-nil, zero value otherwise.

### GetOptionTypeOk

`func (o *RdOption) GetOptionTypeOk() (*string, bool)`

GetOptionTypeOk returns a tuple with the OptionType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionType

`func (o *RdOption) SetOptionType(v string)`

SetOptionType sets OptionType field to given value.

### HasOptionType

`func (o *RdOption) HasOptionType() bool`

HasOptionType returns a boolean if a field has been set.

### GetMultivalueAllSelected

`func (o *RdOption) GetMultivalueAllSelected() bool`

GetMultivalueAllSelected returns the MultivalueAllSelected field if non-nil, zero value otherwise.

### GetMultivalueAllSelectedOk

`func (o *RdOption) GetMultivalueAllSelectedOk() (*bool, bool)`

GetMultivalueAllSelectedOk returns a tuple with the MultivalueAllSelected field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMultivalueAllSelected

`func (o *RdOption) SetMultivalueAllSelected(v bool)`

SetMultivalueAllSelected sets MultivalueAllSelected field to given value.

### HasMultivalueAllSelected

`func (o *RdOption) HasMultivalueAllSelected() bool`

HasMultivalueAllSelected returns a boolean if a field has been set.

### GetOptionValuesPluginType

`func (o *RdOption) GetOptionValuesPluginType() string`

GetOptionValuesPluginType returns the OptionValuesPluginType field if non-nil, zero value otherwise.

### GetOptionValuesPluginTypeOk

`func (o *RdOption) GetOptionValuesPluginTypeOk() (*string, bool)`

GetOptionValuesPluginTypeOk returns a tuple with the OptionValuesPluginType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionValuesPluginType

`func (o *RdOption) SetOptionValuesPluginType(v string)`

SetOptionValuesPluginType sets OptionValuesPluginType field to given value.

### HasOptionValuesPluginType

`func (o *RdOption) HasOptionValuesPluginType() bool`

HasOptionValuesPluginType returns a boolean if a field has been set.

### GetHidden

`func (o *RdOption) GetHidden() bool`

GetHidden returns the Hidden field if non-nil, zero value otherwise.

### GetHiddenOk

`func (o *RdOption) GetHiddenOk() (*bool, bool)`

GetHiddenOk returns a tuple with the Hidden field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHidden

`func (o *RdOption) SetHidden(v bool)`

SetHidden sets Hidden field to given value.

### HasHidden

`func (o *RdOption) HasHidden() bool`

HasHidden returns a boolean if a field has been set.

### GetSortValues

`func (o *RdOption) GetSortValues() bool`

GetSortValues returns the SortValues field if non-nil, zero value otherwise.

### GetSortValuesOk

`func (o *RdOption) GetSortValuesOk() (*bool, bool)`

GetSortValuesOk returns a tuple with the SortValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortValues

`func (o *RdOption) SetSortValues(v bool)`

SetSortValues sets SortValues field to given value.

### HasSortValues

`func (o *RdOption) HasSortValues() bool`

HasSortValues returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



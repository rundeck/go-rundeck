# Calendar

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**CalendarType** | Pointer to **string** |  | [optional] 
**Scope** | Pointer to **string** |  | [optional] 
**AllReference** | Pointer to **bool** |  | [optional] 
**Enable** | Pointer to **bool** |  | [optional] 
**DateType** | Pointer to **string** |  | [optional] 
**DateDefinitionJson** | Pointer to **string** |  | [optional] 
**Project** | Pointer to **string** |  | [optional] 
**JsonData** | Pointer to **string** |  | [optional] 
**Recurrent** | Pointer to **bool** |  | [optional] 
**DateCreated** | Pointer to **time.Time** |  | [optional] 
**LastUpdated** | Pointer to **time.Time** |  | [optional] 
**DateDefinition** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Reference** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewCalendar

`func NewCalendar() *Calendar`

NewCalendar instantiates a new Calendar object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalendarWithDefaults

`func NewCalendarWithDefaults() *Calendar`

NewCalendarWithDefaults instantiates a new Calendar object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Calendar) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Calendar) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Calendar) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Calendar) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *Calendar) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Calendar) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Calendar) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Calendar) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetCalendarType

`func (o *Calendar) GetCalendarType() string`

GetCalendarType returns the CalendarType field if non-nil, zero value otherwise.

### GetCalendarTypeOk

`func (o *Calendar) GetCalendarTypeOk() (*string, bool)`

GetCalendarTypeOk returns a tuple with the CalendarType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCalendarType

`func (o *Calendar) SetCalendarType(v string)`

SetCalendarType sets CalendarType field to given value.

### HasCalendarType

`func (o *Calendar) HasCalendarType() bool`

HasCalendarType returns a boolean if a field has been set.

### GetScope

`func (o *Calendar) GetScope() string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *Calendar) GetScopeOk() (*string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *Calendar) SetScope(v string)`

SetScope sets Scope field to given value.

### HasScope

`func (o *Calendar) HasScope() bool`

HasScope returns a boolean if a field has been set.

### GetAllReference

`func (o *Calendar) GetAllReference() bool`

GetAllReference returns the AllReference field if non-nil, zero value otherwise.

### GetAllReferenceOk

`func (o *Calendar) GetAllReferenceOk() (*bool, bool)`

GetAllReferenceOk returns a tuple with the AllReference field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllReference

`func (o *Calendar) SetAllReference(v bool)`

SetAllReference sets AllReference field to given value.

### HasAllReference

`func (o *Calendar) HasAllReference() bool`

HasAllReference returns a boolean if a field has been set.

### GetEnable

`func (o *Calendar) GetEnable() bool`

GetEnable returns the Enable field if non-nil, zero value otherwise.

### GetEnableOk

`func (o *Calendar) GetEnableOk() (*bool, bool)`

GetEnableOk returns a tuple with the Enable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnable

`func (o *Calendar) SetEnable(v bool)`

SetEnable sets Enable field to given value.

### HasEnable

`func (o *Calendar) HasEnable() bool`

HasEnable returns a boolean if a field has been set.

### GetDateType

`func (o *Calendar) GetDateType() string`

GetDateType returns the DateType field if non-nil, zero value otherwise.

### GetDateTypeOk

`func (o *Calendar) GetDateTypeOk() (*string, bool)`

GetDateTypeOk returns a tuple with the DateType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateType

`func (o *Calendar) SetDateType(v string)`

SetDateType sets DateType field to given value.

### HasDateType

`func (o *Calendar) HasDateType() bool`

HasDateType returns a boolean if a field has been set.

### GetDateDefinitionJson

`func (o *Calendar) GetDateDefinitionJson() string`

GetDateDefinitionJson returns the DateDefinitionJson field if non-nil, zero value otherwise.

### GetDateDefinitionJsonOk

`func (o *Calendar) GetDateDefinitionJsonOk() (*string, bool)`

GetDateDefinitionJsonOk returns a tuple with the DateDefinitionJson field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateDefinitionJson

`func (o *Calendar) SetDateDefinitionJson(v string)`

SetDateDefinitionJson sets DateDefinitionJson field to given value.

### HasDateDefinitionJson

`func (o *Calendar) HasDateDefinitionJson() bool`

HasDateDefinitionJson returns a boolean if a field has been set.

### GetProject

`func (o *Calendar) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *Calendar) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *Calendar) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *Calendar) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetJsonData

`func (o *Calendar) GetJsonData() string`

GetJsonData returns the JsonData field if non-nil, zero value otherwise.

### GetJsonDataOk

`func (o *Calendar) GetJsonDataOk() (*string, bool)`

GetJsonDataOk returns a tuple with the JsonData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJsonData

`func (o *Calendar) SetJsonData(v string)`

SetJsonData sets JsonData field to given value.

### HasJsonData

`func (o *Calendar) HasJsonData() bool`

HasJsonData returns a boolean if a field has been set.

### GetRecurrent

`func (o *Calendar) GetRecurrent() bool`

GetRecurrent returns the Recurrent field if non-nil, zero value otherwise.

### GetRecurrentOk

`func (o *Calendar) GetRecurrentOk() (*bool, bool)`

GetRecurrentOk returns a tuple with the Recurrent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecurrent

`func (o *Calendar) SetRecurrent(v bool)`

SetRecurrent sets Recurrent field to given value.

### HasRecurrent

`func (o *Calendar) HasRecurrent() bool`

HasRecurrent returns a boolean if a field has been set.

### GetDateCreated

`func (o *Calendar) GetDateCreated() time.Time`

GetDateCreated returns the DateCreated field if non-nil, zero value otherwise.

### GetDateCreatedOk

`func (o *Calendar) GetDateCreatedOk() (*time.Time, bool)`

GetDateCreatedOk returns a tuple with the DateCreated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateCreated

`func (o *Calendar) SetDateCreated(v time.Time)`

SetDateCreated sets DateCreated field to given value.

### HasDateCreated

`func (o *Calendar) HasDateCreated() bool`

HasDateCreated returns a boolean if a field has been set.

### GetLastUpdated

`func (o *Calendar) GetLastUpdated() time.Time`

GetLastUpdated returns the LastUpdated field if non-nil, zero value otherwise.

### GetLastUpdatedOk

`func (o *Calendar) GetLastUpdatedOk() (*time.Time, bool)`

GetLastUpdatedOk returns a tuple with the LastUpdated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUpdated

`func (o *Calendar) SetLastUpdated(v time.Time)`

SetLastUpdated sets LastUpdated field to given value.

### HasLastUpdated

`func (o *Calendar) HasLastUpdated() bool`

HasLastUpdated returns a boolean if a field has been set.

### GetDateDefinition

`func (o *Calendar) GetDateDefinition() []map[string]interface{}`

GetDateDefinition returns the DateDefinition field if non-nil, zero value otherwise.

### GetDateDefinitionOk

`func (o *Calendar) GetDateDefinitionOk() (*[]map[string]interface{}, bool)`

GetDateDefinitionOk returns a tuple with the DateDefinition field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateDefinition

`func (o *Calendar) SetDateDefinition(v []map[string]interface{})`

SetDateDefinition sets DateDefinition field to given value.

### HasDateDefinition

`func (o *Calendar) HasDateDefinition() bool`

HasDateDefinition returns a boolean if a field has been set.

### GetReference

`func (o *Calendar) GetReference() []map[string]interface{}`

GetReference returns the Reference field if non-nil, zero value otherwise.

### GetReferenceOk

`func (o *Calendar) GetReferenceOk() (*[]map[string]interface{}, bool)`

GetReferenceOk returns a tuple with the Reference field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReference

`func (o *Calendar) SetReference(v []map[string]interface{})`

SetReference sets Reference field to given value.

### HasReference

`func (o *Calendar) HasReference() bool`

HasReference returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



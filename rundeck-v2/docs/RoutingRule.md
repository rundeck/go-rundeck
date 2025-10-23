# RoutingRule

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Debug** | Pointer to **bool** |  | [optional] 
**Enabled** | Pointer to **bool** |  | [optional] 
**Policy** | Pointer to [**PolicyType**](PolicyType.md) |  | [optional] 
**JobId** | Pointer to **string** |  | [optional] 
**JobArgString** | Pointer to **string** |  | [optional] 
**JobOptions** | Pointer to [**[]JobOption**](JobOption.md) |  | [optional] 
**NodeFilter** | Pointer to **string** |  | [optional] 
**User** | Pointer to **string** |  | [optional] 
**Conditions** | Pointer to [**[]Condition**](Condition.md) |  | [optional] 

## Methods

### NewRoutingRule

`func NewRoutingRule() *RoutingRule`

NewRoutingRule instantiates a new RoutingRule object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoutingRuleWithDefaults

`func NewRoutingRuleWithDefaults() *RoutingRule`

NewRoutingRuleWithDefaults instantiates a new RoutingRule object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *RoutingRule) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *RoutingRule) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *RoutingRule) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *RoutingRule) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *RoutingRule) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *RoutingRule) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *RoutingRule) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *RoutingRule) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetDebug

`func (o *RoutingRule) GetDebug() bool`

GetDebug returns the Debug field if non-nil, zero value otherwise.

### GetDebugOk

`func (o *RoutingRule) GetDebugOk() (*bool, bool)`

GetDebugOk returns a tuple with the Debug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDebug

`func (o *RoutingRule) SetDebug(v bool)`

SetDebug sets Debug field to given value.

### HasDebug

`func (o *RoutingRule) HasDebug() bool`

HasDebug returns a boolean if a field has been set.

### GetEnabled

`func (o *RoutingRule) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *RoutingRule) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *RoutingRule) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *RoutingRule) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetPolicy

`func (o *RoutingRule) GetPolicy() PolicyType`

GetPolicy returns the Policy field if non-nil, zero value otherwise.

### GetPolicyOk

`func (o *RoutingRule) GetPolicyOk() (*PolicyType, bool)`

GetPolicyOk returns a tuple with the Policy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicy

`func (o *RoutingRule) SetPolicy(v PolicyType)`

SetPolicy sets Policy field to given value.

### HasPolicy

`func (o *RoutingRule) HasPolicy() bool`

HasPolicy returns a boolean if a field has been set.

### GetJobId

`func (o *RoutingRule) GetJobId() string`

GetJobId returns the JobId field if non-nil, zero value otherwise.

### GetJobIdOk

`func (o *RoutingRule) GetJobIdOk() (*string, bool)`

GetJobIdOk returns a tuple with the JobId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobId

`func (o *RoutingRule) SetJobId(v string)`

SetJobId sets JobId field to given value.

### HasJobId

`func (o *RoutingRule) HasJobId() bool`

HasJobId returns a boolean if a field has been set.

### GetJobArgString

`func (o *RoutingRule) GetJobArgString() string`

GetJobArgString returns the JobArgString field if non-nil, zero value otherwise.

### GetJobArgStringOk

`func (o *RoutingRule) GetJobArgStringOk() (*string, bool)`

GetJobArgStringOk returns a tuple with the JobArgString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobArgString

`func (o *RoutingRule) SetJobArgString(v string)`

SetJobArgString sets JobArgString field to given value.

### HasJobArgString

`func (o *RoutingRule) HasJobArgString() bool`

HasJobArgString returns a boolean if a field has been set.

### GetJobOptions

`func (o *RoutingRule) GetJobOptions() []JobOption`

GetJobOptions returns the JobOptions field if non-nil, zero value otherwise.

### GetJobOptionsOk

`func (o *RoutingRule) GetJobOptionsOk() (*[]JobOption, bool)`

GetJobOptionsOk returns a tuple with the JobOptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobOptions

`func (o *RoutingRule) SetJobOptions(v []JobOption)`

SetJobOptions sets JobOptions field to given value.

### HasJobOptions

`func (o *RoutingRule) HasJobOptions() bool`

HasJobOptions returns a boolean if a field has been set.

### GetNodeFilter

`func (o *RoutingRule) GetNodeFilter() string`

GetNodeFilter returns the NodeFilter field if non-nil, zero value otherwise.

### GetNodeFilterOk

`func (o *RoutingRule) GetNodeFilterOk() (*string, bool)`

GetNodeFilterOk returns a tuple with the NodeFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeFilter

`func (o *RoutingRule) SetNodeFilter(v string)`

SetNodeFilter sets NodeFilter field to given value.

### HasNodeFilter

`func (o *RoutingRule) HasNodeFilter() bool`

HasNodeFilter returns a boolean if a field has been set.

### GetUser

`func (o *RoutingRule) GetUser() string`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *RoutingRule) GetUserOk() (*string, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *RoutingRule) SetUser(v string)`

SetUser sets User field to given value.

### HasUser

`func (o *RoutingRule) HasUser() bool`

HasUser returns a boolean if a field has been set.

### GetConditions

`func (o *RoutingRule) GetConditions() []Condition`

GetConditions returns the Conditions field if non-nil, zero value otherwise.

### GetConditionsOk

`func (o *RoutingRule) GetConditionsOk() (*[]Condition, bool)`

GetConditionsOk returns a tuple with the Conditions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConditions

`func (o *RoutingRule) SetConditions(v []Condition)`

SetConditions sets Conditions field to given value.

### HasConditions

`func (o *RoutingRule) HasConditions() bool`

HasConditions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



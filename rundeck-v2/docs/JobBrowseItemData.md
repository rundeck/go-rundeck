# JobBrowseItemData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Job** | Pointer to **bool** |  | [optional] 
**GroupPath** | Pointer to **string** |  | [optional] 
**JobName** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Id** | Pointer to **string** |  | [optional] 
**Meta** | Pointer to [**[]ItemMeta**](ItemMeta.md) |  | [optional] 

## Methods

### NewJobBrowseItemData

`func NewJobBrowseItemData() *JobBrowseItemData`

NewJobBrowseItemData instantiates a new JobBrowseItemData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobBrowseItemDataWithDefaults

`func NewJobBrowseItemDataWithDefaults() *JobBrowseItemData`

NewJobBrowseItemDataWithDefaults instantiates a new JobBrowseItemData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetJob

`func (o *JobBrowseItemData) GetJob() bool`

GetJob returns the Job field if non-nil, zero value otherwise.

### GetJobOk

`func (o *JobBrowseItemData) GetJobOk() (*bool, bool)`

GetJobOk returns a tuple with the Job field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJob

`func (o *JobBrowseItemData) SetJob(v bool)`

SetJob sets Job field to given value.

### HasJob

`func (o *JobBrowseItemData) HasJob() bool`

HasJob returns a boolean if a field has been set.

### GetGroupPath

`func (o *JobBrowseItemData) GetGroupPath() string`

GetGroupPath returns the GroupPath field if non-nil, zero value otherwise.

### GetGroupPathOk

`func (o *JobBrowseItemData) GetGroupPathOk() (*string, bool)`

GetGroupPathOk returns a tuple with the GroupPath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroupPath

`func (o *JobBrowseItemData) SetGroupPath(v string)`

SetGroupPath sets GroupPath field to given value.

### HasGroupPath

`func (o *JobBrowseItemData) HasGroupPath() bool`

HasGroupPath returns a boolean if a field has been set.

### GetJobName

`func (o *JobBrowseItemData) GetJobName() string`

GetJobName returns the JobName field if non-nil, zero value otherwise.

### GetJobNameOk

`func (o *JobBrowseItemData) GetJobNameOk() (*string, bool)`

GetJobNameOk returns a tuple with the JobName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobName

`func (o *JobBrowseItemData) SetJobName(v string)`

SetJobName sets JobName field to given value.

### HasJobName

`func (o *JobBrowseItemData) HasJobName() bool`

HasJobName returns a boolean if a field has been set.

### GetDescription

`func (o *JobBrowseItemData) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *JobBrowseItemData) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *JobBrowseItemData) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *JobBrowseItemData) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetId

`func (o *JobBrowseItemData) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *JobBrowseItemData) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *JobBrowseItemData) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *JobBrowseItemData) HasId() bool`

HasId returns a boolean if a field has been set.

### GetMeta

`func (o *JobBrowseItemData) GetMeta() []ItemMeta`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *JobBrowseItemData) GetMetaOk() (*[]ItemMeta, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *JobBrowseItemData) SetMeta(v []ItemMeta)`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *JobBrowseItemData) HasMeta() bool`

HasMeta returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



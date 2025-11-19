# JobBrowseResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Path** | Pointer to **string** |  | [optional] 
**Items** | Pointer to [**[]JobBrowseItemData**](JobBrowseItemData.md) |  | [optional] 

## Methods

### NewJobBrowseResponse

`func NewJobBrowseResponse() *JobBrowseResponse`

NewJobBrowseResponse instantiates a new JobBrowseResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobBrowseResponseWithDefaults

`func NewJobBrowseResponseWithDefaults() *JobBrowseResponse`

NewJobBrowseResponseWithDefaults instantiates a new JobBrowseResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPath

`func (o *JobBrowseResponse) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *JobBrowseResponse) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *JobBrowseResponse) SetPath(v string)`

SetPath sets Path field to given value.

### HasPath

`func (o *JobBrowseResponse) HasPath() bool`

HasPath returns a boolean if a field has been set.

### GetItems

`func (o *JobBrowseResponse) GetItems() []JobBrowseItemData`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *JobBrowseResponse) GetItemsOk() (*[]JobBrowseItemData, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *JobBrowseResponse) SetItems(v []JobBrowseItemData)`

SetItems sets Items field to given value.

### HasItems

`func (o *JobBrowseResponse) HasItems() bool`

HasItems returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



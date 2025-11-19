# ExecutionFileInfoList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Paging** | Pointer to [**Paging**](Paging.md) |  | [optional] 
**Files** | [**[]JobFileInfo**](JobFileInfo.md) |  | 

## Methods

### NewExecutionFileInfoList

`func NewExecutionFileInfoList(files []JobFileInfo, ) *ExecutionFileInfoList`

NewExecutionFileInfoList instantiates a new ExecutionFileInfoList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExecutionFileInfoListWithDefaults

`func NewExecutionFileInfoListWithDefaults() *ExecutionFileInfoList`

NewExecutionFileInfoListWithDefaults instantiates a new ExecutionFileInfoList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPaging

`func (o *ExecutionFileInfoList) GetPaging() Paging`

GetPaging returns the Paging field if non-nil, zero value otherwise.

### GetPagingOk

`func (o *ExecutionFileInfoList) GetPagingOk() (*Paging, bool)`

GetPagingOk returns a tuple with the Paging field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaging

`func (o *ExecutionFileInfoList) SetPaging(v Paging)`

SetPaging sets Paging field to given value.

### HasPaging

`func (o *ExecutionFileInfoList) HasPaging() bool`

HasPaging returns a boolean if a field has been set.

### GetFiles

`func (o *ExecutionFileInfoList) GetFiles() []JobFileInfo`

GetFiles returns the Files field if non-nil, zero value otherwise.

### GetFilesOk

`func (o *ExecutionFileInfoList) GetFilesOk() (*[]JobFileInfo, bool)`

GetFilesOk returns a tuple with the Files field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFiles

`func (o *ExecutionFileInfoList) SetFiles(v []JobFileInfo)`

SetFiles sets Files field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



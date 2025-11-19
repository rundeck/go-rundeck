# DataSet

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Label** | Pointer to **string** |  | [optional] 
**Entries** | Pointer to [**[]IDataEntry**](IDataEntry.md) |  | [optional] 
**Big** | Pointer to **bool** |  | [optional] 

## Methods

### NewDataSet

`func NewDataSet() *DataSet`

NewDataSet instantiates a new DataSet object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDataSetWithDefaults

`func NewDataSetWithDefaults() *DataSet`

NewDataSetWithDefaults instantiates a new DataSet object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *DataSet) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *DataSet) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *DataSet) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *DataSet) HasName() bool`

HasName returns a boolean if a field has been set.

### GetLabel

`func (o *DataSet) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *DataSet) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *DataSet) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *DataSet) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### GetEntries

`func (o *DataSet) GetEntries() []IDataEntry`

GetEntries returns the Entries field if non-nil, zero value otherwise.

### GetEntriesOk

`func (o *DataSet) GetEntriesOk() (*[]IDataEntry, bool)`

GetEntriesOk returns a tuple with the Entries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntries

`func (o *DataSet) SetEntries(v []IDataEntry)`

SetEntries sets Entries field to given value.

### HasEntries

`func (o *DataSet) HasEntries() bool`

HasEntries returns a boolean if a field has been set.

### GetBig

`func (o *DataSet) GetBig() bool`

GetBig returns the Big field if non-nil, zero value otherwise.

### GetBigOk

`func (o *DataSet) GetBigOk() (*bool, bool)`

GetBigOk returns a tuple with the Big field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBig

`func (o *DataSet) SetBig(v bool)`

SetBig sets Big field to given value.

### HasBig

`func (o *DataSet) HasBig() bool`

HasBig returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



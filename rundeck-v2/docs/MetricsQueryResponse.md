# MetricsQueryResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | Pointer to **int64** |  | [optional] 
**Duration** | Pointer to [**MetricsQueryResponseDuration**](MetricsQueryResponseDuration.md) |  | [optional] 

## Methods

### NewMetricsQueryResponse

`func NewMetricsQueryResponse() *MetricsQueryResponse`

NewMetricsQueryResponse instantiates a new MetricsQueryResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMetricsQueryResponseWithDefaults

`func NewMetricsQueryResponseWithDefaults() *MetricsQueryResponse`

NewMetricsQueryResponseWithDefaults instantiates a new MetricsQueryResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *MetricsQueryResponse) GetTotal() int64`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *MetricsQueryResponse) GetTotalOk() (*int64, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *MetricsQueryResponse) SetTotal(v int64)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *MetricsQueryResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetDuration

`func (o *MetricsQueryResponse) GetDuration() MetricsQueryResponseDuration`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *MetricsQueryResponse) GetDurationOk() (*MetricsQueryResponseDuration, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *MetricsQueryResponse) SetDuration(v MetricsQueryResponseDuration)`

SetDuration sets Duration field to given value.

### HasDuration

`func (o *MetricsQueryResponse) HasDuration() bool`

HasDuration returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



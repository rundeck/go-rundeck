# UserClassAllocationResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Allocations** | Pointer to **map[string]string** | The current User Class allocation set, as a map of user name to user class name. | [optional] 
**State** | Pointer to **string** | The current state of the user classe allocations. One of: VALID, EXCEEDED, UPGRADED | [optional] 
**Message** | Pointer to **string** |  | [optional] 
**Summary** | Pointer to **map[string]int64** | Current allocations by user class name. | [optional] 
**Exceeded** | Pointer to **map[string]int64** | Exceeded allocations count by user class name. | [optional] 
**Entitled** | Pointer to **map[string]int64** | Entitled allocations count by user class name. | [optional] 

## Methods

### NewUserClassAllocationResponse

`func NewUserClassAllocationResponse() *UserClassAllocationResponse`

NewUserClassAllocationResponse instantiates a new UserClassAllocationResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserClassAllocationResponseWithDefaults

`func NewUserClassAllocationResponseWithDefaults() *UserClassAllocationResponse`

NewUserClassAllocationResponseWithDefaults instantiates a new UserClassAllocationResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAllocations

`func (o *UserClassAllocationResponse) GetAllocations() map[string]string`

GetAllocations returns the Allocations field if non-nil, zero value otherwise.

### GetAllocationsOk

`func (o *UserClassAllocationResponse) GetAllocationsOk() (*map[string]string, bool)`

GetAllocationsOk returns a tuple with the Allocations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllocations

`func (o *UserClassAllocationResponse) SetAllocations(v map[string]string)`

SetAllocations sets Allocations field to given value.

### HasAllocations

`func (o *UserClassAllocationResponse) HasAllocations() bool`

HasAllocations returns a boolean if a field has been set.

### GetState

`func (o *UserClassAllocationResponse) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *UserClassAllocationResponse) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *UserClassAllocationResponse) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *UserClassAllocationResponse) HasState() bool`

HasState returns a boolean if a field has been set.

### GetMessage

`func (o *UserClassAllocationResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *UserClassAllocationResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *UserClassAllocationResponse) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *UserClassAllocationResponse) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetSummary

`func (o *UserClassAllocationResponse) GetSummary() map[string]int64`

GetSummary returns the Summary field if non-nil, zero value otherwise.

### GetSummaryOk

`func (o *UserClassAllocationResponse) GetSummaryOk() (*map[string]int64, bool)`

GetSummaryOk returns a tuple with the Summary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSummary

`func (o *UserClassAllocationResponse) SetSummary(v map[string]int64)`

SetSummary sets Summary field to given value.

### HasSummary

`func (o *UserClassAllocationResponse) HasSummary() bool`

HasSummary returns a boolean if a field has been set.

### GetExceeded

`func (o *UserClassAllocationResponse) GetExceeded() map[string]int64`

GetExceeded returns the Exceeded field if non-nil, zero value otherwise.

### GetExceededOk

`func (o *UserClassAllocationResponse) GetExceededOk() (*map[string]int64, bool)`

GetExceededOk returns a tuple with the Exceeded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExceeded

`func (o *UserClassAllocationResponse) SetExceeded(v map[string]int64)`

SetExceeded sets Exceeded field to given value.

### HasExceeded

`func (o *UserClassAllocationResponse) HasExceeded() bool`

HasExceeded returns a boolean if a field has been set.

### GetEntitled

`func (o *UserClassAllocationResponse) GetEntitled() map[string]int64`

GetEntitled returns the Entitled field if non-nil, zero value otherwise.

### GetEntitledOk

`func (o *UserClassAllocationResponse) GetEntitledOk() (*map[string]int64, bool)`

GetEntitledOk returns a tuple with the Entitled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntitled

`func (o *UserClassAllocationResponse) SetEntitled(v map[string]int64)`

SetEntitled sets Entitled field to given value.

### HasEntitled

`func (o *UserClassAllocationResponse) HasEntitled() bool`

HasEntitled returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



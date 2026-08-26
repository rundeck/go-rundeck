# RdJobQueryInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Errors** | Pointer to [**Errors**](Errors.md) |  | [optional] 
**Max** | Pointer to **int32** |  | [optional] 
**Offset** | Pointer to **int32** |  | [optional] 
**SortOrders** | Pointer to [**[]SortOrder**](SortOrder.md) |  | [optional] 
**SortBy** | Pointer to **string** |  | [optional] 
**SortOrder** | Pointer to **string** |  | [optional] 
**InputParamMap** | Pointer to **map[string]map[string]interface{}** |  | [optional] 
**JobFilter** | Pointer to **string** |  | [optional] 
**JobExactFilter** | Pointer to **string** |  | [optional] 
**ProjFilter** | Pointer to **string** |  | [optional] 
**GroupPath** | Pointer to **string** |  | [optional] 
**GroupPathExact** | Pointer to **string** |  | [optional] 
**DescFilter** | Pointer to **string** |  | [optional] 
**LoglevelFilter** | Pointer to **string** |  | [optional] 
**Idlist** | Pointer to **string** |  | [optional] 
**ScheduledFilter** | Pointer to **bool** |  | [optional] 
**ScheduleEnabledFilter** | Pointer to **bool** |  | [optional] 
**ExecutionEnabledFilter** | Pointer to **bool** |  | [optional] 
**ServerNodeUUIDFilter** | Pointer to **string** |  | [optional] 
**DaysAhead** | Pointer to **int32** |  | [optional] 
**RunJobLaterFilter** | Pointer to **bool** |  | [optional] 
**PaginatedRequired** | Pointer to **bool** |  | [optional] 

## Methods

### NewRdJobQueryInput

`func NewRdJobQueryInput() *RdJobQueryInput`

NewRdJobQueryInput instantiates a new RdJobQueryInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRdJobQueryInputWithDefaults

`func NewRdJobQueryInputWithDefaults() *RdJobQueryInput`

NewRdJobQueryInputWithDefaults instantiates a new RdJobQueryInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetErrors

`func (o *RdJobQueryInput) GetErrors() Errors`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *RdJobQueryInput) GetErrorsOk() (*Errors, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *RdJobQueryInput) SetErrors(v Errors)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *RdJobQueryInput) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetMax

`func (o *RdJobQueryInput) GetMax() int32`

GetMax returns the Max field if non-nil, zero value otherwise.

### GetMaxOk

`func (o *RdJobQueryInput) GetMaxOk() (*int32, bool)`

GetMaxOk returns a tuple with the Max field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMax

`func (o *RdJobQueryInput) SetMax(v int32)`

SetMax sets Max field to given value.

### HasMax

`func (o *RdJobQueryInput) HasMax() bool`

HasMax returns a boolean if a field has been set.

### GetOffset

`func (o *RdJobQueryInput) GetOffset() int32`

GetOffset returns the Offset field if non-nil, zero value otherwise.

### GetOffsetOk

`func (o *RdJobQueryInput) GetOffsetOk() (*int32, bool)`

GetOffsetOk returns a tuple with the Offset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOffset

`func (o *RdJobQueryInput) SetOffset(v int32)`

SetOffset sets Offset field to given value.

### HasOffset

`func (o *RdJobQueryInput) HasOffset() bool`

HasOffset returns a boolean if a field has been set.

### GetSortOrders

`func (o *RdJobQueryInput) GetSortOrders() []SortOrder`

GetSortOrders returns the SortOrders field if non-nil, zero value otherwise.

### GetSortOrdersOk

`func (o *RdJobQueryInput) GetSortOrdersOk() (*[]SortOrder, bool)`

GetSortOrdersOk returns a tuple with the SortOrders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrders

`func (o *RdJobQueryInput) SetSortOrders(v []SortOrder)`

SetSortOrders sets SortOrders field to given value.

### HasSortOrders

`func (o *RdJobQueryInput) HasSortOrders() bool`

HasSortOrders returns a boolean if a field has been set.

### GetSortBy

`func (o *RdJobQueryInput) GetSortBy() string`

GetSortBy returns the SortBy field if non-nil, zero value otherwise.

### GetSortByOk

`func (o *RdJobQueryInput) GetSortByOk() (*string, bool)`

GetSortByOk returns a tuple with the SortBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortBy

`func (o *RdJobQueryInput) SetSortBy(v string)`

SetSortBy sets SortBy field to given value.

### HasSortBy

`func (o *RdJobQueryInput) HasSortBy() bool`

HasSortBy returns a boolean if a field has been set.

### GetSortOrder

`func (o *RdJobQueryInput) GetSortOrder() string`

GetSortOrder returns the SortOrder field if non-nil, zero value otherwise.

### GetSortOrderOk

`func (o *RdJobQueryInput) GetSortOrderOk() (*string, bool)`

GetSortOrderOk returns a tuple with the SortOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrder

`func (o *RdJobQueryInput) SetSortOrder(v string)`

SetSortOrder sets SortOrder field to given value.

### HasSortOrder

`func (o *RdJobQueryInput) HasSortOrder() bool`

HasSortOrder returns a boolean if a field has been set.

### GetInputParamMap

`func (o *RdJobQueryInput) GetInputParamMap() map[string]map[string]interface{}`

GetInputParamMap returns the InputParamMap field if non-nil, zero value otherwise.

### GetInputParamMapOk

`func (o *RdJobQueryInput) GetInputParamMapOk() (*map[string]map[string]interface{}, bool)`

GetInputParamMapOk returns a tuple with the InputParamMap field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInputParamMap

`func (o *RdJobQueryInput) SetInputParamMap(v map[string]map[string]interface{})`

SetInputParamMap sets InputParamMap field to given value.

### HasInputParamMap

`func (o *RdJobQueryInput) HasInputParamMap() bool`

HasInputParamMap returns a boolean if a field has been set.

### GetJobFilter

`func (o *RdJobQueryInput) GetJobFilter() string`

GetJobFilter returns the JobFilter field if non-nil, zero value otherwise.

### GetJobFilterOk

`func (o *RdJobQueryInput) GetJobFilterOk() (*string, bool)`

GetJobFilterOk returns a tuple with the JobFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobFilter

`func (o *RdJobQueryInput) SetJobFilter(v string)`

SetJobFilter sets JobFilter field to given value.

### HasJobFilter

`func (o *RdJobQueryInput) HasJobFilter() bool`

HasJobFilter returns a boolean if a field has been set.

### GetJobExactFilter

`func (o *RdJobQueryInput) GetJobExactFilter() string`

GetJobExactFilter returns the JobExactFilter field if non-nil, zero value otherwise.

### GetJobExactFilterOk

`func (o *RdJobQueryInput) GetJobExactFilterOk() (*string, bool)`

GetJobExactFilterOk returns a tuple with the JobExactFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobExactFilter

`func (o *RdJobQueryInput) SetJobExactFilter(v string)`

SetJobExactFilter sets JobExactFilter field to given value.

### HasJobExactFilter

`func (o *RdJobQueryInput) HasJobExactFilter() bool`

HasJobExactFilter returns a boolean if a field has been set.

### GetProjFilter

`func (o *RdJobQueryInput) GetProjFilter() string`

GetProjFilter returns the ProjFilter field if non-nil, zero value otherwise.

### GetProjFilterOk

`func (o *RdJobQueryInput) GetProjFilterOk() (*string, bool)`

GetProjFilterOk returns a tuple with the ProjFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjFilter

`func (o *RdJobQueryInput) SetProjFilter(v string)`

SetProjFilter sets ProjFilter field to given value.

### HasProjFilter

`func (o *RdJobQueryInput) HasProjFilter() bool`

HasProjFilter returns a boolean if a field has been set.

### GetGroupPath

`func (o *RdJobQueryInput) GetGroupPath() string`

GetGroupPath returns the GroupPath field if non-nil, zero value otherwise.

### GetGroupPathOk

`func (o *RdJobQueryInput) GetGroupPathOk() (*string, bool)`

GetGroupPathOk returns a tuple with the GroupPath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroupPath

`func (o *RdJobQueryInput) SetGroupPath(v string)`

SetGroupPath sets GroupPath field to given value.

### HasGroupPath

`func (o *RdJobQueryInput) HasGroupPath() bool`

HasGroupPath returns a boolean if a field has been set.

### GetGroupPathExact

`func (o *RdJobQueryInput) GetGroupPathExact() string`

GetGroupPathExact returns the GroupPathExact field if non-nil, zero value otherwise.

### GetGroupPathExactOk

`func (o *RdJobQueryInput) GetGroupPathExactOk() (*string, bool)`

GetGroupPathExactOk returns a tuple with the GroupPathExact field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroupPathExact

`func (o *RdJobQueryInput) SetGroupPathExact(v string)`

SetGroupPathExact sets GroupPathExact field to given value.

### HasGroupPathExact

`func (o *RdJobQueryInput) HasGroupPathExact() bool`

HasGroupPathExact returns a boolean if a field has been set.

### GetDescFilter

`func (o *RdJobQueryInput) GetDescFilter() string`

GetDescFilter returns the DescFilter field if non-nil, zero value otherwise.

### GetDescFilterOk

`func (o *RdJobQueryInput) GetDescFilterOk() (*string, bool)`

GetDescFilterOk returns a tuple with the DescFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescFilter

`func (o *RdJobQueryInput) SetDescFilter(v string)`

SetDescFilter sets DescFilter field to given value.

### HasDescFilter

`func (o *RdJobQueryInput) HasDescFilter() bool`

HasDescFilter returns a boolean if a field has been set.

### GetLoglevelFilter

`func (o *RdJobQueryInput) GetLoglevelFilter() string`

GetLoglevelFilter returns the LoglevelFilter field if non-nil, zero value otherwise.

### GetLoglevelFilterOk

`func (o *RdJobQueryInput) GetLoglevelFilterOk() (*string, bool)`

GetLoglevelFilterOk returns a tuple with the LoglevelFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLoglevelFilter

`func (o *RdJobQueryInput) SetLoglevelFilter(v string)`

SetLoglevelFilter sets LoglevelFilter field to given value.

### HasLoglevelFilter

`func (o *RdJobQueryInput) HasLoglevelFilter() bool`

HasLoglevelFilter returns a boolean if a field has been set.

### GetIdlist

`func (o *RdJobQueryInput) GetIdlist() string`

GetIdlist returns the Idlist field if non-nil, zero value otherwise.

### GetIdlistOk

`func (o *RdJobQueryInput) GetIdlistOk() (*string, bool)`

GetIdlistOk returns a tuple with the Idlist field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIdlist

`func (o *RdJobQueryInput) SetIdlist(v string)`

SetIdlist sets Idlist field to given value.

### HasIdlist

`func (o *RdJobQueryInput) HasIdlist() bool`

HasIdlist returns a boolean if a field has been set.

### GetScheduledFilter

`func (o *RdJobQueryInput) GetScheduledFilter() bool`

GetScheduledFilter returns the ScheduledFilter field if non-nil, zero value otherwise.

### GetScheduledFilterOk

`func (o *RdJobQueryInput) GetScheduledFilterOk() (*bool, bool)`

GetScheduledFilterOk returns a tuple with the ScheduledFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScheduledFilter

`func (o *RdJobQueryInput) SetScheduledFilter(v bool)`

SetScheduledFilter sets ScheduledFilter field to given value.

### HasScheduledFilter

`func (o *RdJobQueryInput) HasScheduledFilter() bool`

HasScheduledFilter returns a boolean if a field has been set.

### GetScheduleEnabledFilter

`func (o *RdJobQueryInput) GetScheduleEnabledFilter() bool`

GetScheduleEnabledFilter returns the ScheduleEnabledFilter field if non-nil, zero value otherwise.

### GetScheduleEnabledFilterOk

`func (o *RdJobQueryInput) GetScheduleEnabledFilterOk() (*bool, bool)`

GetScheduleEnabledFilterOk returns a tuple with the ScheduleEnabledFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScheduleEnabledFilter

`func (o *RdJobQueryInput) SetScheduleEnabledFilter(v bool)`

SetScheduleEnabledFilter sets ScheduleEnabledFilter field to given value.

### HasScheduleEnabledFilter

`func (o *RdJobQueryInput) HasScheduleEnabledFilter() bool`

HasScheduleEnabledFilter returns a boolean if a field has been set.

### GetExecutionEnabledFilter

`func (o *RdJobQueryInput) GetExecutionEnabledFilter() bool`

GetExecutionEnabledFilter returns the ExecutionEnabledFilter field if non-nil, zero value otherwise.

### GetExecutionEnabledFilterOk

`func (o *RdJobQueryInput) GetExecutionEnabledFilterOk() (*bool, bool)`

GetExecutionEnabledFilterOk returns a tuple with the ExecutionEnabledFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutionEnabledFilter

`func (o *RdJobQueryInput) SetExecutionEnabledFilter(v bool)`

SetExecutionEnabledFilter sets ExecutionEnabledFilter field to given value.

### HasExecutionEnabledFilter

`func (o *RdJobQueryInput) HasExecutionEnabledFilter() bool`

HasExecutionEnabledFilter returns a boolean if a field has been set.

### GetServerNodeUUIDFilter

`func (o *RdJobQueryInput) GetServerNodeUUIDFilter() string`

GetServerNodeUUIDFilter returns the ServerNodeUUIDFilter field if non-nil, zero value otherwise.

### GetServerNodeUUIDFilterOk

`func (o *RdJobQueryInput) GetServerNodeUUIDFilterOk() (*string, bool)`

GetServerNodeUUIDFilterOk returns a tuple with the ServerNodeUUIDFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServerNodeUUIDFilter

`func (o *RdJobQueryInput) SetServerNodeUUIDFilter(v string)`

SetServerNodeUUIDFilter sets ServerNodeUUIDFilter field to given value.

### HasServerNodeUUIDFilter

`func (o *RdJobQueryInput) HasServerNodeUUIDFilter() bool`

HasServerNodeUUIDFilter returns a boolean if a field has been set.

### GetDaysAhead

`func (o *RdJobQueryInput) GetDaysAhead() int32`

GetDaysAhead returns the DaysAhead field if non-nil, zero value otherwise.

### GetDaysAheadOk

`func (o *RdJobQueryInput) GetDaysAheadOk() (*int32, bool)`

GetDaysAheadOk returns a tuple with the DaysAhead field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDaysAhead

`func (o *RdJobQueryInput) SetDaysAhead(v int32)`

SetDaysAhead sets DaysAhead field to given value.

### HasDaysAhead

`func (o *RdJobQueryInput) HasDaysAhead() bool`

HasDaysAhead returns a boolean if a field has been set.

### GetRunJobLaterFilter

`func (o *RdJobQueryInput) GetRunJobLaterFilter() bool`

GetRunJobLaterFilter returns the RunJobLaterFilter field if non-nil, zero value otherwise.

### GetRunJobLaterFilterOk

`func (o *RdJobQueryInput) GetRunJobLaterFilterOk() (*bool, bool)`

GetRunJobLaterFilterOk returns a tuple with the RunJobLaterFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunJobLaterFilter

`func (o *RdJobQueryInput) SetRunJobLaterFilter(v bool)`

SetRunJobLaterFilter sets RunJobLaterFilter field to given value.

### HasRunJobLaterFilter

`func (o *RdJobQueryInput) HasRunJobLaterFilter() bool`

HasRunJobLaterFilter returns a boolean if a field has been set.

### GetPaginatedRequired

`func (o *RdJobQueryInput) GetPaginatedRequired() bool`

GetPaginatedRequired returns the PaginatedRequired field if non-nil, zero value otherwise.

### GetPaginatedRequiredOk

`func (o *RdJobQueryInput) GetPaginatedRequiredOk() (*bool, bool)`

GetPaginatedRequiredOk returns a tuple with the PaginatedRequired field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaginatedRequired

`func (o *RdJobQueryInput) SetPaginatedRequired(v bool)`

SetPaginatedRequired sets PaginatedRequired field to given value.

### HasPaginatedRequired

`func (o *RdJobQueryInput) HasPaginatedRequired() bool`

HasPaginatedRequired returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



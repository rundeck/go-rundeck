# UserClassAllocationError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | Pointer to **string** |  | [optional] 
**ErrorCode** | Pointer to **string** |  | [optional] 
**Excessions** | Pointer to **map[string]int64** | Exceeded User Class assignments, by user class name | [optional] 
**Limits** | Pointer to **map[string]int64** | Allowed User Class assignment limits, by user class name | [optional] 

## Methods

### NewUserClassAllocationError

`func NewUserClassAllocationError() *UserClassAllocationError`

NewUserClassAllocationError instantiates a new UserClassAllocationError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserClassAllocationErrorWithDefaults

`func NewUserClassAllocationErrorWithDefaults() *UserClassAllocationError`

NewUserClassAllocationErrorWithDefaults instantiates a new UserClassAllocationError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *UserClassAllocationError) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *UserClassAllocationError) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *UserClassAllocationError) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *UserClassAllocationError) HasError() bool`

HasError returns a boolean if a field has been set.

### GetErrorCode

`func (o *UserClassAllocationError) GetErrorCode() string`

GetErrorCode returns the ErrorCode field if non-nil, zero value otherwise.

### GetErrorCodeOk

`func (o *UserClassAllocationError) GetErrorCodeOk() (*string, bool)`

GetErrorCodeOk returns a tuple with the ErrorCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCode

`func (o *UserClassAllocationError) SetErrorCode(v string)`

SetErrorCode sets ErrorCode field to given value.

### HasErrorCode

`func (o *UserClassAllocationError) HasErrorCode() bool`

HasErrorCode returns a boolean if a field has been set.

### GetExcessions

`func (o *UserClassAllocationError) GetExcessions() map[string]int64`

GetExcessions returns the Excessions field if non-nil, zero value otherwise.

### GetExcessionsOk

`func (o *UserClassAllocationError) GetExcessionsOk() (*map[string]int64, bool)`

GetExcessionsOk returns a tuple with the Excessions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExcessions

`func (o *UserClassAllocationError) SetExcessions(v map[string]int64)`

SetExcessions sets Excessions field to given value.

### HasExcessions

`func (o *UserClassAllocationError) HasExcessions() bool`

HasExcessions returns a boolean if a field has been set.

### GetLimits

`func (o *UserClassAllocationError) GetLimits() map[string]int64`

GetLimits returns the Limits field if non-nil, zero value otherwise.

### GetLimitsOk

`func (o *UserClassAllocationError) GetLimitsOk() (*map[string]int64, bool)`

GetLimitsOk returns a tuple with the Limits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimits

`func (o *UserClassAllocationError) SetLimits(v map[string]int64)`

SetLimits sets Limits field to given value.

### HasLimits

`func (o *UserClassAllocationError) HasLimits() bool`

HasLimits returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



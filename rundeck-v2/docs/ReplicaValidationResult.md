# ReplicaValidationResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Valid** | Pointer to **bool** |  | [optional] 
**Errors** | Pointer to **[]string** |  | [optional] 

## Methods

### NewReplicaValidationResult

`func NewReplicaValidationResult() *ReplicaValidationResult`

NewReplicaValidationResult instantiates a new ReplicaValidationResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReplicaValidationResultWithDefaults

`func NewReplicaValidationResultWithDefaults() *ReplicaValidationResult`

NewReplicaValidationResultWithDefaults instantiates a new ReplicaValidationResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValid

`func (o *ReplicaValidationResult) GetValid() bool`

GetValid returns the Valid field if non-nil, zero value otherwise.

### GetValidOk

`func (o *ReplicaValidationResult) GetValidOk() (*bool, bool)`

GetValidOk returns a tuple with the Valid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValid

`func (o *ReplicaValidationResult) SetValid(v bool)`

SetValid sets Valid field to given value.

### HasValid

`func (o *ReplicaValidationResult) HasValid() bool`

HasValid returns a boolean if a field has been set.

### GetErrors

`func (o *ReplicaValidationResult) GetErrors() []string`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *ReplicaValidationResult) GetErrorsOk() (*[]string, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *ReplicaValidationResult) SetErrors(v []string)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *ReplicaValidationResult) HasErrors() bool`

HasErrors returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



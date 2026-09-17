# StartUpResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | Pointer to **string** |  | [optional] 
**ReplicaId** | Pointer to **string** |  | [optional] 
**ReplicaType** | Pointer to **string** |  | [optional] 

## Methods

### NewStartUpResponse

`func NewStartUpResponse() *StartUpResponse`

NewStartUpResponse instantiates a new StartUpResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStartUpResponseWithDefaults

`func NewStartUpResponseWithDefaults() *StartUpResponse`

NewStartUpResponseWithDefaults instantiates a new StartUpResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *StartUpResponse) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *StartUpResponse) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *StartUpResponse) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *StartUpResponse) HasError() bool`

HasError returns a boolean if a field has been set.

### GetReplicaId

`func (o *StartUpResponse) GetReplicaId() string`

GetReplicaId returns the ReplicaId field if non-nil, zero value otherwise.

### GetReplicaIdOk

`func (o *StartUpResponse) GetReplicaIdOk() (*string, bool)`

GetReplicaIdOk returns a tuple with the ReplicaId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaId

`func (o *StartUpResponse) SetReplicaId(v string)`

SetReplicaId sets ReplicaId field to given value.

### HasReplicaId

`func (o *StartUpResponse) HasReplicaId() bool`

HasReplicaId returns a boolean if a field has been set.

### GetReplicaType

`func (o *StartUpResponse) GetReplicaType() string`

GetReplicaType returns the ReplicaType field if non-nil, zero value otherwise.

### GetReplicaTypeOk

`func (o *StartUpResponse) GetReplicaTypeOk() (*string, bool)`

GetReplicaTypeOk returns a tuple with the ReplicaType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaType

`func (o *StartUpResponse) SetReplicaType(v string)`

SetReplicaType sets ReplicaType field to given value.

### HasReplicaType

`func (o *StartUpResponse) HasReplicaType() bool`

HasReplicaType returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



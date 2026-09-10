# NewRunnerReplicaResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Token** | Pointer to **string** | Authentication token for the new Runner replica. | [optional] 
**RunnerId** | Pointer to **string** | Unique Runner ID for the Runner instance. | [optional] 
**ReplicaId** | Pointer to **string** | Unique Runner ID for the Runner replica. | [optional] 
**DownloadTk** | Pointer to **string** | Download token for retrieving Runner resources. | [optional] 
**Filename** | Pointer to **string** | Filename for the downloadable runner JAR artifact | [optional] 

## Methods

### NewNewRunnerReplicaResponse

`func NewNewRunnerReplicaResponse() *NewRunnerReplicaResponse`

NewNewRunnerReplicaResponse instantiates a new NewRunnerReplicaResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewNewRunnerReplicaResponseWithDefaults

`func NewNewRunnerReplicaResponseWithDefaults() *NewRunnerReplicaResponse`

NewNewRunnerReplicaResponseWithDefaults instantiates a new NewRunnerReplicaResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetToken

`func (o *NewRunnerReplicaResponse) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *NewRunnerReplicaResponse) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *NewRunnerReplicaResponse) SetToken(v string)`

SetToken sets Token field to given value.

### HasToken

`func (o *NewRunnerReplicaResponse) HasToken() bool`

HasToken returns a boolean if a field has been set.

### GetRunnerId

`func (o *NewRunnerReplicaResponse) GetRunnerId() string`

GetRunnerId returns the RunnerId field if non-nil, zero value otherwise.

### GetRunnerIdOk

`func (o *NewRunnerReplicaResponse) GetRunnerIdOk() (*string, bool)`

GetRunnerIdOk returns a tuple with the RunnerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunnerId

`func (o *NewRunnerReplicaResponse) SetRunnerId(v string)`

SetRunnerId sets RunnerId field to given value.

### HasRunnerId

`func (o *NewRunnerReplicaResponse) HasRunnerId() bool`

HasRunnerId returns a boolean if a field has been set.

### GetReplicaId

`func (o *NewRunnerReplicaResponse) GetReplicaId() string`

GetReplicaId returns the ReplicaId field if non-nil, zero value otherwise.

### GetReplicaIdOk

`func (o *NewRunnerReplicaResponse) GetReplicaIdOk() (*string, bool)`

GetReplicaIdOk returns a tuple with the ReplicaId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplicaId

`func (o *NewRunnerReplicaResponse) SetReplicaId(v string)`

SetReplicaId sets ReplicaId field to given value.

### HasReplicaId

`func (o *NewRunnerReplicaResponse) HasReplicaId() bool`

HasReplicaId returns a boolean if a field has been set.

### GetDownloadTk

`func (o *NewRunnerReplicaResponse) GetDownloadTk() string`

GetDownloadTk returns the DownloadTk field if non-nil, zero value otherwise.

### GetDownloadTkOk

`func (o *NewRunnerReplicaResponse) GetDownloadTkOk() (*string, bool)`

GetDownloadTkOk returns a tuple with the DownloadTk field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDownloadTk

`func (o *NewRunnerReplicaResponse) SetDownloadTk(v string)`

SetDownloadTk sets DownloadTk field to given value.

### HasDownloadTk

`func (o *NewRunnerReplicaResponse) HasDownloadTk() bool`

HasDownloadTk returns a boolean if a field has been set.

### GetFilename

`func (o *NewRunnerReplicaResponse) GetFilename() string`

GetFilename returns the Filename field if non-nil, zero value otherwise.

### GetFilenameOk

`func (o *NewRunnerReplicaResponse) GetFilenameOk() (*string, bool)`

GetFilenameOk returns a tuple with the Filename field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilename

`func (o *NewRunnerReplicaResponse) SetFilename(v string)`

SetFilename sets Filename field to given value.

### HasFilename

`func (o *NewRunnerReplicaResponse) HasFilename() bool`

HasFilename returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



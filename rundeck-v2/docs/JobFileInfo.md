# JobFileInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**JobId** | Pointer to **string** |  | [optional] 
**ExecId** | Pointer to **int64** |  | [optional] 
**OptionName** | Pointer to **string** |  | [optional] 
**FileName** | Pointer to **string** |  | [optional] 
**Sha** | Pointer to **string** |  | [optional] 
**Size** | Pointer to **int64** |  | [optional] 
**DateCreated** | Pointer to **string** |  | [optional] 
**ExpirationDate** | Pointer to **string** |  | [optional] 
**User** | Pointer to **string** |  | [optional] 
**FileState** | Pointer to **string** |  | [optional] 
**ServerNodeUUID** | Pointer to **string** |  | [optional] 

## Methods

### NewJobFileInfo

`func NewJobFileInfo() *JobFileInfo`

NewJobFileInfo instantiates a new JobFileInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobFileInfoWithDefaults

`func NewJobFileInfoWithDefaults() *JobFileInfo`

NewJobFileInfoWithDefaults instantiates a new JobFileInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *JobFileInfo) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *JobFileInfo) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *JobFileInfo) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *JobFileInfo) HasId() bool`

HasId returns a boolean if a field has been set.

### GetJobId

`func (o *JobFileInfo) GetJobId() string`

GetJobId returns the JobId field if non-nil, zero value otherwise.

### GetJobIdOk

`func (o *JobFileInfo) GetJobIdOk() (*string, bool)`

GetJobIdOk returns a tuple with the JobId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobId

`func (o *JobFileInfo) SetJobId(v string)`

SetJobId sets JobId field to given value.

### HasJobId

`func (o *JobFileInfo) HasJobId() bool`

HasJobId returns a boolean if a field has been set.

### GetExecId

`func (o *JobFileInfo) GetExecId() int64`

GetExecId returns the ExecId field if non-nil, zero value otherwise.

### GetExecIdOk

`func (o *JobFileInfo) GetExecIdOk() (*int64, bool)`

GetExecIdOk returns a tuple with the ExecId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecId

`func (o *JobFileInfo) SetExecId(v int64)`

SetExecId sets ExecId field to given value.

### HasExecId

`func (o *JobFileInfo) HasExecId() bool`

HasExecId returns a boolean if a field has been set.

### GetOptionName

`func (o *JobFileInfo) GetOptionName() string`

GetOptionName returns the OptionName field if non-nil, zero value otherwise.

### GetOptionNameOk

`func (o *JobFileInfo) GetOptionNameOk() (*string, bool)`

GetOptionNameOk returns a tuple with the OptionName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptionName

`func (o *JobFileInfo) SetOptionName(v string)`

SetOptionName sets OptionName field to given value.

### HasOptionName

`func (o *JobFileInfo) HasOptionName() bool`

HasOptionName returns a boolean if a field has been set.

### GetFileName

`func (o *JobFileInfo) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *JobFileInfo) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *JobFileInfo) SetFileName(v string)`

SetFileName sets FileName field to given value.

### HasFileName

`func (o *JobFileInfo) HasFileName() bool`

HasFileName returns a boolean if a field has been set.

### GetSha

`func (o *JobFileInfo) GetSha() string`

GetSha returns the Sha field if non-nil, zero value otherwise.

### GetShaOk

`func (o *JobFileInfo) GetShaOk() (*string, bool)`

GetShaOk returns a tuple with the Sha field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSha

`func (o *JobFileInfo) SetSha(v string)`

SetSha sets Sha field to given value.

### HasSha

`func (o *JobFileInfo) HasSha() bool`

HasSha returns a boolean if a field has been set.

### GetSize

`func (o *JobFileInfo) GetSize() int64`

GetSize returns the Size field if non-nil, zero value otherwise.

### GetSizeOk

`func (o *JobFileInfo) GetSizeOk() (*int64, bool)`

GetSizeOk returns a tuple with the Size field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSize

`func (o *JobFileInfo) SetSize(v int64)`

SetSize sets Size field to given value.

### HasSize

`func (o *JobFileInfo) HasSize() bool`

HasSize returns a boolean if a field has been set.

### GetDateCreated

`func (o *JobFileInfo) GetDateCreated() string`

GetDateCreated returns the DateCreated field if non-nil, zero value otherwise.

### GetDateCreatedOk

`func (o *JobFileInfo) GetDateCreatedOk() (*string, bool)`

GetDateCreatedOk returns a tuple with the DateCreated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateCreated

`func (o *JobFileInfo) SetDateCreated(v string)`

SetDateCreated sets DateCreated field to given value.

### HasDateCreated

`func (o *JobFileInfo) HasDateCreated() bool`

HasDateCreated returns a boolean if a field has been set.

### GetExpirationDate

`func (o *JobFileInfo) GetExpirationDate() string`

GetExpirationDate returns the ExpirationDate field if non-nil, zero value otherwise.

### GetExpirationDateOk

`func (o *JobFileInfo) GetExpirationDateOk() (*string, bool)`

GetExpirationDateOk returns a tuple with the ExpirationDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpirationDate

`func (o *JobFileInfo) SetExpirationDate(v string)`

SetExpirationDate sets ExpirationDate field to given value.

### HasExpirationDate

`func (o *JobFileInfo) HasExpirationDate() bool`

HasExpirationDate returns a boolean if a field has been set.

### GetUser

`func (o *JobFileInfo) GetUser() string`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *JobFileInfo) GetUserOk() (*string, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *JobFileInfo) SetUser(v string)`

SetUser sets User field to given value.

### HasUser

`func (o *JobFileInfo) HasUser() bool`

HasUser returns a boolean if a field has been set.

### GetFileState

`func (o *JobFileInfo) GetFileState() string`

GetFileState returns the FileState field if non-nil, zero value otherwise.

### GetFileStateOk

`func (o *JobFileInfo) GetFileStateOk() (*string, bool)`

GetFileStateOk returns a tuple with the FileState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileState

`func (o *JobFileInfo) SetFileState(v string)`

SetFileState sets FileState field to given value.

### HasFileState

`func (o *JobFileInfo) HasFileState() bool`

HasFileState returns a boolean if a field has been set.

### GetServerNodeUUID

`func (o *JobFileInfo) GetServerNodeUUID() string`

GetServerNodeUUID returns the ServerNodeUUID field if non-nil, zero value otherwise.

### GetServerNodeUUIDOk

`func (o *JobFileInfo) GetServerNodeUUIDOk() (*string, bool)`

GetServerNodeUUIDOk returns a tuple with the ServerNodeUUID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServerNodeUUID

`func (o *JobFileInfo) SetServerNodeUUID(v string)`

SetServerNodeUUID sets ServerNodeUUID field to given value.

### HasServerNodeUUID

`func (o *JobFileInfo) HasServerNodeUUID() bool`

HasServerNodeUUID returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ScmCommit

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CommitId** | Pointer to **string** |  | [optional] 
**Message** | Pointer to **string** |  | [optional] 
**Author** | Pointer to **string** |  | [optional] 
**Date** | Pointer to **time.Time** |  | [optional] 
**Info** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewScmCommit

`func NewScmCommit() *ScmCommit`

NewScmCommit instantiates a new ScmCommit object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScmCommitWithDefaults

`func NewScmCommitWithDefaults() *ScmCommit`

NewScmCommitWithDefaults instantiates a new ScmCommit object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCommitId

`func (o *ScmCommit) GetCommitId() string`

GetCommitId returns the CommitId field if non-nil, zero value otherwise.

### GetCommitIdOk

`func (o *ScmCommit) GetCommitIdOk() (*string, bool)`

GetCommitIdOk returns a tuple with the CommitId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommitId

`func (o *ScmCommit) SetCommitId(v string)`

SetCommitId sets CommitId field to given value.

### HasCommitId

`func (o *ScmCommit) HasCommitId() bool`

HasCommitId returns a boolean if a field has been set.

### GetMessage

`func (o *ScmCommit) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ScmCommit) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ScmCommit) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *ScmCommit) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetAuthor

`func (o *ScmCommit) GetAuthor() string`

GetAuthor returns the Author field if non-nil, zero value otherwise.

### GetAuthorOk

`func (o *ScmCommit) GetAuthorOk() (*string, bool)`

GetAuthorOk returns a tuple with the Author field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthor

`func (o *ScmCommit) SetAuthor(v string)`

SetAuthor sets Author field to given value.

### HasAuthor

`func (o *ScmCommit) HasAuthor() bool`

HasAuthor returns a boolean if a field has been set.

### GetDate

`func (o *ScmCommit) GetDate() time.Time`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *ScmCommit) GetDateOk() (*time.Time, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *ScmCommit) SetDate(v time.Time)`

SetDate sets Date field to given value.

### HasDate

`func (o *ScmCommit) HasDate() bool`

HasDate returns a boolean if a field has been set.

### GetInfo

`func (o *ScmCommit) GetInfo() map[string]interface{}`

GetInfo returns the Info field if non-nil, zero value otherwise.

### GetInfoOk

`func (o *ScmCommit) GetInfoOk() (*map[string]interface{}, bool)`

GetInfoOk returns a tuple with the Info field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInfo

`func (o *ScmCommit) SetInfo(v map[string]interface{})`

SetInfo sets Info field to given value.

### HasInfo

`func (o *ScmCommit) HasInfo() bool`

HasInfo returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CreateUserRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Username** | **string** | Username for the new user | 
**Pwd** | **string** | Password for the new user. Note: field is named &#39;pwd&#39; not &#39;password&#39; for consistency with internal authentication system | 
**Roles** | **[]string** | List of role names to assign to the user | 
**Firstname** | Pointer to **string** | User&#39;s first name (optional) | [optional] 
**Lastname** | Pointer to **string** | User&#39;s last name (optional) | [optional] 
**Email** | Pointer to **string** | User&#39;s email address (optional) | [optional] 
**Notes** | Pointer to **string** | Additional notes about the user (optional) | [optional] 

## Methods

### NewCreateUserRequest

`func NewCreateUserRequest(username string, pwd string, roles []string, ) *CreateUserRequest`

NewCreateUserRequest instantiates a new CreateUserRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateUserRequestWithDefaults

`func NewCreateUserRequestWithDefaults() *CreateUserRequest`

NewCreateUserRequestWithDefaults instantiates a new CreateUserRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUsername

`func (o *CreateUserRequest) GetUsername() string`

GetUsername returns the Username field if non-nil, zero value otherwise.

### GetUsernameOk

`func (o *CreateUserRequest) GetUsernameOk() (*string, bool)`

GetUsernameOk returns a tuple with the Username field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsername

`func (o *CreateUserRequest) SetUsername(v string)`

SetUsername sets Username field to given value.


### GetPwd

`func (o *CreateUserRequest) GetPwd() string`

GetPwd returns the Pwd field if non-nil, zero value otherwise.

### GetPwdOk

`func (o *CreateUserRequest) GetPwdOk() (*string, bool)`

GetPwdOk returns a tuple with the Pwd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPwd

`func (o *CreateUserRequest) SetPwd(v string)`

SetPwd sets Pwd field to given value.


### GetRoles

`func (o *CreateUserRequest) GetRoles() []string`

GetRoles returns the Roles field if non-nil, zero value otherwise.

### GetRolesOk

`func (o *CreateUserRequest) GetRolesOk() (*[]string, bool)`

GetRolesOk returns a tuple with the Roles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoles

`func (o *CreateUserRequest) SetRoles(v []string)`

SetRoles sets Roles field to given value.


### GetFirstname

`func (o *CreateUserRequest) GetFirstname() string`

GetFirstname returns the Firstname field if non-nil, zero value otherwise.

### GetFirstnameOk

`func (o *CreateUserRequest) GetFirstnameOk() (*string, bool)`

GetFirstnameOk returns a tuple with the Firstname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstname

`func (o *CreateUserRequest) SetFirstname(v string)`

SetFirstname sets Firstname field to given value.

### HasFirstname

`func (o *CreateUserRequest) HasFirstname() bool`

HasFirstname returns a boolean if a field has been set.

### GetLastname

`func (o *CreateUserRequest) GetLastname() string`

GetLastname returns the Lastname field if non-nil, zero value otherwise.

### GetLastnameOk

`func (o *CreateUserRequest) GetLastnameOk() (*string, bool)`

GetLastnameOk returns a tuple with the Lastname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastname

`func (o *CreateUserRequest) SetLastname(v string)`

SetLastname sets Lastname field to given value.

### HasLastname

`func (o *CreateUserRequest) HasLastname() bool`

HasLastname returns a boolean if a field has been set.

### GetEmail

`func (o *CreateUserRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *CreateUserRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *CreateUserRequest) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *CreateUserRequest) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetNotes

`func (o *CreateUserRequest) GetNotes() string`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *CreateUserRequest) GetNotesOk() (*string, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *CreateUserRequest) SetNotes(v string)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *CreateUserRequest) HasNotes() bool`

HasNotes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CreateToken

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Roles** | Pointer to **[]string** | since: v19 | [optional] 
**User** | Pointer to **string** |  | [optional] 
**Duration** | Pointer to **string** | since: v19 | [optional] 
**Name** | Pointer to **string** | since: v19 | [optional] 

## Methods

### NewCreateToken

`func NewCreateToken() *CreateToken`

NewCreateToken instantiates a new CreateToken object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateTokenWithDefaults

`func NewCreateTokenWithDefaults() *CreateToken`

NewCreateTokenWithDefaults instantiates a new CreateToken object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRoles

`func (o *CreateToken) GetRoles() []string`

GetRoles returns the Roles field if non-nil, zero value otherwise.

### GetRolesOk

`func (o *CreateToken) GetRolesOk() (*[]string, bool)`

GetRolesOk returns a tuple with the Roles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoles

`func (o *CreateToken) SetRoles(v []string)`

SetRoles sets Roles field to given value.

### HasRoles

`func (o *CreateToken) HasRoles() bool`

HasRoles returns a boolean if a field has been set.

### GetUser

`func (o *CreateToken) GetUser() string`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *CreateToken) GetUserOk() (*string, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *CreateToken) SetUser(v string)`

SetUser sets User field to given value.

### HasUser

`func (o *CreateToken) HasUser() bool`

HasUser returns a boolean if a field has been set.

### GetDuration

`func (o *CreateToken) GetDuration() string`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *CreateToken) GetDurationOk() (*string, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *CreateToken) SetDuration(v string)`

SetDuration sets Duration field to given value.

### HasDuration

`func (o *CreateToken) HasDuration() bool`

HasDuration returns a boolean if a field has been set.

### GetName

`func (o *CreateToken) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateToken) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateToken) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CreateToken) HasName() bool`

HasName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



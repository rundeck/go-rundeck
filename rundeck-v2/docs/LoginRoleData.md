# LoginRoleData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** |  | [optional] 
**Authority** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 

## Methods

### NewLoginRoleData

`func NewLoginRoleData() *LoginRoleData`

NewLoginRoleData instantiates a new LoginRoleData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLoginRoleDataWithDefaults

`func NewLoginRoleDataWithDefaults() *LoginRoleData`

NewLoginRoleDataWithDefaults instantiates a new LoginRoleData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *LoginRoleData) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *LoginRoleData) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *LoginRoleData) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *LoginRoleData) HasId() bool`

HasId returns a boolean if a field has been set.

### GetAuthority

`func (o *LoginRoleData) GetAuthority() string`

GetAuthority returns the Authority field if non-nil, zero value otherwise.

### GetAuthorityOk

`func (o *LoginRoleData) GetAuthorityOk() (*string, bool)`

GetAuthorityOk returns a tuple with the Authority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthority

`func (o *LoginRoleData) SetAuthority(v string)`

SetAuthority sets Authority field to given value.

### HasAuthority

`func (o *LoginRoleData) HasAuthority() bool`

HasAuthority returns a boolean if a field has been set.

### GetDescription

`func (o *LoginRoleData) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *LoginRoleData) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *LoginRoleData) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *LoginRoleData) HasDescription() bool`

HasDescription returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



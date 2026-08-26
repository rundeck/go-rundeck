# AuthorizationsResponseResource

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Kind** | **string** | Resource kind | 
**Type** | **string** | Resource Type | 
**Specifier** | Pointer to **string** | Type Specifier | [optional] 

## Methods

### NewAuthorizationsResponseResource

`func NewAuthorizationsResponseResource(kind string, type_ string, ) *AuthorizationsResponseResource`

NewAuthorizationsResponseResource instantiates a new AuthorizationsResponseResource object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthorizationsResponseResourceWithDefaults

`func NewAuthorizationsResponseResourceWithDefaults() *AuthorizationsResponseResource`

NewAuthorizationsResponseResourceWithDefaults instantiates a new AuthorizationsResponseResource object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKind

`func (o *AuthorizationsResponseResource) GetKind() string`

GetKind returns the Kind field if non-nil, zero value otherwise.

### GetKindOk

`func (o *AuthorizationsResponseResource) GetKindOk() (*string, bool)`

GetKindOk returns a tuple with the Kind field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKind

`func (o *AuthorizationsResponseResource) SetKind(v string)`

SetKind sets Kind field to given value.


### GetType

`func (o *AuthorizationsResponseResource) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *AuthorizationsResponseResource) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *AuthorizationsResponseResource) SetType(v string)`

SetType sets Type field to given value.


### GetSpecifier

`func (o *AuthorizationsResponseResource) GetSpecifier() string`

GetSpecifier returns the Specifier field if non-nil, zero value otherwise.

### GetSpecifierOk

`func (o *AuthorizationsResponseResource) GetSpecifierOk() (*string, bool)`

GetSpecifierOk returns a tuple with the Specifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecifier

`func (o *AuthorizationsResponseResource) SetSpecifier(v string)`

SetSpecifier sets Specifier field to given value.

### HasSpecifier

`func (o *AuthorizationsResponseResource) HasSpecifier() bool`

HasSpecifier returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



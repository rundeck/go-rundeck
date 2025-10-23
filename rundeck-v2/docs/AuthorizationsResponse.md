# AuthorizationsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AuthorizationContext** | **map[string]interface{}** |  | 
**Resource** | **map[string]interface{}** |  | 
**ActionAuthorizations** | [**[]ActionAuthorization**](ActionAuthorization.md) | Action authorization | 

## Methods

### NewAuthorizationsResponse

`func NewAuthorizationsResponse(authorizationContext map[string]interface{}, resource map[string]interface{}, actionAuthorizations []ActionAuthorization, ) *AuthorizationsResponse`

NewAuthorizationsResponse instantiates a new AuthorizationsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthorizationsResponseWithDefaults

`func NewAuthorizationsResponseWithDefaults() *AuthorizationsResponse`

NewAuthorizationsResponseWithDefaults instantiates a new AuthorizationsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAuthorizationContext

`func (o *AuthorizationsResponse) GetAuthorizationContext() map[string]interface{}`

GetAuthorizationContext returns the AuthorizationContext field if non-nil, zero value otherwise.

### GetAuthorizationContextOk

`func (o *AuthorizationsResponse) GetAuthorizationContextOk() (*map[string]interface{}, bool)`

GetAuthorizationContextOk returns a tuple with the AuthorizationContext field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthorizationContext

`func (o *AuthorizationsResponse) SetAuthorizationContext(v map[string]interface{})`

SetAuthorizationContext sets AuthorizationContext field to given value.


### GetResource

`func (o *AuthorizationsResponse) GetResource() map[string]interface{}`

GetResource returns the Resource field if non-nil, zero value otherwise.

### GetResourceOk

`func (o *AuthorizationsResponse) GetResourceOk() (*map[string]interface{}, bool)`

GetResourceOk returns a tuple with the Resource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResource

`func (o *AuthorizationsResponse) SetResource(v map[string]interface{})`

SetResource sets Resource field to given value.


### GetActionAuthorizations

`func (o *AuthorizationsResponse) GetActionAuthorizations() []ActionAuthorization`

GetActionAuthorizations returns the ActionAuthorizations field if non-nil, zero value otherwise.

### GetActionAuthorizationsOk

`func (o *AuthorizationsResponse) GetActionAuthorizationsOk() (*[]ActionAuthorization, bool)`

GetActionAuthorizationsOk returns a tuple with the ActionAuthorizations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionAuthorizations

`func (o *AuthorizationsResponse) SetActionAuthorizations(v []ActionAuthorization)`

SetActionAuthorizations sets ActionAuthorizations field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



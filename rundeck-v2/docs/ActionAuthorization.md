# ActionAuthorization

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ActionName** | **string** | Action name | 
**IsAuthorized** | **bool** | Action authorization flag | 

## Methods

### NewActionAuthorization

`func NewActionAuthorization(actionName string, isAuthorized bool, ) *ActionAuthorization`

NewActionAuthorization instantiates a new ActionAuthorization object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewActionAuthorizationWithDefaults

`func NewActionAuthorizationWithDefaults() *ActionAuthorization`

NewActionAuthorizationWithDefaults instantiates a new ActionAuthorization object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActionName

`func (o *ActionAuthorization) GetActionName() string`

GetActionName returns the ActionName field if non-nil, zero value otherwise.

### GetActionNameOk

`func (o *ActionAuthorization) GetActionNameOk() (*string, bool)`

GetActionNameOk returns a tuple with the ActionName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionName

`func (o *ActionAuthorization) SetActionName(v string)`

SetActionName sets ActionName field to given value.


### GetIsAuthorized

`func (o *ActionAuthorization) GetIsAuthorized() bool`

GetIsAuthorized returns the IsAuthorized field if non-nil, zero value otherwise.

### GetIsAuthorizedOk

`func (o *ActionAuthorization) GetIsAuthorizedOk() (*bool, bool)`

GetIsAuthorizedOk returns a tuple with the IsAuthorized field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsAuthorized

`func (o *ActionAuthorization) SetIsAuthorized(v bool)`

SetIsAuthorized sets IsAuthorized field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



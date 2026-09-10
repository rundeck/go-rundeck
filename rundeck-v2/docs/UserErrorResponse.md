# UserErrorResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Err** | Pointer to **string** | Error message describing what went wrong | [optional] 

## Methods

### NewUserErrorResponse

`func NewUserErrorResponse() *UserErrorResponse`

NewUserErrorResponse instantiates a new UserErrorResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserErrorResponseWithDefaults

`func NewUserErrorResponseWithDefaults() *UserErrorResponse`

NewUserErrorResponseWithDefaults instantiates a new UserErrorResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetErr

`func (o *UserErrorResponse) GetErr() string`

GetErr returns the Err field if non-nil, zero value otherwise.

### GetErrOk

`func (o *UserErrorResponse) GetErrOk() (*string, bool)`

GetErrOk returns a tuple with the Err field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErr

`func (o *UserErrorResponse) SetErr(v string)`

SetErr sets Err field to given value.

### HasErr

`func (o *UserErrorResponse) HasErr() bool`

HasErr returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



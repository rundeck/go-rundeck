# Source

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Project** | Pointer to **string** |  | [optional] 
**Index** | Pointer to **int32** |  | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**Errors** | Pointer to **string** |  | [optional] 
**Resources** | Pointer to [**Resources**](Resources.md) |  | [optional] 

## Methods

### NewSource

`func NewSource() *Source`

NewSource instantiates a new Source object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSourceWithDefaults

`func NewSourceWithDefaults() *Source`

NewSourceWithDefaults instantiates a new Source object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProject

`func (o *Source) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *Source) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *Source) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *Source) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetIndex

`func (o *Source) GetIndex() int32`

GetIndex returns the Index field if non-nil, zero value otherwise.

### GetIndexOk

`func (o *Source) GetIndexOk() (*int32, bool)`

GetIndexOk returns a tuple with the Index field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndex

`func (o *Source) SetIndex(v int32)`

SetIndex sets Index field to given value.

### HasIndex

`func (o *Source) HasIndex() bool`

HasIndex returns a boolean if a field has been set.

### GetType

`func (o *Source) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Source) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Source) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *Source) HasType() bool`

HasType returns a boolean if a field has been set.

### GetErrors

`func (o *Source) GetErrors() string`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *Source) GetErrorsOk() (*string, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *Source) SetErrors(v string)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *Source) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetResources

`func (o *Source) GetResources() Resources`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *Source) GetResourcesOk() (*Resources, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *Source) SetResources(v Resources)`

SetResources sets Resources field to given value.

### HasResources

`func (o *Source) HasResources() bool`

HasResources returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ProjectModeLaterRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** | Mode to change, one of &#x60;executions&#x60; or &#x60;schedule&#x60; | [optional] 
**Value** | Pointer to **string** | Time duration expression.  A series of: an integer followed by a unit.  Units: * &#x60;s&#x60; - seconds (default) * &#x60;m&#x60; - minutes * &#x60;h&#x60; - hours * &#x60;d&#x60; - days * &#x60;w&#x60; - weeks * &#x60;y&#x60; - years.  Examples: &#x60;1d12h&#x60;, &#x60;3600&#x60; (defaults to seconds), &#x60;15m30s&#x60;.  | [optional] 

## Methods

### NewProjectModeLaterRequest

`func NewProjectModeLaterRequest() *ProjectModeLaterRequest`

NewProjectModeLaterRequest instantiates a new ProjectModeLaterRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProjectModeLaterRequestWithDefaults

`func NewProjectModeLaterRequestWithDefaults() *ProjectModeLaterRequest`

NewProjectModeLaterRequestWithDefaults instantiates a new ProjectModeLaterRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *ProjectModeLaterRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ProjectModeLaterRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ProjectModeLaterRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ProjectModeLaterRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetValue

`func (o *ProjectModeLaterRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ProjectModeLaterRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ProjectModeLaterRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *ProjectModeLaterRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



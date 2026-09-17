# RouterEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Meta** | Pointer to [**RouterEventMetadata**](RouterEventMetadata.md) |  | [optional] 
**Event** | Pointer to **map[string]map[string]interface{}** |  | [optional] 

## Methods

### NewRouterEvent

`func NewRouterEvent() *RouterEvent`

NewRouterEvent instantiates a new RouterEvent object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRouterEventWithDefaults

`func NewRouterEventWithDefaults() *RouterEvent`

NewRouterEventWithDefaults instantiates a new RouterEvent object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMeta

`func (o *RouterEvent) GetMeta() RouterEventMetadata`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *RouterEvent) GetMetaOk() (*RouterEventMetadata, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *RouterEvent) SetMeta(v RouterEventMetadata)`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *RouterEvent) HasMeta() bool`

HasMeta returns a boolean if a field has been set.

### GetEvent

`func (o *RouterEvent) GetEvent() map[string]map[string]interface{}`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *RouterEvent) GetEventOk() (*map[string]map[string]interface{}, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *RouterEvent) SetEvent(v map[string]map[string]interface{})`

SetEvent sets Event field to given value.

### HasEvent

`func (o *RouterEvent) HasEvent() bool`

HasEvent returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



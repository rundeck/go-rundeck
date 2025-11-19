# ApiPluginListProvider

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Service** | Pointer to **string** |  | [optional] 
**ArtifactName** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Id** | Pointer to **string** |  | [optional] 
**Builtin** | Pointer to **bool** |  | [optional] 
**PluginVersion** | Pointer to **string** |  | [optional] 
**Title** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Author** | Pointer to **string** |  | [optional] 
**IconUrl** | Pointer to **string** | URL to icon file for the plugin if present. Since: v40 | [optional] 
**ProviderMetadata** | Pointer to **map[string]string** | Map of metadata about the plugin if present. Since: v40 | [optional] 
**IsHighlighted** | Pointer to **bool** | Indication of whether the plugin is marked as highlighted. Since: v51 | [optional] 
**HighlightedOrder** | Pointer to **int32** | Order of the highlighted plugin. Since: v51 | [optional] 

## Methods

### NewApiPluginListProvider

`func NewApiPluginListProvider() *ApiPluginListProvider`

NewApiPluginListProvider instantiates a new ApiPluginListProvider object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiPluginListProviderWithDefaults

`func NewApiPluginListProviderWithDefaults() *ApiPluginListProvider`

NewApiPluginListProviderWithDefaults instantiates a new ApiPluginListProvider object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetService

`func (o *ApiPluginListProvider) GetService() string`

GetService returns the Service field if non-nil, zero value otherwise.

### GetServiceOk

`func (o *ApiPluginListProvider) GetServiceOk() (*string, bool)`

GetServiceOk returns a tuple with the Service field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetService

`func (o *ApiPluginListProvider) SetService(v string)`

SetService sets Service field to given value.

### HasService

`func (o *ApiPluginListProvider) HasService() bool`

HasService returns a boolean if a field has been set.

### GetArtifactName

`func (o *ApiPluginListProvider) GetArtifactName() string`

GetArtifactName returns the ArtifactName field if non-nil, zero value otherwise.

### GetArtifactNameOk

`func (o *ApiPluginListProvider) GetArtifactNameOk() (*string, bool)`

GetArtifactNameOk returns a tuple with the ArtifactName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArtifactName

`func (o *ApiPluginListProvider) SetArtifactName(v string)`

SetArtifactName sets ArtifactName field to given value.

### HasArtifactName

`func (o *ApiPluginListProvider) HasArtifactName() bool`

HasArtifactName returns a boolean if a field has been set.

### GetName

`func (o *ApiPluginListProvider) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApiPluginListProvider) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApiPluginListProvider) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ApiPluginListProvider) HasName() bool`

HasName returns a boolean if a field has been set.

### GetId

`func (o *ApiPluginListProvider) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApiPluginListProvider) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApiPluginListProvider) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *ApiPluginListProvider) HasId() bool`

HasId returns a boolean if a field has been set.

### GetBuiltin

`func (o *ApiPluginListProvider) GetBuiltin() bool`

GetBuiltin returns the Builtin field if non-nil, zero value otherwise.

### GetBuiltinOk

`func (o *ApiPluginListProvider) GetBuiltinOk() (*bool, bool)`

GetBuiltinOk returns a tuple with the Builtin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuiltin

`func (o *ApiPluginListProvider) SetBuiltin(v bool)`

SetBuiltin sets Builtin field to given value.

### HasBuiltin

`func (o *ApiPluginListProvider) HasBuiltin() bool`

HasBuiltin returns a boolean if a field has been set.

### GetPluginVersion

`func (o *ApiPluginListProvider) GetPluginVersion() string`

GetPluginVersion returns the PluginVersion field if non-nil, zero value otherwise.

### GetPluginVersionOk

`func (o *ApiPluginListProvider) GetPluginVersionOk() (*string, bool)`

GetPluginVersionOk returns a tuple with the PluginVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPluginVersion

`func (o *ApiPluginListProvider) SetPluginVersion(v string)`

SetPluginVersion sets PluginVersion field to given value.

### HasPluginVersion

`func (o *ApiPluginListProvider) HasPluginVersion() bool`

HasPluginVersion returns a boolean if a field has been set.

### GetTitle

`func (o *ApiPluginListProvider) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ApiPluginListProvider) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ApiPluginListProvider) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ApiPluginListProvider) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetDescription

`func (o *ApiPluginListProvider) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ApiPluginListProvider) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ApiPluginListProvider) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ApiPluginListProvider) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetAuthor

`func (o *ApiPluginListProvider) GetAuthor() string`

GetAuthor returns the Author field if non-nil, zero value otherwise.

### GetAuthorOk

`func (o *ApiPluginListProvider) GetAuthorOk() (*string, bool)`

GetAuthorOk returns a tuple with the Author field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthor

`func (o *ApiPluginListProvider) SetAuthor(v string)`

SetAuthor sets Author field to given value.

### HasAuthor

`func (o *ApiPluginListProvider) HasAuthor() bool`

HasAuthor returns a boolean if a field has been set.

### GetIconUrl

`func (o *ApiPluginListProvider) GetIconUrl() string`

GetIconUrl returns the IconUrl field if non-nil, zero value otherwise.

### GetIconUrlOk

`func (o *ApiPluginListProvider) GetIconUrlOk() (*string, bool)`

GetIconUrlOk returns a tuple with the IconUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIconUrl

`func (o *ApiPluginListProvider) SetIconUrl(v string)`

SetIconUrl sets IconUrl field to given value.

### HasIconUrl

`func (o *ApiPluginListProvider) HasIconUrl() bool`

HasIconUrl returns a boolean if a field has been set.

### GetProviderMetadata

`func (o *ApiPluginListProvider) GetProviderMetadata() map[string]string`

GetProviderMetadata returns the ProviderMetadata field if non-nil, zero value otherwise.

### GetProviderMetadataOk

`func (o *ApiPluginListProvider) GetProviderMetadataOk() (*map[string]string, bool)`

GetProviderMetadataOk returns a tuple with the ProviderMetadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProviderMetadata

`func (o *ApiPluginListProvider) SetProviderMetadata(v map[string]string)`

SetProviderMetadata sets ProviderMetadata field to given value.

### HasProviderMetadata

`func (o *ApiPluginListProvider) HasProviderMetadata() bool`

HasProviderMetadata returns a boolean if a field has been set.

### GetIsHighlighted

`func (o *ApiPluginListProvider) GetIsHighlighted() bool`

GetIsHighlighted returns the IsHighlighted field if non-nil, zero value otherwise.

### GetIsHighlightedOk

`func (o *ApiPluginListProvider) GetIsHighlightedOk() (*bool, bool)`

GetIsHighlightedOk returns a tuple with the IsHighlighted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsHighlighted

`func (o *ApiPluginListProvider) SetIsHighlighted(v bool)`

SetIsHighlighted sets IsHighlighted field to given value.

### HasIsHighlighted

`func (o *ApiPluginListProvider) HasIsHighlighted() bool`

HasIsHighlighted returns a boolean if a field has been set.

### GetHighlightedOrder

`func (o *ApiPluginListProvider) GetHighlightedOrder() int32`

GetHighlightedOrder returns the HighlightedOrder field if non-nil, zero value otherwise.

### GetHighlightedOrderOk

`func (o *ApiPluginListProvider) GetHighlightedOrderOk() (*int32, bool)`

GetHighlightedOrderOk returns a tuple with the HighlightedOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHighlightedOrder

`func (o *ApiPluginListProvider) SetHighlightedOrder(v int32)`

SetHighlightedOrder sets HighlightedOrder field to given value.

### HasHighlightedOrder

`func (o *ApiPluginListProvider) HasHighlightedOrder() bool`

HasHighlightedOrder returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ApiRunAdhocRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Project** | Pointer to **string** |  | [optional] 
**Exec** | Pointer to **string** |  | [optional] 
**Script** | Pointer to **string** |  | [optional] 
**ScriptInterpreter** | Pointer to **string** |  | [optional] 
**ArgString** | Pointer to **string** |  | [optional] 
**InterpreterArgsQuoted** | Pointer to **bool** |  | [optional] 
**Url** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Filter** | Pointer to **string** |  | [optional] 
**AsUser** | Pointer to **string** |  | [optional] 
**FileExtension** | Pointer to **string** |  | [optional] 
**NodeKeepgoing** | Pointer to **bool** |  | [optional] 
**NodeThreadcount** | Pointer to **int32** |  | [optional] 
**Meta** | Pointer to **map[string]string** |  | [optional] 

## Methods

### NewApiRunAdhocRequest

`func NewApiRunAdhocRequest() *ApiRunAdhocRequest`

NewApiRunAdhocRequest instantiates a new ApiRunAdhocRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiRunAdhocRequestWithDefaults

`func NewApiRunAdhocRequestWithDefaults() *ApiRunAdhocRequest`

NewApiRunAdhocRequestWithDefaults instantiates a new ApiRunAdhocRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProject

`func (o *ApiRunAdhocRequest) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *ApiRunAdhocRequest) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *ApiRunAdhocRequest) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *ApiRunAdhocRequest) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetExec

`func (o *ApiRunAdhocRequest) GetExec() string`

GetExec returns the Exec field if non-nil, zero value otherwise.

### GetExecOk

`func (o *ApiRunAdhocRequest) GetExecOk() (*string, bool)`

GetExecOk returns a tuple with the Exec field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExec

`func (o *ApiRunAdhocRequest) SetExec(v string)`

SetExec sets Exec field to given value.

### HasExec

`func (o *ApiRunAdhocRequest) HasExec() bool`

HasExec returns a boolean if a field has been set.

### GetScript

`func (o *ApiRunAdhocRequest) GetScript() string`

GetScript returns the Script field if non-nil, zero value otherwise.

### GetScriptOk

`func (o *ApiRunAdhocRequest) GetScriptOk() (*string, bool)`

GetScriptOk returns a tuple with the Script field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScript

`func (o *ApiRunAdhocRequest) SetScript(v string)`

SetScript sets Script field to given value.

### HasScript

`func (o *ApiRunAdhocRequest) HasScript() bool`

HasScript returns a boolean if a field has been set.

### GetScriptInterpreter

`func (o *ApiRunAdhocRequest) GetScriptInterpreter() string`

GetScriptInterpreter returns the ScriptInterpreter field if non-nil, zero value otherwise.

### GetScriptInterpreterOk

`func (o *ApiRunAdhocRequest) GetScriptInterpreterOk() (*string, bool)`

GetScriptInterpreterOk returns a tuple with the ScriptInterpreter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScriptInterpreter

`func (o *ApiRunAdhocRequest) SetScriptInterpreter(v string)`

SetScriptInterpreter sets ScriptInterpreter field to given value.

### HasScriptInterpreter

`func (o *ApiRunAdhocRequest) HasScriptInterpreter() bool`

HasScriptInterpreter returns a boolean if a field has been set.

### GetArgString

`func (o *ApiRunAdhocRequest) GetArgString() string`

GetArgString returns the ArgString field if non-nil, zero value otherwise.

### GetArgStringOk

`func (o *ApiRunAdhocRequest) GetArgStringOk() (*string, bool)`

GetArgStringOk returns a tuple with the ArgString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArgString

`func (o *ApiRunAdhocRequest) SetArgString(v string)`

SetArgString sets ArgString field to given value.

### HasArgString

`func (o *ApiRunAdhocRequest) HasArgString() bool`

HasArgString returns a boolean if a field has been set.

### GetInterpreterArgsQuoted

`func (o *ApiRunAdhocRequest) GetInterpreterArgsQuoted() bool`

GetInterpreterArgsQuoted returns the InterpreterArgsQuoted field if non-nil, zero value otherwise.

### GetInterpreterArgsQuotedOk

`func (o *ApiRunAdhocRequest) GetInterpreterArgsQuotedOk() (*bool, bool)`

GetInterpreterArgsQuotedOk returns a tuple with the InterpreterArgsQuoted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInterpreterArgsQuoted

`func (o *ApiRunAdhocRequest) SetInterpreterArgsQuoted(v bool)`

SetInterpreterArgsQuoted sets InterpreterArgsQuoted field to given value.

### HasInterpreterArgsQuoted

`func (o *ApiRunAdhocRequest) HasInterpreterArgsQuoted() bool`

HasInterpreterArgsQuoted returns a boolean if a field has been set.

### GetUrl

`func (o *ApiRunAdhocRequest) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ApiRunAdhocRequest) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ApiRunAdhocRequest) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *ApiRunAdhocRequest) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetDescription

`func (o *ApiRunAdhocRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ApiRunAdhocRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ApiRunAdhocRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ApiRunAdhocRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetFilter

`func (o *ApiRunAdhocRequest) GetFilter() string`

GetFilter returns the Filter field if non-nil, zero value otherwise.

### GetFilterOk

`func (o *ApiRunAdhocRequest) GetFilterOk() (*string, bool)`

GetFilterOk returns a tuple with the Filter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilter

`func (o *ApiRunAdhocRequest) SetFilter(v string)`

SetFilter sets Filter field to given value.

### HasFilter

`func (o *ApiRunAdhocRequest) HasFilter() bool`

HasFilter returns a boolean if a field has been set.

### GetAsUser

`func (o *ApiRunAdhocRequest) GetAsUser() string`

GetAsUser returns the AsUser field if non-nil, zero value otherwise.

### GetAsUserOk

`func (o *ApiRunAdhocRequest) GetAsUserOk() (*string, bool)`

GetAsUserOk returns a tuple with the AsUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsUser

`func (o *ApiRunAdhocRequest) SetAsUser(v string)`

SetAsUser sets AsUser field to given value.

### HasAsUser

`func (o *ApiRunAdhocRequest) HasAsUser() bool`

HasAsUser returns a boolean if a field has been set.

### GetFileExtension

`func (o *ApiRunAdhocRequest) GetFileExtension() string`

GetFileExtension returns the FileExtension field if non-nil, zero value otherwise.

### GetFileExtensionOk

`func (o *ApiRunAdhocRequest) GetFileExtensionOk() (*string, bool)`

GetFileExtensionOk returns a tuple with the FileExtension field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileExtension

`func (o *ApiRunAdhocRequest) SetFileExtension(v string)`

SetFileExtension sets FileExtension field to given value.

### HasFileExtension

`func (o *ApiRunAdhocRequest) HasFileExtension() bool`

HasFileExtension returns a boolean if a field has been set.

### GetNodeKeepgoing

`func (o *ApiRunAdhocRequest) GetNodeKeepgoing() bool`

GetNodeKeepgoing returns the NodeKeepgoing field if non-nil, zero value otherwise.

### GetNodeKeepgoingOk

`func (o *ApiRunAdhocRequest) GetNodeKeepgoingOk() (*bool, bool)`

GetNodeKeepgoingOk returns a tuple with the NodeKeepgoing field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeKeepgoing

`func (o *ApiRunAdhocRequest) SetNodeKeepgoing(v bool)`

SetNodeKeepgoing sets NodeKeepgoing field to given value.

### HasNodeKeepgoing

`func (o *ApiRunAdhocRequest) HasNodeKeepgoing() bool`

HasNodeKeepgoing returns a boolean if a field has been set.

### GetNodeThreadcount

`func (o *ApiRunAdhocRequest) GetNodeThreadcount() int32`

GetNodeThreadcount returns the NodeThreadcount field if non-nil, zero value otherwise.

### GetNodeThreadcountOk

`func (o *ApiRunAdhocRequest) GetNodeThreadcountOk() (*int32, bool)`

GetNodeThreadcountOk returns a tuple with the NodeThreadcount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeThreadcount

`func (o *ApiRunAdhocRequest) SetNodeThreadcount(v int32)`

SetNodeThreadcount sets NodeThreadcount field to given value.

### HasNodeThreadcount

`func (o *ApiRunAdhocRequest) HasNodeThreadcount() bool`

HasNodeThreadcount returns a boolean if a field has been set.

### GetMeta

`func (o *ApiRunAdhocRequest) GetMeta() map[string]string`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *ApiRunAdhocRequest) GetMetaOk() (*map[string]string, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *ApiRunAdhocRequest) SetMeta(v map[string]string)`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *ApiRunAdhocRequest) HasMeta() bool`

HasMeta returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ApiRunScriptv14Request

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RunAdhocRequest** | Pointer to [**ApiRunAdhocRequest**](ApiRunAdhocRequest.md) |  | [optional] 
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

### NewApiRunScriptv14Request

`func NewApiRunScriptv14Request() *ApiRunScriptv14Request`

NewApiRunScriptv14Request instantiates a new ApiRunScriptv14Request object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiRunScriptv14RequestWithDefaults

`func NewApiRunScriptv14RequestWithDefaults() *ApiRunScriptv14Request`

NewApiRunScriptv14RequestWithDefaults instantiates a new ApiRunScriptv14Request object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRunAdhocRequest

`func (o *ApiRunScriptv14Request) GetRunAdhocRequest() ApiRunAdhocRequest`

GetRunAdhocRequest returns the RunAdhocRequest field if non-nil, zero value otherwise.

### GetRunAdhocRequestOk

`func (o *ApiRunScriptv14Request) GetRunAdhocRequestOk() (*ApiRunAdhocRequest, bool)`

GetRunAdhocRequestOk returns a tuple with the RunAdhocRequest field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAdhocRequest

`func (o *ApiRunScriptv14Request) SetRunAdhocRequest(v ApiRunAdhocRequest)`

SetRunAdhocRequest sets RunAdhocRequest field to given value.

### HasRunAdhocRequest

`func (o *ApiRunScriptv14Request) HasRunAdhocRequest() bool`

HasRunAdhocRequest returns a boolean if a field has been set.

### GetProject

`func (o *ApiRunScriptv14Request) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *ApiRunScriptv14Request) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *ApiRunScriptv14Request) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *ApiRunScriptv14Request) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetExec

`func (o *ApiRunScriptv14Request) GetExec() string`

GetExec returns the Exec field if non-nil, zero value otherwise.

### GetExecOk

`func (o *ApiRunScriptv14Request) GetExecOk() (*string, bool)`

GetExecOk returns a tuple with the Exec field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExec

`func (o *ApiRunScriptv14Request) SetExec(v string)`

SetExec sets Exec field to given value.

### HasExec

`func (o *ApiRunScriptv14Request) HasExec() bool`

HasExec returns a boolean if a field has been set.

### GetScript

`func (o *ApiRunScriptv14Request) GetScript() string`

GetScript returns the Script field if non-nil, zero value otherwise.

### GetScriptOk

`func (o *ApiRunScriptv14Request) GetScriptOk() (*string, bool)`

GetScriptOk returns a tuple with the Script field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScript

`func (o *ApiRunScriptv14Request) SetScript(v string)`

SetScript sets Script field to given value.

### HasScript

`func (o *ApiRunScriptv14Request) HasScript() bool`

HasScript returns a boolean if a field has been set.

### GetScriptInterpreter

`func (o *ApiRunScriptv14Request) GetScriptInterpreter() string`

GetScriptInterpreter returns the ScriptInterpreter field if non-nil, zero value otherwise.

### GetScriptInterpreterOk

`func (o *ApiRunScriptv14Request) GetScriptInterpreterOk() (*string, bool)`

GetScriptInterpreterOk returns a tuple with the ScriptInterpreter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScriptInterpreter

`func (o *ApiRunScriptv14Request) SetScriptInterpreter(v string)`

SetScriptInterpreter sets ScriptInterpreter field to given value.

### HasScriptInterpreter

`func (o *ApiRunScriptv14Request) HasScriptInterpreter() bool`

HasScriptInterpreter returns a boolean if a field has been set.

### GetArgString

`func (o *ApiRunScriptv14Request) GetArgString() string`

GetArgString returns the ArgString field if non-nil, zero value otherwise.

### GetArgStringOk

`func (o *ApiRunScriptv14Request) GetArgStringOk() (*string, bool)`

GetArgStringOk returns a tuple with the ArgString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArgString

`func (o *ApiRunScriptv14Request) SetArgString(v string)`

SetArgString sets ArgString field to given value.

### HasArgString

`func (o *ApiRunScriptv14Request) HasArgString() bool`

HasArgString returns a boolean if a field has been set.

### GetInterpreterArgsQuoted

`func (o *ApiRunScriptv14Request) GetInterpreterArgsQuoted() bool`

GetInterpreterArgsQuoted returns the InterpreterArgsQuoted field if non-nil, zero value otherwise.

### GetInterpreterArgsQuotedOk

`func (o *ApiRunScriptv14Request) GetInterpreterArgsQuotedOk() (*bool, bool)`

GetInterpreterArgsQuotedOk returns a tuple with the InterpreterArgsQuoted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInterpreterArgsQuoted

`func (o *ApiRunScriptv14Request) SetInterpreterArgsQuoted(v bool)`

SetInterpreterArgsQuoted sets InterpreterArgsQuoted field to given value.

### HasInterpreterArgsQuoted

`func (o *ApiRunScriptv14Request) HasInterpreterArgsQuoted() bool`

HasInterpreterArgsQuoted returns a boolean if a field has been set.

### GetUrl

`func (o *ApiRunScriptv14Request) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ApiRunScriptv14Request) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ApiRunScriptv14Request) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *ApiRunScriptv14Request) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetDescription

`func (o *ApiRunScriptv14Request) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ApiRunScriptv14Request) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ApiRunScriptv14Request) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ApiRunScriptv14Request) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetFilter

`func (o *ApiRunScriptv14Request) GetFilter() string`

GetFilter returns the Filter field if non-nil, zero value otherwise.

### GetFilterOk

`func (o *ApiRunScriptv14Request) GetFilterOk() (*string, bool)`

GetFilterOk returns a tuple with the Filter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilter

`func (o *ApiRunScriptv14Request) SetFilter(v string)`

SetFilter sets Filter field to given value.

### HasFilter

`func (o *ApiRunScriptv14Request) HasFilter() bool`

HasFilter returns a boolean if a field has been set.

### GetAsUser

`func (o *ApiRunScriptv14Request) GetAsUser() string`

GetAsUser returns the AsUser field if non-nil, zero value otherwise.

### GetAsUserOk

`func (o *ApiRunScriptv14Request) GetAsUserOk() (*string, bool)`

GetAsUserOk returns a tuple with the AsUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsUser

`func (o *ApiRunScriptv14Request) SetAsUser(v string)`

SetAsUser sets AsUser field to given value.

### HasAsUser

`func (o *ApiRunScriptv14Request) HasAsUser() bool`

HasAsUser returns a boolean if a field has been set.

### GetFileExtension

`func (o *ApiRunScriptv14Request) GetFileExtension() string`

GetFileExtension returns the FileExtension field if non-nil, zero value otherwise.

### GetFileExtensionOk

`func (o *ApiRunScriptv14Request) GetFileExtensionOk() (*string, bool)`

GetFileExtensionOk returns a tuple with the FileExtension field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileExtension

`func (o *ApiRunScriptv14Request) SetFileExtension(v string)`

SetFileExtension sets FileExtension field to given value.

### HasFileExtension

`func (o *ApiRunScriptv14Request) HasFileExtension() bool`

HasFileExtension returns a boolean if a field has been set.

### GetNodeKeepgoing

`func (o *ApiRunScriptv14Request) GetNodeKeepgoing() bool`

GetNodeKeepgoing returns the NodeKeepgoing field if non-nil, zero value otherwise.

### GetNodeKeepgoingOk

`func (o *ApiRunScriptv14Request) GetNodeKeepgoingOk() (*bool, bool)`

GetNodeKeepgoingOk returns a tuple with the NodeKeepgoing field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeKeepgoing

`func (o *ApiRunScriptv14Request) SetNodeKeepgoing(v bool)`

SetNodeKeepgoing sets NodeKeepgoing field to given value.

### HasNodeKeepgoing

`func (o *ApiRunScriptv14Request) HasNodeKeepgoing() bool`

HasNodeKeepgoing returns a boolean if a field has been set.

### GetNodeThreadcount

`func (o *ApiRunScriptv14Request) GetNodeThreadcount() int32`

GetNodeThreadcount returns the NodeThreadcount field if non-nil, zero value otherwise.

### GetNodeThreadcountOk

`func (o *ApiRunScriptv14Request) GetNodeThreadcountOk() (*int32, bool)`

GetNodeThreadcountOk returns a tuple with the NodeThreadcount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeThreadcount

`func (o *ApiRunScriptv14Request) SetNodeThreadcount(v int32)`

SetNodeThreadcount sets NodeThreadcount field to given value.

### HasNodeThreadcount

`func (o *ApiRunScriptv14Request) HasNodeThreadcount() bool`

HasNodeThreadcount returns a boolean if a field has been set.

### GetMeta

`func (o *ApiRunScriptv14Request) GetMeta() map[string]string`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *ApiRunScriptv14Request) GetMetaOk() (*map[string]string, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *ApiRunScriptv14Request) SetMeta(v map[string]string)`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *ApiRunScriptv14Request) HasMeta() bool`

HasMeta returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



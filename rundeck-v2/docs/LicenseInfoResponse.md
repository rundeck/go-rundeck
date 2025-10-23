# LicenseInfoResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Authorized** | Pointer to **bool** |  | [optional] 
**Company** | Pointer to **string** |  | [optional] 
**ContactEmail** | Pointer to **string** |  | [optional] 
**Application** | Pointer to **string** |  | [optional] 
**Editions** | Pointer to **[]string** |  | [optional] 
**ApplicationVersion** | Pointer to **[]string** |  | [optional] 
**GracePeriod** | Pointer to **int32** | Expiry Grace Period in Days | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**LicenseId** | Pointer to **string** |  | [optional] 
**LicenseVersion** | Pointer to **string** |  | [optional] 
**IssueDate** | Pointer to **string** | Issue Date | [optional] 
**ValidSince** | Pointer to **string** | Valid Since Date | [optional] 
**ValidUntil** | Pointer to **string** | Valid Until Date | [optional] 
**GraceUntil** | Pointer to **string** | Grace Period until Date | [optional] 
**State** | Pointer to **string** |  | [optional] 
**Perpetual** | Pointer to **bool** |  | [optional] 
**Active** | Pointer to **bool** |  | [optional] 
**Remaining** | Pointer to **int32** | License Remaining Period in Days | [optional] 
**ShouldWarn** | Pointer to **bool** |  | [optional] 
**BaseUrl** | Pointer to **string** |  | [optional] 
**Edition** | Pointer to **string** |  | [optional] 
**ServerUUIDs** | Pointer to **[]string** |  | [optional] 
**Reason** | Pointer to **string** |  | [optional] 
**Warning** | Pointer to **string** |  | [optional] 
**InvalidCode** | Pointer to **string** |  | [optional] 
**Entitlements** | Pointer to [**[]LicenseEntitlement**](LicenseEntitlement.md) |  | [optional] 

## Methods

### NewLicenseInfoResponse

`func NewLicenseInfoResponse() *LicenseInfoResponse`

NewLicenseInfoResponse instantiates a new LicenseInfoResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseInfoResponseWithDefaults

`func NewLicenseInfoResponseWithDefaults() *LicenseInfoResponse`

NewLicenseInfoResponseWithDefaults instantiates a new LicenseInfoResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAuthorized

`func (o *LicenseInfoResponse) GetAuthorized() bool`

GetAuthorized returns the Authorized field if non-nil, zero value otherwise.

### GetAuthorizedOk

`func (o *LicenseInfoResponse) GetAuthorizedOk() (*bool, bool)`

GetAuthorizedOk returns a tuple with the Authorized field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthorized

`func (o *LicenseInfoResponse) SetAuthorized(v bool)`

SetAuthorized sets Authorized field to given value.

### HasAuthorized

`func (o *LicenseInfoResponse) HasAuthorized() bool`

HasAuthorized returns a boolean if a field has been set.

### GetCompany

`func (o *LicenseInfoResponse) GetCompany() string`

GetCompany returns the Company field if non-nil, zero value otherwise.

### GetCompanyOk

`func (o *LicenseInfoResponse) GetCompanyOk() (*string, bool)`

GetCompanyOk returns a tuple with the Company field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompany

`func (o *LicenseInfoResponse) SetCompany(v string)`

SetCompany sets Company field to given value.

### HasCompany

`func (o *LicenseInfoResponse) HasCompany() bool`

HasCompany returns a boolean if a field has been set.

### GetContactEmail

`func (o *LicenseInfoResponse) GetContactEmail() string`

GetContactEmail returns the ContactEmail field if non-nil, zero value otherwise.

### GetContactEmailOk

`func (o *LicenseInfoResponse) GetContactEmailOk() (*string, bool)`

GetContactEmailOk returns a tuple with the ContactEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactEmail

`func (o *LicenseInfoResponse) SetContactEmail(v string)`

SetContactEmail sets ContactEmail field to given value.

### HasContactEmail

`func (o *LicenseInfoResponse) HasContactEmail() bool`

HasContactEmail returns a boolean if a field has been set.

### GetApplication

`func (o *LicenseInfoResponse) GetApplication() string`

GetApplication returns the Application field if non-nil, zero value otherwise.

### GetApplicationOk

`func (o *LicenseInfoResponse) GetApplicationOk() (*string, bool)`

GetApplicationOk returns a tuple with the Application field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApplication

`func (o *LicenseInfoResponse) SetApplication(v string)`

SetApplication sets Application field to given value.

### HasApplication

`func (o *LicenseInfoResponse) HasApplication() bool`

HasApplication returns a boolean if a field has been set.

### GetEditions

`func (o *LicenseInfoResponse) GetEditions() []string`

GetEditions returns the Editions field if non-nil, zero value otherwise.

### GetEditionsOk

`func (o *LicenseInfoResponse) GetEditionsOk() (*[]string, bool)`

GetEditionsOk returns a tuple with the Editions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEditions

`func (o *LicenseInfoResponse) SetEditions(v []string)`

SetEditions sets Editions field to given value.

### HasEditions

`func (o *LicenseInfoResponse) HasEditions() bool`

HasEditions returns a boolean if a field has been set.

### GetApplicationVersion

`func (o *LicenseInfoResponse) GetApplicationVersion() []string`

GetApplicationVersion returns the ApplicationVersion field if non-nil, zero value otherwise.

### GetApplicationVersionOk

`func (o *LicenseInfoResponse) GetApplicationVersionOk() (*[]string, bool)`

GetApplicationVersionOk returns a tuple with the ApplicationVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApplicationVersion

`func (o *LicenseInfoResponse) SetApplicationVersion(v []string)`

SetApplicationVersion sets ApplicationVersion field to given value.

### HasApplicationVersion

`func (o *LicenseInfoResponse) HasApplicationVersion() bool`

HasApplicationVersion returns a boolean if a field has been set.

### GetGracePeriod

`func (o *LicenseInfoResponse) GetGracePeriod() int32`

GetGracePeriod returns the GracePeriod field if non-nil, zero value otherwise.

### GetGracePeriodOk

`func (o *LicenseInfoResponse) GetGracePeriodOk() (*int32, bool)`

GetGracePeriodOk returns a tuple with the GracePeriod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGracePeriod

`func (o *LicenseInfoResponse) SetGracePeriod(v int32)`

SetGracePeriod sets GracePeriod field to given value.

### HasGracePeriod

`func (o *LicenseInfoResponse) HasGracePeriod() bool`

HasGracePeriod returns a boolean if a field has been set.

### GetType

`func (o *LicenseInfoResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *LicenseInfoResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *LicenseInfoResponse) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *LicenseInfoResponse) HasType() bool`

HasType returns a boolean if a field has been set.

### GetLicenseId

`func (o *LicenseInfoResponse) GetLicenseId() string`

GetLicenseId returns the LicenseId field if non-nil, zero value otherwise.

### GetLicenseIdOk

`func (o *LicenseInfoResponse) GetLicenseIdOk() (*string, bool)`

GetLicenseIdOk returns a tuple with the LicenseId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseId

`func (o *LicenseInfoResponse) SetLicenseId(v string)`

SetLicenseId sets LicenseId field to given value.

### HasLicenseId

`func (o *LicenseInfoResponse) HasLicenseId() bool`

HasLicenseId returns a boolean if a field has been set.

### GetLicenseVersion

`func (o *LicenseInfoResponse) GetLicenseVersion() string`

GetLicenseVersion returns the LicenseVersion field if non-nil, zero value otherwise.

### GetLicenseVersionOk

`func (o *LicenseInfoResponse) GetLicenseVersionOk() (*string, bool)`

GetLicenseVersionOk returns a tuple with the LicenseVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseVersion

`func (o *LicenseInfoResponse) SetLicenseVersion(v string)`

SetLicenseVersion sets LicenseVersion field to given value.

### HasLicenseVersion

`func (o *LicenseInfoResponse) HasLicenseVersion() bool`

HasLicenseVersion returns a boolean if a field has been set.

### GetIssueDate

`func (o *LicenseInfoResponse) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *LicenseInfoResponse) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *LicenseInfoResponse) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.

### HasIssueDate

`func (o *LicenseInfoResponse) HasIssueDate() bool`

HasIssueDate returns a boolean if a field has been set.

### GetValidSince

`func (o *LicenseInfoResponse) GetValidSince() string`

GetValidSince returns the ValidSince field if non-nil, zero value otherwise.

### GetValidSinceOk

`func (o *LicenseInfoResponse) GetValidSinceOk() (*string, bool)`

GetValidSinceOk returns a tuple with the ValidSince field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValidSince

`func (o *LicenseInfoResponse) SetValidSince(v string)`

SetValidSince sets ValidSince field to given value.

### HasValidSince

`func (o *LicenseInfoResponse) HasValidSince() bool`

HasValidSince returns a boolean if a field has been set.

### GetValidUntil

`func (o *LicenseInfoResponse) GetValidUntil() string`

GetValidUntil returns the ValidUntil field if non-nil, zero value otherwise.

### GetValidUntilOk

`func (o *LicenseInfoResponse) GetValidUntilOk() (*string, bool)`

GetValidUntilOk returns a tuple with the ValidUntil field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValidUntil

`func (o *LicenseInfoResponse) SetValidUntil(v string)`

SetValidUntil sets ValidUntil field to given value.

### HasValidUntil

`func (o *LicenseInfoResponse) HasValidUntil() bool`

HasValidUntil returns a boolean if a field has been set.

### GetGraceUntil

`func (o *LicenseInfoResponse) GetGraceUntil() string`

GetGraceUntil returns the GraceUntil field if non-nil, zero value otherwise.

### GetGraceUntilOk

`func (o *LicenseInfoResponse) GetGraceUntilOk() (*string, bool)`

GetGraceUntilOk returns a tuple with the GraceUntil field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGraceUntil

`func (o *LicenseInfoResponse) SetGraceUntil(v string)`

SetGraceUntil sets GraceUntil field to given value.

### HasGraceUntil

`func (o *LicenseInfoResponse) HasGraceUntil() bool`

HasGraceUntil returns a boolean if a field has been set.

### GetState

`func (o *LicenseInfoResponse) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *LicenseInfoResponse) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *LicenseInfoResponse) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *LicenseInfoResponse) HasState() bool`

HasState returns a boolean if a field has been set.

### GetPerpetual

`func (o *LicenseInfoResponse) GetPerpetual() bool`

GetPerpetual returns the Perpetual field if non-nil, zero value otherwise.

### GetPerpetualOk

`func (o *LicenseInfoResponse) GetPerpetualOk() (*bool, bool)`

GetPerpetualOk returns a tuple with the Perpetual field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerpetual

`func (o *LicenseInfoResponse) SetPerpetual(v bool)`

SetPerpetual sets Perpetual field to given value.

### HasPerpetual

`func (o *LicenseInfoResponse) HasPerpetual() bool`

HasPerpetual returns a boolean if a field has been set.

### GetActive

`func (o *LicenseInfoResponse) GetActive() bool`

GetActive returns the Active field if non-nil, zero value otherwise.

### GetActiveOk

`func (o *LicenseInfoResponse) GetActiveOk() (*bool, bool)`

GetActiveOk returns a tuple with the Active field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActive

`func (o *LicenseInfoResponse) SetActive(v bool)`

SetActive sets Active field to given value.

### HasActive

`func (o *LicenseInfoResponse) HasActive() bool`

HasActive returns a boolean if a field has been set.

### GetRemaining

`func (o *LicenseInfoResponse) GetRemaining() int32`

GetRemaining returns the Remaining field if non-nil, zero value otherwise.

### GetRemainingOk

`func (o *LicenseInfoResponse) GetRemainingOk() (*int32, bool)`

GetRemainingOk returns a tuple with the Remaining field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemaining

`func (o *LicenseInfoResponse) SetRemaining(v int32)`

SetRemaining sets Remaining field to given value.

### HasRemaining

`func (o *LicenseInfoResponse) HasRemaining() bool`

HasRemaining returns a boolean if a field has been set.

### GetShouldWarn

`func (o *LicenseInfoResponse) GetShouldWarn() bool`

GetShouldWarn returns the ShouldWarn field if non-nil, zero value otherwise.

### GetShouldWarnOk

`func (o *LicenseInfoResponse) GetShouldWarnOk() (*bool, bool)`

GetShouldWarnOk returns a tuple with the ShouldWarn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShouldWarn

`func (o *LicenseInfoResponse) SetShouldWarn(v bool)`

SetShouldWarn sets ShouldWarn field to given value.

### HasShouldWarn

`func (o *LicenseInfoResponse) HasShouldWarn() bool`

HasShouldWarn returns a boolean if a field has been set.

### GetBaseUrl

`func (o *LicenseInfoResponse) GetBaseUrl() string`

GetBaseUrl returns the BaseUrl field if non-nil, zero value otherwise.

### GetBaseUrlOk

`func (o *LicenseInfoResponse) GetBaseUrlOk() (*string, bool)`

GetBaseUrlOk returns a tuple with the BaseUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBaseUrl

`func (o *LicenseInfoResponse) SetBaseUrl(v string)`

SetBaseUrl sets BaseUrl field to given value.

### HasBaseUrl

`func (o *LicenseInfoResponse) HasBaseUrl() bool`

HasBaseUrl returns a boolean if a field has been set.

### GetEdition

`func (o *LicenseInfoResponse) GetEdition() string`

GetEdition returns the Edition field if non-nil, zero value otherwise.

### GetEditionOk

`func (o *LicenseInfoResponse) GetEditionOk() (*string, bool)`

GetEditionOk returns a tuple with the Edition field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEdition

`func (o *LicenseInfoResponse) SetEdition(v string)`

SetEdition sets Edition field to given value.

### HasEdition

`func (o *LicenseInfoResponse) HasEdition() bool`

HasEdition returns a boolean if a field has been set.

### GetServerUUIDs

`func (o *LicenseInfoResponse) GetServerUUIDs() []string`

GetServerUUIDs returns the ServerUUIDs field if non-nil, zero value otherwise.

### GetServerUUIDsOk

`func (o *LicenseInfoResponse) GetServerUUIDsOk() (*[]string, bool)`

GetServerUUIDsOk returns a tuple with the ServerUUIDs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServerUUIDs

`func (o *LicenseInfoResponse) SetServerUUIDs(v []string)`

SetServerUUIDs sets ServerUUIDs field to given value.

### HasServerUUIDs

`func (o *LicenseInfoResponse) HasServerUUIDs() bool`

HasServerUUIDs returns a boolean if a field has been set.

### GetReason

`func (o *LicenseInfoResponse) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *LicenseInfoResponse) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *LicenseInfoResponse) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *LicenseInfoResponse) HasReason() bool`

HasReason returns a boolean if a field has been set.

### GetWarning

`func (o *LicenseInfoResponse) GetWarning() string`

GetWarning returns the Warning field if non-nil, zero value otherwise.

### GetWarningOk

`func (o *LicenseInfoResponse) GetWarningOk() (*string, bool)`

GetWarningOk returns a tuple with the Warning field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWarning

`func (o *LicenseInfoResponse) SetWarning(v string)`

SetWarning sets Warning field to given value.

### HasWarning

`func (o *LicenseInfoResponse) HasWarning() bool`

HasWarning returns a boolean if a field has been set.

### GetInvalidCode

`func (o *LicenseInfoResponse) GetInvalidCode() string`

GetInvalidCode returns the InvalidCode field if non-nil, zero value otherwise.

### GetInvalidCodeOk

`func (o *LicenseInfoResponse) GetInvalidCodeOk() (*string, bool)`

GetInvalidCodeOk returns a tuple with the InvalidCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvalidCode

`func (o *LicenseInfoResponse) SetInvalidCode(v string)`

SetInvalidCode sets InvalidCode field to given value.

### HasInvalidCode

`func (o *LicenseInfoResponse) HasInvalidCode() bool`

HasInvalidCode returns a boolean if a field has been set.

### GetEntitlements

`func (o *LicenseInfoResponse) GetEntitlements() []LicenseEntitlement`

GetEntitlements returns the Entitlements field if non-nil, zero value otherwise.

### GetEntitlementsOk

`func (o *LicenseInfoResponse) GetEntitlementsOk() (*[]LicenseEntitlement, bool)`

GetEntitlementsOk returns a tuple with the Entitlements field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntitlements

`func (o *LicenseInfoResponse) SetEntitlements(v []LicenseEntitlement)`

SetEntitlements sets Entitlements field to given value.

### HasEntitlements

`func (o *LicenseInfoResponse) HasEntitlements() bool`

HasEntitlements returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



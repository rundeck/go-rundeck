# \LicenseAPI

All URIs are relative to *https://localhost:4440/api/56*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiStoreLicense**](LicenseAPI.md#ApiStoreLicense) | **Post** /enterprise/license | Set License Key
[**Verify**](LicenseAPI.md#Verify) | **Get** /enterprise/license | View License



## ApiStoreLicense

> Basic ApiStoreLicense(ctx).LicenseAgreement(licenseAgreement).Body(body).Execute()

Set License Key



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {
	licenseAgreement := TODO // interface{} | true to agree with the Runbook Automation License
	body := "-----BEGIN PGP MESSAGE-----
Version: ...
...
-----END PGP MESSAGE-----
" // string | The Runbook Automation License key file

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicenseAPI.ApiStoreLicense(context.Background()).LicenseAgreement(licenseAgreement).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicenseAPI.ApiStoreLicense``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiStoreLicense`: Basic
	fmt.Fprintf(os.Stdout, "Response from `LicenseAPI.ApiStoreLicense`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiStoreLicenseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **licenseAgreement** | [**interface{}**](interface{}.md) | true to agree with the Runbook Automation License | 
 **body** | **string** | The Runbook Automation License key file | 

### Return type

[**Basic**](Basic.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: application/x-rundeck-license
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Verify

> LicenseInfoResponse Verify(ctx).Execute()

View License



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rundeck/go-rundeck/rundeck-v2"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicenseAPI.Verify(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicenseAPI.Verify``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Verify`: LicenseInfoResponse
	fmt.Fprintf(os.Stdout, "Response from `LicenseAPI.Verify`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiVerifyRequest struct via the builder pattern


### Return type

[**LicenseInfoResponse**](LicenseInfoResponse.md)

### Authorization

[rundeckApiToken](../README.md#rundeckApiToken), [rundeckJWT](../README.md#rundeckJWT), [rundeckPassword](../README.md#rundeckPassword)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


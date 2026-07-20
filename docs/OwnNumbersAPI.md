# \OwnNumbersAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteOwnNumber**](OwnNumbersAPI.md#DeleteOwnNumber) | **Delete** /v3/own-numbers/{own_number_id} | Delete Own Number
[**GetOwnNumberDetail**](OwnNumbersAPI.md#GetOwnNumberDetail) | **Get** /v3/own-numbers/{own_number_id} | Get Own Number Detail
[**ListOwnNumbers**](OwnNumbersAPI.md#ListOwnNumbers) | **Get** /v3/own-numbers | List Own Numbers
[**RequestOwnNumberVerificationOtp**](OwnNumbersAPI.md#RequestOwnNumberVerificationOtp) | **Post** /v3/own-numbers/verifications | Request Own Number Verification OTP
[**UpdateOwnNumber**](OwnNumbersAPI.md#UpdateOwnNumber) | **Patch** /v3/own-numbers/{own_number_id} | Update Own Number
[**VerifyOwnNumberOtp**](OwnNumbersAPI.md#VerifyOwnNumberOtp) | **Post** /v3/own-numbers/verifications/{verification_id}/verify | Verify Own Number OTP



## DeleteOwnNumber

> OwnNumber DeleteOwnNumber(ctx, ownNumberId).ContentType(contentType).Execute()

Delete Own Number



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	ownNumberId := "ownNumberId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OwnNumbersAPI.DeleteOwnNumber(context.Background(), ownNumberId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OwnNumbersAPI.DeleteOwnNumber``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteOwnNumber`: OwnNumber
	fmt.Fprintf(os.Stdout, "Response from `OwnNumbersAPI.DeleteOwnNumber`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ownNumberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteOwnNumberRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**OwnNumber**](OwnNumber.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetOwnNumberDetail

> OwnNumber GetOwnNumberDetail(ctx, ownNumberId).ContentType(contentType).Execute()

Get Own Number Detail



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	ownNumberId := "ownNumberId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OwnNumbersAPI.GetOwnNumberDetail(context.Background(), ownNumberId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OwnNumbersAPI.GetOwnNumberDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOwnNumberDetail`: OwnNumber
	fmt.Fprintf(os.Stdout, "Response from `OwnNumbersAPI.GetOwnNumberDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ownNumberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetOwnNumberDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**OwnNumber**](OwnNumber.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListOwnNumbers

> ListOwnNumbers ListOwnNumbers(ctx).ContentType(contentType).Execute()

List Own Numbers



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OwnNumbersAPI.ListOwnNumbers(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OwnNumbersAPI.ListOwnNumbers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListOwnNumbers`: ListOwnNumbers
	fmt.Fprintf(os.Stdout, "Response from `OwnNumbersAPI.ListOwnNumbers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListOwnNumbersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ListOwnNumbers**](ListOwnNumbers.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RequestOwnNumberVerificationOtp

> RequestOwnNumberVerificationOtp RequestOwnNumberVerificationOtp(ctx).ContentType(contentType).RequestOwnNumberVerificationOtpRequest(requestOwnNumberVerificationOtpRequest).Execute()

Request Own Number Verification OTP



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	contentType := "application/json" // string |  (optional)
	requestOwnNumberVerificationOtpRequest := *openapiclient.NewRequestOwnNumberVerificationOtpRequest() // RequestOwnNumberVerificationOtpRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OwnNumbersAPI.RequestOwnNumberVerificationOtp(context.Background()).ContentType(contentType).RequestOwnNumberVerificationOtpRequest(requestOwnNumberVerificationOtpRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OwnNumbersAPI.RequestOwnNumberVerificationOtp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RequestOwnNumberVerificationOtp`: RequestOwnNumberVerificationOtp
	fmt.Fprintf(os.Stdout, "Response from `OwnNumbersAPI.RequestOwnNumberVerificationOtp`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRequestOwnNumberVerificationOtpRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **requestOwnNumberVerificationOtpRequest** | [**RequestOwnNumberVerificationOtpRequest**](RequestOwnNumberVerificationOtpRequest.md) |  | 

### Return type

[**RequestOwnNumberVerificationOtp**](RequestOwnNumberVerificationOtp.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateOwnNumber

> OwnNumber UpdateOwnNumber(ctx, ownNumberId).Execute()

Update Own Number



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	ownNumberId := "ownNumberId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OwnNumbersAPI.UpdateOwnNumber(context.Background(), ownNumberId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OwnNumbersAPI.UpdateOwnNumber``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateOwnNumber`: OwnNumber
	fmt.Fprintf(os.Stdout, "Response from `OwnNumbersAPI.UpdateOwnNumber`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ownNumberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateOwnNumberRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**OwnNumber**](OwnNumber.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## VerifyOwnNumberOtp

> VerifyOwnNumberOtp VerifyOwnNumberOtp(ctx, verificationId).ContentType(contentType).VerifyOwnNumberOtpRequest(verifyOwnNumberOtpRequest).Execute()

Verify Own Number OTP



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	verificationId := "verificationId_example" // string | 
	contentType := "application/json" // string |  (optional)
	verifyOwnNumberOtpRequest := *openapiclient.NewVerifyOwnNumberOtpRequest() // VerifyOwnNumberOtpRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OwnNumbersAPI.VerifyOwnNumberOtp(context.Background(), verificationId).ContentType(contentType).VerifyOwnNumberOtpRequest(verifyOwnNumberOtpRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OwnNumbersAPI.VerifyOwnNumberOtp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VerifyOwnNumberOtp`: VerifyOwnNumberOtp
	fmt.Fprintf(os.Stdout, "Response from `OwnNumbersAPI.VerifyOwnNumberOtp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**verificationId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiVerifyOwnNumberOtpRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **verifyOwnNumberOtpRequest** | [**VerifyOwnNumberOtpRequest**](VerifyOwnNumberOtpRequest.md) |  | 

### Return type

[**VerifyOwnNumberOtp**](VerifyOwnNumberOtp.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


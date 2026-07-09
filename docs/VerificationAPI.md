# \VerificationAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ForgotPassword**](VerificationAPI.md#ForgotPassword) | **Put** /v3/forgot-password | Forgot Password
[**ForgotUsername**](VerificationAPI.md#ForgotUsername) | **Put** /v3/forgot-username | Forgot Username



## ForgotPassword

> ForgotPassword ForgotPassword(ctx).ContentType(contentType).ForgotPasswordRequest(forgotPasswordRequest).Execute()

Forgot Password



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	contentType := "application/json" // string |  (optional)
	forgotPasswordRequest := *openapiclient.NewForgotPasswordRequest() // ForgotPasswordRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VerificationAPI.ForgotPassword(context.Background()).ContentType(contentType).ForgotPasswordRequest(forgotPasswordRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VerificationAPI.ForgotPassword``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ForgotPassword`: ForgotPassword
	fmt.Fprintf(os.Stdout, "Response from `VerificationAPI.ForgotPassword`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiForgotPasswordRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **forgotPasswordRequest** | [**ForgotPasswordRequest**](ForgotPasswordRequest.md) |  | 

### Return type

[**ForgotPassword**](ForgotPassword.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ForgotUsername

> ForgotUsername ForgotUsername(ctx).ContentType(contentType).ForgotUsernameRequest(forgotUsernameRequest).Execute()

Forgot Username



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	contentType := "application/json" // string |  (optional)
	forgotUsernameRequest := *openapiclient.NewForgotUsernameRequest() // ForgotUsernameRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VerificationAPI.ForgotUsername(context.Background()).ContentType(contentType).ForgotUsernameRequest(forgotUsernameRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VerificationAPI.ForgotUsername``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ForgotUsername`: ForgotUsername
	fmt.Fprintf(os.Stdout, "Response from `VerificationAPI.ForgotUsername`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiForgotUsernameRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **forgotUsernameRequest** | [**ForgotUsernameRequest**](ForgotUsernameRequest.md) |  | 

### Return type

[**ForgotUsername**](ForgotUsername.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


# \InternationalMessagingAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AgreeToRulesAndRegulation**](InternationalMessagingAPI.md#AgreeToRulesAndRegulation) | **Post** /v3/user-countries/agree | Agree to rules and regulation
[**GetCountriesForGlobalSending**](InternationalMessagingAPI.md#GetCountriesForGlobalSending) | **Get** /v3/user-countries | Get Countries for Global Sending
[**ListCountries**](InternationalMessagingAPI.md#ListCountries) | **Get** /v3/country-list | International Messaging
[**SelectCountriesForGlobalSending**](InternationalMessagingAPI.md#SelectCountriesForGlobalSending) | **Post** /v3/user-countries | Select Countries for Global Sending
[**Timezones**](InternationalMessagingAPI.md#Timezones) | **Get** /v3/timezones | Timezones
[**ViewCountries**](InternationalMessagingAPI.md#ViewCountries) | **Get** /v3/countries | View Countries



## AgreeToRulesAndRegulation

> AgreeToRulesAndRegulation AgreeToRulesAndRegulation(ctx).Execute()

Agree to rules and regulation



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InternationalMessagingAPI.AgreeToRulesAndRegulation(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InternationalMessagingAPI.AgreeToRulesAndRegulation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AgreeToRulesAndRegulation`: AgreeToRulesAndRegulation
	fmt.Fprintf(os.Stdout, "Response from `InternationalMessagingAPI.AgreeToRulesAndRegulation`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAgreeToRulesAndRegulationRequest struct via the builder pattern


### Return type

[**AgreeToRulesAndRegulation**](AgreeToRulesAndRegulation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetCountriesForGlobalSending

> GetCountriesForGlobalSending GetCountriesForGlobalSending(ctx).Execute()

Get Countries for Global Sending



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InternationalMessagingAPI.GetCountriesForGlobalSending(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InternationalMessagingAPI.GetCountriesForGlobalSending``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCountriesForGlobalSending`: GetCountriesForGlobalSending
	fmt.Fprintf(os.Stdout, "Response from `InternationalMessagingAPI.GetCountriesForGlobalSending`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetCountriesForGlobalSendingRequest struct via the builder pattern


### Return type

[**GetCountriesForGlobalSending**](GetCountriesForGlobalSending.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCountries

> ListCountries ListCountries(ctx).Execute()

International Messaging



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InternationalMessagingAPI.ListCountries(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InternationalMessagingAPI.ListCountries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCountries`: ListCountries
	fmt.Fprintf(os.Stdout, "Response from `InternationalMessagingAPI.ListCountries`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListCountriesRequest struct via the builder pattern


### Return type

[**ListCountries**](ListCountries.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SelectCountriesForGlobalSending

> SelectCountriesForGlobalSending SelectCountriesForGlobalSending(ctx).SelectCountriesForGlobalSendingRequest(selectCountriesForGlobalSendingRequest).Execute()

Select Countries for Global Sending



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
	selectCountriesForGlobalSendingRequest := *openapiclient.NewSelectCountriesForGlobalSendingRequest() // SelectCountriesForGlobalSendingRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InternationalMessagingAPI.SelectCountriesForGlobalSending(context.Background()).SelectCountriesForGlobalSendingRequest(selectCountriesForGlobalSendingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InternationalMessagingAPI.SelectCountriesForGlobalSending``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SelectCountriesForGlobalSending`: SelectCountriesForGlobalSending
	fmt.Fprintf(os.Stdout, "Response from `InternationalMessagingAPI.SelectCountriesForGlobalSending`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSelectCountriesForGlobalSendingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **selectCountriesForGlobalSendingRequest** | [**SelectCountriesForGlobalSendingRequest**](SelectCountriesForGlobalSendingRequest.md) |  | 

### Return type

[**SelectCountriesForGlobalSending**](SelectCountriesForGlobalSending.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Timezones

> Timezones Timezones(ctx).ContentType(contentType).Execute()

Timezones



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InternationalMessagingAPI.Timezones(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InternationalMessagingAPI.Timezones``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Timezones`: Timezones
	fmt.Fprintf(os.Stdout, "Response from `InternationalMessagingAPI.Timezones`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTimezonesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**Timezones**](Timezones.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewCountries

> ViewCountries ViewCountries(ctx).Execute()

View Countries



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InternationalMessagingAPI.ViewCountries(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InternationalMessagingAPI.ViewCountries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewCountries`: ViewCountries
	fmt.Fprintf(os.Stdout, "Response from `InternationalMessagingAPI.ViewCountries`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiViewCountriesRequest struct via the builder pattern


### Return type

[**ViewCountries**](ViewCountries.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


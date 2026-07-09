# RegisterNumbersRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FullName** | **string** | Legal full name of the individual registering the number. Must be a personal name, not a business name. | 
**CompanyName** | **string** | Legal business name of the organization requesting registration | 
**Email** | **string** | Contact email address for registration communications and notifications | 
**WebsiteUrl** | **string** | Official business website URL | 
**SampleMessage** | **string** | Representative example of messages that will be sent using this number | 
**PrimaryUseCase** | **string** | Primary intended purpose for the registered number (e.g., Marketing, Notifications, Authentication) | 
**CompanyNumber** | **string** | Official support phone number of the organization requesting registration | 
**AreaCode** | **string** | Your area codes, please provide your top 3 area codes in case your 1st choice is not available | 

## Methods

### NewRegisterNumbersRequest

`func NewRegisterNumbersRequest(fullName string, companyName string, email string, websiteUrl string, sampleMessage string, primaryUseCase string, companyNumber string, areaCode string, ) *RegisterNumbersRequest`

NewRegisterNumbersRequest instantiates a new RegisterNumbersRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRegisterNumbersRequestWithDefaults

`func NewRegisterNumbersRequestWithDefaults() *RegisterNumbersRequest`

NewRegisterNumbersRequestWithDefaults instantiates a new RegisterNumbersRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFullName

`func (o *RegisterNumbersRequest) GetFullName() string`

GetFullName returns the FullName field if non-nil, zero value otherwise.

### GetFullNameOk

`func (o *RegisterNumbersRequest) GetFullNameOk() (*string, bool)`

GetFullNameOk returns a tuple with the FullName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullName

`func (o *RegisterNumbersRequest) SetFullName(v string)`

SetFullName sets FullName field to given value.


### GetCompanyName

`func (o *RegisterNumbersRequest) GetCompanyName() string`

GetCompanyName returns the CompanyName field if non-nil, zero value otherwise.

### GetCompanyNameOk

`func (o *RegisterNumbersRequest) GetCompanyNameOk() (*string, bool)`

GetCompanyNameOk returns a tuple with the CompanyName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompanyName

`func (o *RegisterNumbersRequest) SetCompanyName(v string)`

SetCompanyName sets CompanyName field to given value.


### GetEmail

`func (o *RegisterNumbersRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *RegisterNumbersRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *RegisterNumbersRequest) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetWebsiteUrl

`func (o *RegisterNumbersRequest) GetWebsiteUrl() string`

GetWebsiteUrl returns the WebsiteUrl field if non-nil, zero value otherwise.

### GetWebsiteUrlOk

`func (o *RegisterNumbersRequest) GetWebsiteUrlOk() (*string, bool)`

GetWebsiteUrlOk returns a tuple with the WebsiteUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsiteUrl

`func (o *RegisterNumbersRequest) SetWebsiteUrl(v string)`

SetWebsiteUrl sets WebsiteUrl field to given value.


### GetSampleMessage

`func (o *RegisterNumbersRequest) GetSampleMessage() string`

GetSampleMessage returns the SampleMessage field if non-nil, zero value otherwise.

### GetSampleMessageOk

`func (o *RegisterNumbersRequest) GetSampleMessageOk() (*string, bool)`

GetSampleMessageOk returns a tuple with the SampleMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSampleMessage

`func (o *RegisterNumbersRequest) SetSampleMessage(v string)`

SetSampleMessage sets SampleMessage field to given value.


### GetPrimaryUseCase

`func (o *RegisterNumbersRequest) GetPrimaryUseCase() string`

GetPrimaryUseCase returns the PrimaryUseCase field if non-nil, zero value otherwise.

### GetPrimaryUseCaseOk

`func (o *RegisterNumbersRequest) GetPrimaryUseCaseOk() (*string, bool)`

GetPrimaryUseCaseOk returns a tuple with the PrimaryUseCase field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrimaryUseCase

`func (o *RegisterNumbersRequest) SetPrimaryUseCase(v string)`

SetPrimaryUseCase sets PrimaryUseCase field to given value.


### GetCompanyNumber

`func (o *RegisterNumbersRequest) GetCompanyNumber() string`

GetCompanyNumber returns the CompanyNumber field if non-nil, zero value otherwise.

### GetCompanyNumberOk

`func (o *RegisterNumbersRequest) GetCompanyNumberOk() (*string, bool)`

GetCompanyNumberOk returns a tuple with the CompanyNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompanyNumber

`func (o *RegisterNumbersRequest) SetCompanyNumber(v string)`

SetCompanyNumber sets CompanyNumber field to given value.


### GetAreaCode

`func (o *RegisterNumbersRequest) GetAreaCode() string`

GetAreaCode returns the AreaCode field if non-nil, zero value otherwise.

### GetAreaCodeOk

`func (o *RegisterNumbersRequest) GetAreaCodeOk() (*string, bool)`

GetAreaCodeOk returns a tuple with the AreaCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAreaCode

`func (o *RegisterNumbersRequest) SetAreaCode(v string)`

SetAreaCode sets AreaCode field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



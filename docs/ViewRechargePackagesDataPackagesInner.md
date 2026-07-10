# ViewRechargePackagesDataPackagesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PackageId** | Pointer to **float32** | The ID of the package. | [optional] 
**PackagePrice** | Pointer to **string** | The price of the package. | [optional] 
**PriceRate** | Pointer to **int32** | The pricing tier used to determine the cost per message. | [optional] 
**SmsPrice** | Pointer to **float32** | The price of the SMS. | [optional] 
**SmsQuantity** | Pointer to **float32** | The quantity of the SMS. | [optional] 
**VoiceMobilePrice** | Pointer to **float32** | The price of the voice mobile. | [optional] 
**VoiceMobileQuantity** | Pointer to **float32** | The quantity of the voice mobile. | [optional] 
**VoiceLandlinePrice** | Pointer to **float32** | The price of the voice landline. | [optional] 
**VoiceLandlineQuantity** | Pointer to **float32** | The quantity of the voice landline. | [optional] 
**FaxPrice** | Pointer to **float32** | The price of the fax. | [optional] 
**FaxQuantity** | Pointer to **float32** | The quantity of the fax. | [optional] 
**EmailPrice** | Pointer to **float32** | The price of the email. | [optional] 
**EmailQuantity** | Pointer to **float32** | The quantity of the email. | [optional] 
**PostLetterBlackPrice** | Pointer to **float32** | The price of the post letter black. | [optional] 
**PostLetterColourPrice** | Pointer to **float32** | The price of the post letter colour. | [optional] 
**PostPageBlackPrice** | Pointer to **float32** | The price of the post page black. | [optional] 
**PostPageColourPrice** | Pointer to **float32** | The price of the post page colour. | [optional] 
**PostLetterBlackQuantity** | Pointer to **float32** | The quantity of the post letter black. | [optional] 
**PostLetterColourQuantity** | Pointer to **float32** | The quantity of the post letter colour. | [optional] 
**PostDirectMailDlPrice** | Pointer to **float32** | The price of the post direct mail dl. | [optional] 
**PostDirectMailA5Price** | Pointer to **float32** | The price of the post direct mail a5. | [optional] 
**PostDirectMailMinQuantity** | Pointer to **float32** | The quantity of the post direct mail min. | [optional] 
**PostcardPrice** | Pointer to **float32** | The price of the postcard. | [optional] 
**PostcardQuantity** | Pointer to **float32** | The quantity of the postcard. | [optional] 
**AutomationPrice** | Pointer to **float32** | The price of the automation. | [optional] 

## Methods

### NewViewRechargePackagesDataPackagesInner

`func NewViewRechargePackagesDataPackagesInner() *ViewRechargePackagesDataPackagesInner`

NewViewRechargePackagesDataPackagesInner instantiates a new ViewRechargePackagesDataPackagesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewRechargePackagesDataPackagesInnerWithDefaults

`func NewViewRechargePackagesDataPackagesInnerWithDefaults() *ViewRechargePackagesDataPackagesInner`

NewViewRechargePackagesDataPackagesInnerWithDefaults instantiates a new ViewRechargePackagesDataPackagesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPackageId

`func (o *ViewRechargePackagesDataPackagesInner) GetPackageId() float32`

GetPackageId returns the PackageId field if non-nil, zero value otherwise.

### GetPackageIdOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPackageIdOk() (*float32, bool)`

GetPackageIdOk returns a tuple with the PackageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackageId

`func (o *ViewRechargePackagesDataPackagesInner) SetPackageId(v float32)`

SetPackageId sets PackageId field to given value.

### HasPackageId

`func (o *ViewRechargePackagesDataPackagesInner) HasPackageId() bool`

HasPackageId returns a boolean if a field has been set.

### GetPackagePrice

`func (o *ViewRechargePackagesDataPackagesInner) GetPackagePrice() string`

GetPackagePrice returns the PackagePrice field if non-nil, zero value otherwise.

### GetPackagePriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPackagePriceOk() (*string, bool)`

GetPackagePriceOk returns a tuple with the PackagePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackagePrice

`func (o *ViewRechargePackagesDataPackagesInner) SetPackagePrice(v string)`

SetPackagePrice sets PackagePrice field to given value.

### HasPackagePrice

`func (o *ViewRechargePackagesDataPackagesInner) HasPackagePrice() bool`

HasPackagePrice returns a boolean if a field has been set.

### GetPriceRate

`func (o *ViewRechargePackagesDataPackagesInner) GetPriceRate() int32`

GetPriceRate returns the PriceRate field if non-nil, zero value otherwise.

### GetPriceRateOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPriceRateOk() (*int32, bool)`

GetPriceRateOk returns a tuple with the PriceRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceRate

`func (o *ViewRechargePackagesDataPackagesInner) SetPriceRate(v int32)`

SetPriceRate sets PriceRate field to given value.

### HasPriceRate

`func (o *ViewRechargePackagesDataPackagesInner) HasPriceRate() bool`

HasPriceRate returns a boolean if a field has been set.

### GetSmsPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetSmsPrice() float32`

GetSmsPrice returns the SmsPrice field if non-nil, zero value otherwise.

### GetSmsPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetSmsPriceOk() (*float32, bool)`

GetSmsPriceOk returns a tuple with the SmsPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSmsPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetSmsPrice(v float32)`

SetSmsPrice sets SmsPrice field to given value.

### HasSmsPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasSmsPrice() bool`

HasSmsPrice returns a boolean if a field has been set.

### GetSmsQuantity

`func (o *ViewRechargePackagesDataPackagesInner) GetSmsQuantity() float32`

GetSmsQuantity returns the SmsQuantity field if non-nil, zero value otherwise.

### GetSmsQuantityOk

`func (o *ViewRechargePackagesDataPackagesInner) GetSmsQuantityOk() (*float32, bool)`

GetSmsQuantityOk returns a tuple with the SmsQuantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSmsQuantity

`func (o *ViewRechargePackagesDataPackagesInner) SetSmsQuantity(v float32)`

SetSmsQuantity sets SmsQuantity field to given value.

### HasSmsQuantity

`func (o *ViewRechargePackagesDataPackagesInner) HasSmsQuantity() bool`

HasSmsQuantity returns a boolean if a field has been set.

### GetVoiceMobilePrice

`func (o *ViewRechargePackagesDataPackagesInner) GetVoiceMobilePrice() float32`

GetVoiceMobilePrice returns the VoiceMobilePrice field if non-nil, zero value otherwise.

### GetVoiceMobilePriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetVoiceMobilePriceOk() (*float32, bool)`

GetVoiceMobilePriceOk returns a tuple with the VoiceMobilePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVoiceMobilePrice

`func (o *ViewRechargePackagesDataPackagesInner) SetVoiceMobilePrice(v float32)`

SetVoiceMobilePrice sets VoiceMobilePrice field to given value.

### HasVoiceMobilePrice

`func (o *ViewRechargePackagesDataPackagesInner) HasVoiceMobilePrice() bool`

HasVoiceMobilePrice returns a boolean if a field has been set.

### GetVoiceMobileQuantity

`func (o *ViewRechargePackagesDataPackagesInner) GetVoiceMobileQuantity() float32`

GetVoiceMobileQuantity returns the VoiceMobileQuantity field if non-nil, zero value otherwise.

### GetVoiceMobileQuantityOk

`func (o *ViewRechargePackagesDataPackagesInner) GetVoiceMobileQuantityOk() (*float32, bool)`

GetVoiceMobileQuantityOk returns a tuple with the VoiceMobileQuantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVoiceMobileQuantity

`func (o *ViewRechargePackagesDataPackagesInner) SetVoiceMobileQuantity(v float32)`

SetVoiceMobileQuantity sets VoiceMobileQuantity field to given value.

### HasVoiceMobileQuantity

`func (o *ViewRechargePackagesDataPackagesInner) HasVoiceMobileQuantity() bool`

HasVoiceMobileQuantity returns a boolean if a field has been set.

### GetVoiceLandlinePrice

`func (o *ViewRechargePackagesDataPackagesInner) GetVoiceLandlinePrice() float32`

GetVoiceLandlinePrice returns the VoiceLandlinePrice field if non-nil, zero value otherwise.

### GetVoiceLandlinePriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetVoiceLandlinePriceOk() (*float32, bool)`

GetVoiceLandlinePriceOk returns a tuple with the VoiceLandlinePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVoiceLandlinePrice

`func (o *ViewRechargePackagesDataPackagesInner) SetVoiceLandlinePrice(v float32)`

SetVoiceLandlinePrice sets VoiceLandlinePrice field to given value.

### HasVoiceLandlinePrice

`func (o *ViewRechargePackagesDataPackagesInner) HasVoiceLandlinePrice() bool`

HasVoiceLandlinePrice returns a boolean if a field has been set.

### GetVoiceLandlineQuantity

`func (o *ViewRechargePackagesDataPackagesInner) GetVoiceLandlineQuantity() float32`

GetVoiceLandlineQuantity returns the VoiceLandlineQuantity field if non-nil, zero value otherwise.

### GetVoiceLandlineQuantityOk

`func (o *ViewRechargePackagesDataPackagesInner) GetVoiceLandlineQuantityOk() (*float32, bool)`

GetVoiceLandlineQuantityOk returns a tuple with the VoiceLandlineQuantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVoiceLandlineQuantity

`func (o *ViewRechargePackagesDataPackagesInner) SetVoiceLandlineQuantity(v float32)`

SetVoiceLandlineQuantity sets VoiceLandlineQuantity field to given value.

### HasVoiceLandlineQuantity

`func (o *ViewRechargePackagesDataPackagesInner) HasVoiceLandlineQuantity() bool`

HasVoiceLandlineQuantity returns a boolean if a field has been set.

### GetFaxPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetFaxPrice() float32`

GetFaxPrice returns the FaxPrice field if non-nil, zero value otherwise.

### GetFaxPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetFaxPriceOk() (*float32, bool)`

GetFaxPriceOk returns a tuple with the FaxPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFaxPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetFaxPrice(v float32)`

SetFaxPrice sets FaxPrice field to given value.

### HasFaxPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasFaxPrice() bool`

HasFaxPrice returns a boolean if a field has been set.

### GetFaxQuantity

`func (o *ViewRechargePackagesDataPackagesInner) GetFaxQuantity() float32`

GetFaxQuantity returns the FaxQuantity field if non-nil, zero value otherwise.

### GetFaxQuantityOk

`func (o *ViewRechargePackagesDataPackagesInner) GetFaxQuantityOk() (*float32, bool)`

GetFaxQuantityOk returns a tuple with the FaxQuantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFaxQuantity

`func (o *ViewRechargePackagesDataPackagesInner) SetFaxQuantity(v float32)`

SetFaxQuantity sets FaxQuantity field to given value.

### HasFaxQuantity

`func (o *ViewRechargePackagesDataPackagesInner) HasFaxQuantity() bool`

HasFaxQuantity returns a boolean if a field has been set.

### GetEmailPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetEmailPrice() float32`

GetEmailPrice returns the EmailPrice field if non-nil, zero value otherwise.

### GetEmailPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetEmailPriceOk() (*float32, bool)`

GetEmailPriceOk returns a tuple with the EmailPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetEmailPrice(v float32)`

SetEmailPrice sets EmailPrice field to given value.

### HasEmailPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasEmailPrice() bool`

HasEmailPrice returns a boolean if a field has been set.

### GetEmailQuantity

`func (o *ViewRechargePackagesDataPackagesInner) GetEmailQuantity() float32`

GetEmailQuantity returns the EmailQuantity field if non-nil, zero value otherwise.

### GetEmailQuantityOk

`func (o *ViewRechargePackagesDataPackagesInner) GetEmailQuantityOk() (*float32, bool)`

GetEmailQuantityOk returns a tuple with the EmailQuantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailQuantity

`func (o *ViewRechargePackagesDataPackagesInner) SetEmailQuantity(v float32)`

SetEmailQuantity sets EmailQuantity field to given value.

### HasEmailQuantity

`func (o *ViewRechargePackagesDataPackagesInner) HasEmailQuantity() bool`

HasEmailQuantity returns a boolean if a field has been set.

### GetPostLetterBlackPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetPostLetterBlackPrice() float32`

GetPostLetterBlackPrice returns the PostLetterBlackPrice field if non-nil, zero value otherwise.

### GetPostLetterBlackPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostLetterBlackPriceOk() (*float32, bool)`

GetPostLetterBlackPriceOk returns a tuple with the PostLetterBlackPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostLetterBlackPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetPostLetterBlackPrice(v float32)`

SetPostLetterBlackPrice sets PostLetterBlackPrice field to given value.

### HasPostLetterBlackPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasPostLetterBlackPrice() bool`

HasPostLetterBlackPrice returns a boolean if a field has been set.

### GetPostLetterColourPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetPostLetterColourPrice() float32`

GetPostLetterColourPrice returns the PostLetterColourPrice field if non-nil, zero value otherwise.

### GetPostLetterColourPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostLetterColourPriceOk() (*float32, bool)`

GetPostLetterColourPriceOk returns a tuple with the PostLetterColourPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostLetterColourPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetPostLetterColourPrice(v float32)`

SetPostLetterColourPrice sets PostLetterColourPrice field to given value.

### HasPostLetterColourPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasPostLetterColourPrice() bool`

HasPostLetterColourPrice returns a boolean if a field has been set.

### GetPostPageBlackPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetPostPageBlackPrice() float32`

GetPostPageBlackPrice returns the PostPageBlackPrice field if non-nil, zero value otherwise.

### GetPostPageBlackPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostPageBlackPriceOk() (*float32, bool)`

GetPostPageBlackPriceOk returns a tuple with the PostPageBlackPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostPageBlackPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetPostPageBlackPrice(v float32)`

SetPostPageBlackPrice sets PostPageBlackPrice field to given value.

### HasPostPageBlackPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasPostPageBlackPrice() bool`

HasPostPageBlackPrice returns a boolean if a field has been set.

### GetPostPageColourPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetPostPageColourPrice() float32`

GetPostPageColourPrice returns the PostPageColourPrice field if non-nil, zero value otherwise.

### GetPostPageColourPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostPageColourPriceOk() (*float32, bool)`

GetPostPageColourPriceOk returns a tuple with the PostPageColourPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostPageColourPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetPostPageColourPrice(v float32)`

SetPostPageColourPrice sets PostPageColourPrice field to given value.

### HasPostPageColourPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasPostPageColourPrice() bool`

HasPostPageColourPrice returns a boolean if a field has been set.

### GetPostLetterBlackQuantity

`func (o *ViewRechargePackagesDataPackagesInner) GetPostLetterBlackQuantity() float32`

GetPostLetterBlackQuantity returns the PostLetterBlackQuantity field if non-nil, zero value otherwise.

### GetPostLetterBlackQuantityOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostLetterBlackQuantityOk() (*float32, bool)`

GetPostLetterBlackQuantityOk returns a tuple with the PostLetterBlackQuantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostLetterBlackQuantity

`func (o *ViewRechargePackagesDataPackagesInner) SetPostLetterBlackQuantity(v float32)`

SetPostLetterBlackQuantity sets PostLetterBlackQuantity field to given value.

### HasPostLetterBlackQuantity

`func (o *ViewRechargePackagesDataPackagesInner) HasPostLetterBlackQuantity() bool`

HasPostLetterBlackQuantity returns a boolean if a field has been set.

### GetPostLetterColourQuantity

`func (o *ViewRechargePackagesDataPackagesInner) GetPostLetterColourQuantity() float32`

GetPostLetterColourQuantity returns the PostLetterColourQuantity field if non-nil, zero value otherwise.

### GetPostLetterColourQuantityOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostLetterColourQuantityOk() (*float32, bool)`

GetPostLetterColourQuantityOk returns a tuple with the PostLetterColourQuantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostLetterColourQuantity

`func (o *ViewRechargePackagesDataPackagesInner) SetPostLetterColourQuantity(v float32)`

SetPostLetterColourQuantity sets PostLetterColourQuantity field to given value.

### HasPostLetterColourQuantity

`func (o *ViewRechargePackagesDataPackagesInner) HasPostLetterColourQuantity() bool`

HasPostLetterColourQuantity returns a boolean if a field has been set.

### GetPostDirectMailDlPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetPostDirectMailDlPrice() float32`

GetPostDirectMailDlPrice returns the PostDirectMailDlPrice field if non-nil, zero value otherwise.

### GetPostDirectMailDlPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostDirectMailDlPriceOk() (*float32, bool)`

GetPostDirectMailDlPriceOk returns a tuple with the PostDirectMailDlPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostDirectMailDlPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetPostDirectMailDlPrice(v float32)`

SetPostDirectMailDlPrice sets PostDirectMailDlPrice field to given value.

### HasPostDirectMailDlPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasPostDirectMailDlPrice() bool`

HasPostDirectMailDlPrice returns a boolean if a field has been set.

### GetPostDirectMailA5Price

`func (o *ViewRechargePackagesDataPackagesInner) GetPostDirectMailA5Price() float32`

GetPostDirectMailA5Price returns the PostDirectMailA5Price field if non-nil, zero value otherwise.

### GetPostDirectMailA5PriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostDirectMailA5PriceOk() (*float32, bool)`

GetPostDirectMailA5PriceOk returns a tuple with the PostDirectMailA5Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostDirectMailA5Price

`func (o *ViewRechargePackagesDataPackagesInner) SetPostDirectMailA5Price(v float32)`

SetPostDirectMailA5Price sets PostDirectMailA5Price field to given value.

### HasPostDirectMailA5Price

`func (o *ViewRechargePackagesDataPackagesInner) HasPostDirectMailA5Price() bool`

HasPostDirectMailA5Price returns a boolean if a field has been set.

### GetPostDirectMailMinQuantity

`func (o *ViewRechargePackagesDataPackagesInner) GetPostDirectMailMinQuantity() float32`

GetPostDirectMailMinQuantity returns the PostDirectMailMinQuantity field if non-nil, zero value otherwise.

### GetPostDirectMailMinQuantityOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostDirectMailMinQuantityOk() (*float32, bool)`

GetPostDirectMailMinQuantityOk returns a tuple with the PostDirectMailMinQuantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostDirectMailMinQuantity

`func (o *ViewRechargePackagesDataPackagesInner) SetPostDirectMailMinQuantity(v float32)`

SetPostDirectMailMinQuantity sets PostDirectMailMinQuantity field to given value.

### HasPostDirectMailMinQuantity

`func (o *ViewRechargePackagesDataPackagesInner) HasPostDirectMailMinQuantity() bool`

HasPostDirectMailMinQuantity returns a boolean if a field has been set.

### GetPostcardPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetPostcardPrice() float32`

GetPostcardPrice returns the PostcardPrice field if non-nil, zero value otherwise.

### GetPostcardPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostcardPriceOk() (*float32, bool)`

GetPostcardPriceOk returns a tuple with the PostcardPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostcardPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetPostcardPrice(v float32)`

SetPostcardPrice sets PostcardPrice field to given value.

### HasPostcardPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasPostcardPrice() bool`

HasPostcardPrice returns a boolean if a field has been set.

### GetPostcardQuantity

`func (o *ViewRechargePackagesDataPackagesInner) GetPostcardQuantity() float32`

GetPostcardQuantity returns the PostcardQuantity field if non-nil, zero value otherwise.

### GetPostcardQuantityOk

`func (o *ViewRechargePackagesDataPackagesInner) GetPostcardQuantityOk() (*float32, bool)`

GetPostcardQuantityOk returns a tuple with the PostcardQuantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostcardQuantity

`func (o *ViewRechargePackagesDataPackagesInner) SetPostcardQuantity(v float32)`

SetPostcardQuantity sets PostcardQuantity field to given value.

### HasPostcardQuantity

`func (o *ViewRechargePackagesDataPackagesInner) HasPostcardQuantity() bool`

HasPostcardQuantity returns a boolean if a field has been set.

### GetAutomationPrice

`func (o *ViewRechargePackagesDataPackagesInner) GetAutomationPrice() float32`

GetAutomationPrice returns the AutomationPrice field if non-nil, zero value otherwise.

### GetAutomationPriceOk

`func (o *ViewRechargePackagesDataPackagesInner) GetAutomationPriceOk() (*float32, bool)`

GetAutomationPriceOk returns a tuple with the AutomationPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutomationPrice

`func (o *ViewRechargePackagesDataPackagesInner) SetAutomationPrice(v float32)`

SetAutomationPrice sets AutomationPrice field to given value.

### HasAutomationPrice

`func (o *ViewRechargePackagesDataPackagesInner) HasAutomationPrice() bool`

HasAutomationPrice returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



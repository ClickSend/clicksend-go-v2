# GetTrackingDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OpenCount** | Pointer to **float32** | Number of times the short URL was opened | [optional] 
**DateOpened** | Pointer to **float32** | Date in unix seconds when the short URL was first opened. Null if the short URL was never opened. | [optional] 
**UserGeoCountry** | Pointer to **string** | Country where the recipient is located when the short URL was opened. Null if the short URL was never opened. | [optional] 
**UserGeoRegion** | Pointer to **string** | Geographical region where the recipient is located when the short URL was opened. Null if the short URL was never opened. | [optional] 
**UserDevice** | Pointer to **string** | Deviced used by the recipient to open the short URL. Null if the short URL was never opened. | [optional] 
**UserBrowser** | Pointer to **string** | Browser used by the recipient to open the short URL. Null if the short URL was never opened. | [optional] 
**UserOs** | Pointer to **string** | Opearating system used by the recipient to open the short URL. Null if the short URL was never opened. | [optional] 
**Contact** | Pointer to [**GetTrackingDataInnerContact**](GetTrackingDataInnerContact.md) |  | [optional] 

## Methods

### NewGetTrackingDataInner

`func NewGetTrackingDataInner() *GetTrackingDataInner`

NewGetTrackingDataInner instantiates a new GetTrackingDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetTrackingDataInnerWithDefaults

`func NewGetTrackingDataInnerWithDefaults() *GetTrackingDataInner`

NewGetTrackingDataInnerWithDefaults instantiates a new GetTrackingDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOpenCount

`func (o *GetTrackingDataInner) GetOpenCount() float32`

GetOpenCount returns the OpenCount field if non-nil, zero value otherwise.

### GetOpenCountOk

`func (o *GetTrackingDataInner) GetOpenCountOk() (*float32, bool)`

GetOpenCountOk returns a tuple with the OpenCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenCount

`func (o *GetTrackingDataInner) SetOpenCount(v float32)`

SetOpenCount sets OpenCount field to given value.

### HasOpenCount

`func (o *GetTrackingDataInner) HasOpenCount() bool`

HasOpenCount returns a boolean if a field has been set.

### GetDateOpened

`func (o *GetTrackingDataInner) GetDateOpened() float32`

GetDateOpened returns the DateOpened field if non-nil, zero value otherwise.

### GetDateOpenedOk

`func (o *GetTrackingDataInner) GetDateOpenedOk() (*float32, bool)`

GetDateOpenedOk returns a tuple with the DateOpened field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateOpened

`func (o *GetTrackingDataInner) SetDateOpened(v float32)`

SetDateOpened sets DateOpened field to given value.

### HasDateOpened

`func (o *GetTrackingDataInner) HasDateOpened() bool`

HasDateOpened returns a boolean if a field has been set.

### GetUserGeoCountry

`func (o *GetTrackingDataInner) GetUserGeoCountry() string`

GetUserGeoCountry returns the UserGeoCountry field if non-nil, zero value otherwise.

### GetUserGeoCountryOk

`func (o *GetTrackingDataInner) GetUserGeoCountryOk() (*string, bool)`

GetUserGeoCountryOk returns a tuple with the UserGeoCountry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserGeoCountry

`func (o *GetTrackingDataInner) SetUserGeoCountry(v string)`

SetUserGeoCountry sets UserGeoCountry field to given value.

### HasUserGeoCountry

`func (o *GetTrackingDataInner) HasUserGeoCountry() bool`

HasUserGeoCountry returns a boolean if a field has been set.

### GetUserGeoRegion

`func (o *GetTrackingDataInner) GetUserGeoRegion() string`

GetUserGeoRegion returns the UserGeoRegion field if non-nil, zero value otherwise.

### GetUserGeoRegionOk

`func (o *GetTrackingDataInner) GetUserGeoRegionOk() (*string, bool)`

GetUserGeoRegionOk returns a tuple with the UserGeoRegion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserGeoRegion

`func (o *GetTrackingDataInner) SetUserGeoRegion(v string)`

SetUserGeoRegion sets UserGeoRegion field to given value.

### HasUserGeoRegion

`func (o *GetTrackingDataInner) HasUserGeoRegion() bool`

HasUserGeoRegion returns a boolean if a field has been set.

### GetUserDevice

`func (o *GetTrackingDataInner) GetUserDevice() string`

GetUserDevice returns the UserDevice field if non-nil, zero value otherwise.

### GetUserDeviceOk

`func (o *GetTrackingDataInner) GetUserDeviceOk() (*string, bool)`

GetUserDeviceOk returns a tuple with the UserDevice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserDevice

`func (o *GetTrackingDataInner) SetUserDevice(v string)`

SetUserDevice sets UserDevice field to given value.

### HasUserDevice

`func (o *GetTrackingDataInner) HasUserDevice() bool`

HasUserDevice returns a boolean if a field has been set.

### GetUserBrowser

`func (o *GetTrackingDataInner) GetUserBrowser() string`

GetUserBrowser returns the UserBrowser field if non-nil, zero value otherwise.

### GetUserBrowserOk

`func (o *GetTrackingDataInner) GetUserBrowserOk() (*string, bool)`

GetUserBrowserOk returns a tuple with the UserBrowser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserBrowser

`func (o *GetTrackingDataInner) SetUserBrowser(v string)`

SetUserBrowser sets UserBrowser field to given value.

### HasUserBrowser

`func (o *GetTrackingDataInner) HasUserBrowser() bool`

HasUserBrowser returns a boolean if a field has been set.

### GetUserOs

`func (o *GetTrackingDataInner) GetUserOs() string`

GetUserOs returns the UserOs field if non-nil, zero value otherwise.

### GetUserOsOk

`func (o *GetTrackingDataInner) GetUserOsOk() (*string, bool)`

GetUserOsOk returns a tuple with the UserOs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserOs

`func (o *GetTrackingDataInner) SetUserOs(v string)`

SetUserOs sets UserOs field to given value.

### HasUserOs

`func (o *GetTrackingDataInner) HasUserOs() bool`

HasUserOs returns a boolean if a field has been set.

### GetContact

`func (o *GetTrackingDataInner) GetContact() GetTrackingDataInnerContact`

GetContact returns the Contact field if non-nil, zero value otherwise.

### GetContactOk

`func (o *GetTrackingDataInner) GetContactOk() (*GetTrackingDataInnerContact, bool)`

GetContactOk returns a tuple with the Contact field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContact

`func (o *GetTrackingDataInner) SetContact(v GetTrackingDataInnerContact)`

SetContact sets Contact field to given value.

### HasContact

`func (o *GetTrackingDataInner) HasContact() bool`

HasContact returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



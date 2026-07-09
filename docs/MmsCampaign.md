# MmsCampaign

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MmsCampaignId** | Pointer to **int32** | The ID of the MMS campaign. | [optional] 
**Name** | Pointer to **string** | The name of the MMS campaign. | [optional] 
**UserId** | Pointer to **int32** | The ID of the user who created the campaign. | [optional] 
**SubaccountId** | Pointer to **int32** | The ID of the subaccount associated with the campaign. | [optional] 
**ListId** | Pointer to **int32** | The ID of the list associated with the campaign. | [optional] 
**From** | Pointer to **string** | The sender&#39;s phone number or ID. | [optional] 
**Subject** | Pointer to **string** | The subject of the MMS campaign. | [optional] 
**FileName** | Pointer to **string** | The name of the media file attached to the MMS. | [optional] 
**Body** | Pointer to **string** | The body or content of the MMS. | [optional] 
**Schedule** | Pointer to **int32** | The schedule time of the MMS campaign. | [optional] 
**Status** | Pointer to **string** | The status of the MMS campaign. | [optional] 
**DateAdded** | Pointer to **int32** | The date when the campaign was added. | [optional] 
**TotalCount** | Pointer to **int32** | The total count associated with the campaign. | [optional] 
**ListName** | Pointer to **string** | The name of the list associated with the campaign. | [optional] 
**MediaFileUrl** | Pointer to **string** | The URL of the media file attached to the MMS. | [optional] 

## Methods

### NewMmsCampaign

`func NewMmsCampaign() *MmsCampaign`

NewMmsCampaign instantiates a new MmsCampaign object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMmsCampaignWithDefaults

`func NewMmsCampaignWithDefaults() *MmsCampaign`

NewMmsCampaignWithDefaults instantiates a new MmsCampaign object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMmsCampaignId

`func (o *MmsCampaign) GetMmsCampaignId() int32`

GetMmsCampaignId returns the MmsCampaignId field if non-nil, zero value otherwise.

### GetMmsCampaignIdOk

`func (o *MmsCampaign) GetMmsCampaignIdOk() (*int32, bool)`

GetMmsCampaignIdOk returns a tuple with the MmsCampaignId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMmsCampaignId

`func (o *MmsCampaign) SetMmsCampaignId(v int32)`

SetMmsCampaignId sets MmsCampaignId field to given value.

### HasMmsCampaignId

`func (o *MmsCampaign) HasMmsCampaignId() bool`

HasMmsCampaignId returns a boolean if a field has been set.

### GetName

`func (o *MmsCampaign) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *MmsCampaign) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *MmsCampaign) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *MmsCampaign) HasName() bool`

HasName returns a boolean if a field has been set.

### GetUserId

`func (o *MmsCampaign) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *MmsCampaign) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *MmsCampaign) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *MmsCampaign) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *MmsCampaign) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *MmsCampaign) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *MmsCampaign) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *MmsCampaign) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetListId

`func (o *MmsCampaign) GetListId() int32`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *MmsCampaign) GetListIdOk() (*int32, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *MmsCampaign) SetListId(v int32)`

SetListId sets ListId field to given value.

### HasListId

`func (o *MmsCampaign) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetFrom

`func (o *MmsCampaign) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *MmsCampaign) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *MmsCampaign) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *MmsCampaign) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSubject

`func (o *MmsCampaign) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *MmsCampaign) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *MmsCampaign) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *MmsCampaign) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetFileName

`func (o *MmsCampaign) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *MmsCampaign) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *MmsCampaign) SetFileName(v string)`

SetFileName sets FileName field to given value.

### HasFileName

`func (o *MmsCampaign) HasFileName() bool`

HasFileName returns a boolean if a field has been set.

### GetBody

`func (o *MmsCampaign) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *MmsCampaign) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *MmsCampaign) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *MmsCampaign) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetSchedule

`func (o *MmsCampaign) GetSchedule() int32`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *MmsCampaign) GetScheduleOk() (*int32, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *MmsCampaign) SetSchedule(v int32)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *MmsCampaign) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetStatus

`func (o *MmsCampaign) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *MmsCampaign) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *MmsCampaign) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *MmsCampaign) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetDateAdded

`func (o *MmsCampaign) GetDateAdded() int32`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *MmsCampaign) GetDateAddedOk() (*int32, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *MmsCampaign) SetDateAdded(v int32)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *MmsCampaign) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetTotalCount

`func (o *MmsCampaign) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *MmsCampaign) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *MmsCampaign) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *MmsCampaign) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetListName

`func (o *MmsCampaign) GetListName() string`

GetListName returns the ListName field if non-nil, zero value otherwise.

### GetListNameOk

`func (o *MmsCampaign) GetListNameOk() (*string, bool)`

GetListNameOk returns a tuple with the ListName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListName

`func (o *MmsCampaign) SetListName(v string)`

SetListName sets ListName field to given value.

### HasListName

`func (o *MmsCampaign) HasListName() bool`

HasListName returns a boolean if a field has been set.

### GetMediaFileUrl

`func (o *MmsCampaign) GetMediaFileUrl() string`

GetMediaFileUrl returns the MediaFileUrl field if non-nil, zero value otherwise.

### GetMediaFileUrlOk

`func (o *MmsCampaign) GetMediaFileUrlOk() (*string, bool)`

GetMediaFileUrlOk returns a tuple with the MediaFileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMediaFileUrl

`func (o *MmsCampaign) SetMediaFileUrl(v string)`

SetMediaFileUrl sets MediaFileUrl field to given value.

### HasMediaFileUrl

`func (o *MmsCampaign) HasMediaFileUrl() bool`

HasMediaFileUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



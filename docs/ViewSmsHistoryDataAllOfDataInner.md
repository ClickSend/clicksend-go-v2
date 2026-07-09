# ViewSmsHistoryDataAllOfDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Direction** | Pointer to **string** | It can either be in or out:   - **in** - You received a message. it has to do with inbound messages.   - **out** - You are sending a message. It has to do with outbound messages. | [optional] 
**Date** | Pointer to **int32** | The date you sent the message. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**To** | Pointer to **string** | The phone number of the recipient. It should be in &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/E.164\&quot; target&#x3D;\&quot;_blank\&quot;&gt;E.164 format&lt;/a&gt;. | [optional] 
**Body** | Pointer to **string** | The message sent. | [optional] 
**Status** | Pointer to **string** | The status of the SMS. It can either be:  - _Queued_ - _Completed_ - _Scheduled_ - _WaitApproval_ - _Failed_ - _Cancelled_ - _CancelledAfterReview_ - _Received_ - _Sent_  This parameter reflects the actual status of the SMS. It is based on the  status of the SMS sent from the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/SMS_gateway\&quot; target&#x3D;\&quot;_blank\&quot;&gt;SMS gateway&lt;/a&gt;, which is different  from the [API status code](https://developers-dev.clicksend.net/docs/#status-codes). Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. | [optional] 
**From** | Pointer to **string** | The sender of the message. | [optional] 
**Schedule** | Pointer to **int32** | The scheduled date of the message. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**StatusCode** | Pointer to **int32** | The status code sent from the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/SMS_gateway\&quot; target&#x3D;\&quot;_blank\&quot;&gt;SMS gateway&lt;/a&gt;. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. | [optional] 
**StatusText** | Pointer to **string** | A message describing the _status_code_ of the operation. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. | [optional] 
**ErrorCode** | Pointer to **NullableInt32** | The error code of the operation. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. If no error occurred, the value is **null**. | [optional] 
**ErrorText** | Pointer to **NullableString** | A message describing the _error_code_ of the operation. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. If no error occurred, the value is **null**. | [optional] 
**MessageId** | Pointer to **int32** | The generated ID of the message. | [optional] 
**MessageParts** | Pointer to **int32** | The number of parts the message was broken into. To look at how many parts your message is broken down into, use the &lt;a href&#x3D;\&quot;http://smscharactercount.com/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;&lt;strong&gt;SMS Character Count&lt;/strong&gt;&lt;/a&gt;. | [optional] 
**MessagePrice** | Pointer to **float32** | The price of this message. This depends on the total number of parts of the message. | [optional] 
**FromEmail** | Pointer to **string** | The email address to which replies should be emailed to. If omitted, the reply will be emailed back to the user who sent the outgoing SMS | [optional] 
**ListId** | Pointer to **NullableString** | The _list_id_ of the contact list the message was sent to. This parameter will have a **null** value if you didn’t send to a list in the request. | [optional] 
**CustomString** | Pointer to **string** | A note that was included with the outgoing SMS. If no note was included, the value is **null**. | [optional] 
**ContactId** | Pointer to **string** | This is the ID of the contact. This parameter will have a **null** value if you didn’t provide a _contact_id_ in the request. | [optional] 
**UserId** | Pointer to **int32** | The unique user ID of the sender. | [optional] 
**SubaccountId** | Pointer to **int32** | The sub-account of the user. A user can have multiple sub-accounts. | [optional] 
**Country** | Pointer to **string** | The country of the recipient in two-letter format (e.g. US, UK, AU, NZ, etc). | [optional] 
**Carrier** | Pointer to **string** | The phone carrier of the recipient. | [optional] 
**FirstName** | Pointer to **NullableString** | The first name of the recipient. The name will appear if you sent the message to a contact from a contact list. If you are sending directly to a phone number, the value will be **null**. | [optional] 
**LastName** | Pointer to **NullableString** | The last name of the recipient. The name will appear if you sent the message to a contact from a contact list. If you are sending directly to a phone number, the value will be **null**. | [optional] 
**ApiUsername** | Pointer to **string** | The username of the SMS sender. This can be a &lt;a href&#x3D;\&quot;https://dashboard.clicksend.com/account/subaccounts\&quot; target&#x3D;\&quot;_blank\&quot;&gt;sub-account&lt;/a&gt;. | [optional] 

## Methods

### NewViewSmsHistoryDataAllOfDataInner

`func NewViewSmsHistoryDataAllOfDataInner() *ViewSmsHistoryDataAllOfDataInner`

NewViewSmsHistoryDataAllOfDataInner instantiates a new ViewSmsHistoryDataAllOfDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewSmsHistoryDataAllOfDataInnerWithDefaults

`func NewViewSmsHistoryDataAllOfDataInnerWithDefaults() *ViewSmsHistoryDataAllOfDataInner`

NewViewSmsHistoryDataAllOfDataInnerWithDefaults instantiates a new ViewSmsHistoryDataAllOfDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDirection

`func (o *ViewSmsHistoryDataAllOfDataInner) GetDirection() string`

GetDirection returns the Direction field if non-nil, zero value otherwise.

### GetDirectionOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetDirectionOk() (*string, bool)`

GetDirectionOk returns a tuple with the Direction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDirection

`func (o *ViewSmsHistoryDataAllOfDataInner) SetDirection(v string)`

SetDirection sets Direction field to given value.

### HasDirection

`func (o *ViewSmsHistoryDataAllOfDataInner) HasDirection() bool`

HasDirection returns a boolean if a field has been set.

### GetDate

`func (o *ViewSmsHistoryDataAllOfDataInner) GetDate() int32`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetDateOk() (*int32, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *ViewSmsHistoryDataAllOfDataInner) SetDate(v int32)`

SetDate sets Date field to given value.

### HasDate

`func (o *ViewSmsHistoryDataAllOfDataInner) HasDate() bool`

HasDate returns a boolean if a field has been set.

### GetTo

`func (o *ViewSmsHistoryDataAllOfDataInner) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ViewSmsHistoryDataAllOfDataInner) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *ViewSmsHistoryDataAllOfDataInner) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetBody

`func (o *ViewSmsHistoryDataAllOfDataInner) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *ViewSmsHistoryDataAllOfDataInner) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *ViewSmsHistoryDataAllOfDataInner) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetStatus

`func (o *ViewSmsHistoryDataAllOfDataInner) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ViewSmsHistoryDataAllOfDataInner) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *ViewSmsHistoryDataAllOfDataInner) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetFrom

`func (o *ViewSmsHistoryDataAllOfDataInner) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ViewSmsHistoryDataAllOfDataInner) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *ViewSmsHistoryDataAllOfDataInner) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSchedule

`func (o *ViewSmsHistoryDataAllOfDataInner) GetSchedule() int32`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetScheduleOk() (*int32, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *ViewSmsHistoryDataAllOfDataInner) SetSchedule(v int32)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *ViewSmsHistoryDataAllOfDataInner) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetStatusCode

`func (o *ViewSmsHistoryDataAllOfDataInner) GetStatusCode() int32`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetStatusCodeOk() (*int32, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *ViewSmsHistoryDataAllOfDataInner) SetStatusCode(v int32)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *ViewSmsHistoryDataAllOfDataInner) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### GetStatusText

`func (o *ViewSmsHistoryDataAllOfDataInner) GetStatusText() string`

GetStatusText returns the StatusText field if non-nil, zero value otherwise.

### GetStatusTextOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetStatusTextOk() (*string, bool)`

GetStatusTextOk returns a tuple with the StatusText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusText

`func (o *ViewSmsHistoryDataAllOfDataInner) SetStatusText(v string)`

SetStatusText sets StatusText field to given value.

### HasStatusText

`func (o *ViewSmsHistoryDataAllOfDataInner) HasStatusText() bool`

HasStatusText returns a boolean if a field has been set.

### GetErrorCode

`func (o *ViewSmsHistoryDataAllOfDataInner) GetErrorCode() int32`

GetErrorCode returns the ErrorCode field if non-nil, zero value otherwise.

### GetErrorCodeOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetErrorCodeOk() (*int32, bool)`

GetErrorCodeOk returns a tuple with the ErrorCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCode

`func (o *ViewSmsHistoryDataAllOfDataInner) SetErrorCode(v int32)`

SetErrorCode sets ErrorCode field to given value.

### HasErrorCode

`func (o *ViewSmsHistoryDataAllOfDataInner) HasErrorCode() bool`

HasErrorCode returns a boolean if a field has been set.

### SetErrorCodeNil

`func (o *ViewSmsHistoryDataAllOfDataInner) SetErrorCodeNil(b bool)`

 SetErrorCodeNil sets the value for ErrorCode to be an explicit nil

### UnsetErrorCode
`func (o *ViewSmsHistoryDataAllOfDataInner) UnsetErrorCode()`

UnsetErrorCode ensures that no value is present for ErrorCode, not even an explicit nil
### GetErrorText

`func (o *ViewSmsHistoryDataAllOfDataInner) GetErrorText() string`

GetErrorText returns the ErrorText field if non-nil, zero value otherwise.

### GetErrorTextOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetErrorTextOk() (*string, bool)`

GetErrorTextOk returns a tuple with the ErrorText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorText

`func (o *ViewSmsHistoryDataAllOfDataInner) SetErrorText(v string)`

SetErrorText sets ErrorText field to given value.

### HasErrorText

`func (o *ViewSmsHistoryDataAllOfDataInner) HasErrorText() bool`

HasErrorText returns a boolean if a field has been set.

### SetErrorTextNil

`func (o *ViewSmsHistoryDataAllOfDataInner) SetErrorTextNil(b bool)`

 SetErrorTextNil sets the value for ErrorText to be an explicit nil

### UnsetErrorText
`func (o *ViewSmsHistoryDataAllOfDataInner) UnsetErrorText()`

UnsetErrorText ensures that no value is present for ErrorText, not even an explicit nil
### GetMessageId

`func (o *ViewSmsHistoryDataAllOfDataInner) GetMessageId() int32`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetMessageIdOk() (*int32, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *ViewSmsHistoryDataAllOfDataInner) SetMessageId(v int32)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *ViewSmsHistoryDataAllOfDataInner) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetMessageParts

`func (o *ViewSmsHistoryDataAllOfDataInner) GetMessageParts() int32`

GetMessageParts returns the MessageParts field if non-nil, zero value otherwise.

### GetMessagePartsOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetMessagePartsOk() (*int32, bool)`

GetMessagePartsOk returns a tuple with the MessageParts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageParts

`func (o *ViewSmsHistoryDataAllOfDataInner) SetMessageParts(v int32)`

SetMessageParts sets MessageParts field to given value.

### HasMessageParts

`func (o *ViewSmsHistoryDataAllOfDataInner) HasMessageParts() bool`

HasMessageParts returns a boolean if a field has been set.

### GetMessagePrice

`func (o *ViewSmsHistoryDataAllOfDataInner) GetMessagePrice() float32`

GetMessagePrice returns the MessagePrice field if non-nil, zero value otherwise.

### GetMessagePriceOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetMessagePriceOk() (*float32, bool)`

GetMessagePriceOk returns a tuple with the MessagePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagePrice

`func (o *ViewSmsHistoryDataAllOfDataInner) SetMessagePrice(v float32)`

SetMessagePrice sets MessagePrice field to given value.

### HasMessagePrice

`func (o *ViewSmsHistoryDataAllOfDataInner) HasMessagePrice() bool`

HasMessagePrice returns a boolean if a field has been set.

### GetFromEmail

`func (o *ViewSmsHistoryDataAllOfDataInner) GetFromEmail() string`

GetFromEmail returns the FromEmail field if non-nil, zero value otherwise.

### GetFromEmailOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetFromEmailOk() (*string, bool)`

GetFromEmailOk returns a tuple with the FromEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromEmail

`func (o *ViewSmsHistoryDataAllOfDataInner) SetFromEmail(v string)`

SetFromEmail sets FromEmail field to given value.

### HasFromEmail

`func (o *ViewSmsHistoryDataAllOfDataInner) HasFromEmail() bool`

HasFromEmail returns a boolean if a field has been set.

### GetListId

`func (o *ViewSmsHistoryDataAllOfDataInner) GetListId() string`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetListIdOk() (*string, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *ViewSmsHistoryDataAllOfDataInner) SetListId(v string)`

SetListId sets ListId field to given value.

### HasListId

`func (o *ViewSmsHistoryDataAllOfDataInner) HasListId() bool`

HasListId returns a boolean if a field has been set.

### SetListIdNil

`func (o *ViewSmsHistoryDataAllOfDataInner) SetListIdNil(b bool)`

 SetListIdNil sets the value for ListId to be an explicit nil

### UnsetListId
`func (o *ViewSmsHistoryDataAllOfDataInner) UnsetListId()`

UnsetListId ensures that no value is present for ListId, not even an explicit nil
### GetCustomString

`func (o *ViewSmsHistoryDataAllOfDataInner) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *ViewSmsHistoryDataAllOfDataInner) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *ViewSmsHistoryDataAllOfDataInner) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetContactId

`func (o *ViewSmsHistoryDataAllOfDataInner) GetContactId() string`

GetContactId returns the ContactId field if non-nil, zero value otherwise.

### GetContactIdOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetContactIdOk() (*string, bool)`

GetContactIdOk returns a tuple with the ContactId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactId

`func (o *ViewSmsHistoryDataAllOfDataInner) SetContactId(v string)`

SetContactId sets ContactId field to given value.

### HasContactId

`func (o *ViewSmsHistoryDataAllOfDataInner) HasContactId() bool`

HasContactId returns a boolean if a field has been set.

### GetUserId

`func (o *ViewSmsHistoryDataAllOfDataInner) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ViewSmsHistoryDataAllOfDataInner) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ViewSmsHistoryDataAllOfDataInner) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *ViewSmsHistoryDataAllOfDataInner) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *ViewSmsHistoryDataAllOfDataInner) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *ViewSmsHistoryDataAllOfDataInner) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetCountry

`func (o *ViewSmsHistoryDataAllOfDataInner) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ViewSmsHistoryDataAllOfDataInner) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *ViewSmsHistoryDataAllOfDataInner) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetCarrier

`func (o *ViewSmsHistoryDataAllOfDataInner) GetCarrier() string`

GetCarrier returns the Carrier field if non-nil, zero value otherwise.

### GetCarrierOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetCarrierOk() (*string, bool)`

GetCarrierOk returns a tuple with the Carrier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCarrier

`func (o *ViewSmsHistoryDataAllOfDataInner) SetCarrier(v string)`

SetCarrier sets Carrier field to given value.

### HasCarrier

`func (o *ViewSmsHistoryDataAllOfDataInner) HasCarrier() bool`

HasCarrier returns a boolean if a field has been set.

### GetFirstName

`func (o *ViewSmsHistoryDataAllOfDataInner) GetFirstName() string`

GetFirstName returns the FirstName field if non-nil, zero value otherwise.

### GetFirstNameOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetFirstNameOk() (*string, bool)`

GetFirstNameOk returns a tuple with the FirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstName

`func (o *ViewSmsHistoryDataAllOfDataInner) SetFirstName(v string)`

SetFirstName sets FirstName field to given value.

### HasFirstName

`func (o *ViewSmsHistoryDataAllOfDataInner) HasFirstName() bool`

HasFirstName returns a boolean if a field has been set.

### SetFirstNameNil

`func (o *ViewSmsHistoryDataAllOfDataInner) SetFirstNameNil(b bool)`

 SetFirstNameNil sets the value for FirstName to be an explicit nil

### UnsetFirstName
`func (o *ViewSmsHistoryDataAllOfDataInner) UnsetFirstName()`

UnsetFirstName ensures that no value is present for FirstName, not even an explicit nil
### GetLastName

`func (o *ViewSmsHistoryDataAllOfDataInner) GetLastName() string`

GetLastName returns the LastName field if non-nil, zero value otherwise.

### GetLastNameOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetLastNameOk() (*string, bool)`

GetLastNameOk returns a tuple with the LastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastName

`func (o *ViewSmsHistoryDataAllOfDataInner) SetLastName(v string)`

SetLastName sets LastName field to given value.

### HasLastName

`func (o *ViewSmsHistoryDataAllOfDataInner) HasLastName() bool`

HasLastName returns a boolean if a field has been set.

### SetLastNameNil

`func (o *ViewSmsHistoryDataAllOfDataInner) SetLastNameNil(b bool)`

 SetLastNameNil sets the value for LastName to be an explicit nil

### UnsetLastName
`func (o *ViewSmsHistoryDataAllOfDataInner) UnsetLastName()`

UnsetLastName ensures that no value is present for LastName, not even an explicit nil
### GetApiUsername

`func (o *ViewSmsHistoryDataAllOfDataInner) GetApiUsername() string`

GetApiUsername returns the ApiUsername field if non-nil, zero value otherwise.

### GetApiUsernameOk

`func (o *ViewSmsHistoryDataAllOfDataInner) GetApiUsernameOk() (*string, bool)`

GetApiUsernameOk returns a tuple with the ApiUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiUsername

`func (o *ViewSmsHistoryDataAllOfDataInner) SetApiUsername(v string)`

SetApiUsername sets ApiUsername field to given value.

### HasApiUsername

`func (o *ViewSmsHistoryDataAllOfDataInner) HasApiUsername() bool`

HasApiUsername returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



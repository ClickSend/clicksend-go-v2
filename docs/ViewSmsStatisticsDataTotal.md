# ViewSmsStatisticsDataTotal

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Outbound** | Pointer to [**ViewVoiceStatisticsDataStatsInnerOutbound**](ViewVoiceStatisticsDataStatsInnerOutbound.md) |  | [optional] 
**Inbound** | Pointer to [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 
**Bounced** | Pointer to [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 

## Methods

### NewViewSmsStatisticsDataTotal

`func NewViewSmsStatisticsDataTotal() *ViewSmsStatisticsDataTotal`

NewViewSmsStatisticsDataTotal instantiates a new ViewSmsStatisticsDataTotal object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewSmsStatisticsDataTotalWithDefaults

`func NewViewSmsStatisticsDataTotalWithDefaults() *ViewSmsStatisticsDataTotal`

NewViewSmsStatisticsDataTotalWithDefaults instantiates a new ViewSmsStatisticsDataTotal object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOutbound

`func (o *ViewSmsStatisticsDataTotal) GetOutbound() ViewVoiceStatisticsDataStatsInnerOutbound`

GetOutbound returns the Outbound field if non-nil, zero value otherwise.

### GetOutboundOk

`func (o *ViewSmsStatisticsDataTotal) GetOutboundOk() (*ViewVoiceStatisticsDataStatsInnerOutbound, bool)`

GetOutboundOk returns a tuple with the Outbound field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutbound

`func (o *ViewSmsStatisticsDataTotal) SetOutbound(v ViewVoiceStatisticsDataStatsInnerOutbound)`

SetOutbound sets Outbound field to given value.

### HasOutbound

`func (o *ViewSmsStatisticsDataTotal) HasOutbound() bool`

HasOutbound returns a boolean if a field has been set.

### GetInbound

`func (o *ViewSmsStatisticsDataTotal) GetInbound() CancelAllSmsData`

GetInbound returns the Inbound field if non-nil, zero value otherwise.

### GetInboundOk

`func (o *ViewSmsStatisticsDataTotal) GetInboundOk() (*CancelAllSmsData, bool)`

GetInboundOk returns a tuple with the Inbound field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInbound

`func (o *ViewSmsStatisticsDataTotal) SetInbound(v CancelAllSmsData)`

SetInbound sets Inbound field to given value.

### HasInbound

`func (o *ViewSmsStatisticsDataTotal) HasInbound() bool`

HasInbound returns a boolean if a field has been set.

### GetBounced

`func (o *ViewSmsStatisticsDataTotal) GetBounced() CancelAllSmsData`

GetBounced returns the Bounced field if non-nil, zero value otherwise.

### GetBouncedOk

`func (o *ViewSmsStatisticsDataTotal) GetBouncedOk() (*CancelAllSmsData, bool)`

GetBouncedOk returns a tuple with the Bounced field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBounced

`func (o *ViewSmsStatisticsDataTotal) SetBounced(v CancelAllSmsData)`

SetBounced sets Bounced field to given value.

### HasBounced

`func (o *ViewSmsStatisticsDataTotal) HasBounced() bool`

HasBounced returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



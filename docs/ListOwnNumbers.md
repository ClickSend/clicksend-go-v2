# ListOwnNumbers

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OwnNumbers** | Pointer to [**[]OwnNumber**](OwnNumber.md) | The list of own numbers. | [optional] 
**Metadata** | Pointer to [**ListOwnNumbersMetadata**](ListOwnNumbersMetadata.md) |  | [optional] 

## Methods

### NewListOwnNumbers

`func NewListOwnNumbers() *ListOwnNumbers`

NewListOwnNumbers instantiates a new ListOwnNumbers object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListOwnNumbersWithDefaults

`func NewListOwnNumbersWithDefaults() *ListOwnNumbers`

NewListOwnNumbersWithDefaults instantiates a new ListOwnNumbers object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOwnNumbers

`func (o *ListOwnNumbers) GetOwnNumbers() []OwnNumber`

GetOwnNumbers returns the OwnNumbers field if non-nil, zero value otherwise.

### GetOwnNumbersOk

`func (o *ListOwnNumbers) GetOwnNumbersOk() (*[]OwnNumber, bool)`

GetOwnNumbersOk returns a tuple with the OwnNumbers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnNumbers

`func (o *ListOwnNumbers) SetOwnNumbers(v []OwnNumber)`

SetOwnNumbers sets OwnNumbers field to given value.

### HasOwnNumbers

`func (o *ListOwnNumbers) HasOwnNumbers() bool`

HasOwnNumbers returns a boolean if a field has been set.

### GetMetadata

`func (o *ListOwnNumbers) GetMetadata() ListOwnNumbersMetadata`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *ListOwnNumbers) GetMetadataOk() (*ListOwnNumbersMetadata, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *ListOwnNumbers) SetMetadata(v ListOwnNumbersMetadata)`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *ListOwnNumbers) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



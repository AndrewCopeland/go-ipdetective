# IPResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Ip** | **string** |  | 
**Bot** | **bool** |  | 
**Type** | Pointer to **string** |  | [optional] 
**Asn** | Pointer to **int32** |  | [optional] 
**AsnDescription** | Pointer to **string** |  | [optional] 
**CountryCode** | Pointer to **string** |  | [optional] 
**CountryName** | Pointer to **string** |  | [optional] 

## Methods

### NewIPResponse

`func NewIPResponse(ip string, bot bool, ) *IPResponse`

NewIPResponse instantiates a new IPResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIPResponseWithDefaults

`func NewIPResponseWithDefaults() *IPResponse`

NewIPResponseWithDefaults instantiates a new IPResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIp

`func (o *IPResponse) GetIp() string`

GetIp returns the Ip field if non-nil, zero value otherwise.

### GetIpOk

`func (o *IPResponse) GetIpOk() (*string, bool)`

GetIpOk returns a tuple with the Ip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIp

`func (o *IPResponse) SetIp(v string)`

SetIp sets Ip field to given value.


### GetBot

`func (o *IPResponse) GetBot() bool`

GetBot returns the Bot field if non-nil, zero value otherwise.

### GetBotOk

`func (o *IPResponse) GetBotOk() (*bool, bool)`

GetBotOk returns a tuple with the Bot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBot

`func (o *IPResponse) SetBot(v bool)`

SetBot sets Bot field to given value.


### GetType

`func (o *IPResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *IPResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *IPResponse) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *IPResponse) HasType() bool`

HasType returns a boolean if a field has been set.

### GetAsn

`func (o *IPResponse) GetAsn() int32`

GetAsn returns the Asn field if non-nil, zero value otherwise.

### GetAsnOk

`func (o *IPResponse) GetAsnOk() (*int32, bool)`

GetAsnOk returns a tuple with the Asn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsn

`func (o *IPResponse) SetAsn(v int32)`

SetAsn sets Asn field to given value.

### HasAsn

`func (o *IPResponse) HasAsn() bool`

HasAsn returns a boolean if a field has been set.

### GetAsnDescription

`func (o *IPResponse) GetAsnDescription() string`

GetAsnDescription returns the AsnDescription field if non-nil, zero value otherwise.

### GetAsnDescriptionOk

`func (o *IPResponse) GetAsnDescriptionOk() (*string, bool)`

GetAsnDescriptionOk returns a tuple with the AsnDescription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsnDescription

`func (o *IPResponse) SetAsnDescription(v string)`

SetAsnDescription sets AsnDescription field to given value.

### HasAsnDescription

`func (o *IPResponse) HasAsnDescription() bool`

HasAsnDescription returns a boolean if a field has been set.

### GetCountryCode

`func (o *IPResponse) GetCountryCode() string`

GetCountryCode returns the CountryCode field if non-nil, zero value otherwise.

### GetCountryCodeOk

`func (o *IPResponse) GetCountryCodeOk() (*string, bool)`

GetCountryCodeOk returns a tuple with the CountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryCode

`func (o *IPResponse) SetCountryCode(v string)`

SetCountryCode sets CountryCode field to given value.

### HasCountryCode

`func (o *IPResponse) HasCountryCode() bool`

HasCountryCode returns a boolean if a field has been set.

### GetCountryName

`func (o *IPResponse) GetCountryName() string`

GetCountryName returns the CountryName field if non-nil, zero value otherwise.

### GetCountryNameOk

`func (o *IPResponse) GetCountryNameOk() (*string, bool)`

GetCountryNameOk returns a tuple with the CountryName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryName

`func (o *IPResponse) SetCountryName(v string)`

SetCountryName sets CountryName field to given value.

### HasCountryName

`func (o *IPResponse) HasCountryName() bool`

HasCountryName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



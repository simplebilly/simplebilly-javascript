# SimpleBillyApi.VoucherApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createVoucher**](VoucherApi.md#createVoucher) | **POST** /api/v1/vouchers | 
[**deleteVoucher**](VoucherApi.md#deleteVoucher) | **DELETE** /api/v1/vouchers/{voucher_id} | 
[**getVoucher**](VoucherApi.md#getVoucher) | **GET** /api/v1/vouchers/{voucher_id} | 
[**listVouchers**](VoucherApi.md#listVouchers) | **GET** /api/v1/vouchers/ | 
[**updateVoucher**](VoucherApi.md#updateVoucher) | **PUT** /api/v1/vouchers/{voucher_id} | 
[**voucherRestore**](VoucherApi.md#voucherRestore) | **POST** /api/v1/vouchers/{voucher_id}/restore | 



## createVoucher

> Voucher createVoucher(voucherCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.VoucherApi();
let voucherCreate = new SimpleBillyApi.VoucherCreate(); // VoucherCreate | 
apiInstance.createVoucher(voucherCreate, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherCreate** | [**VoucherCreate**](VoucherCreate.md)|  | 

### Return type

[**Voucher**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteVoucher

> deleteVoucher(voucherId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.VoucherApi();
let voucherId = "voucherId_example"; // String | 
apiInstance.deleteVoucher(voucherId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getVoucher

> Voucher getVoucher(voucherId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.VoucherApi();
let voucherId = "voucherId_example"; // String | 
apiInstance.getVoucher(voucherId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherId** | **String**|  | 

### Return type

[**Voucher**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listVouchers

> [Voucher] listVouchers(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.VoucherApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'voucherType': "voucherType_example", // String | 
  'voucherStatus': "voucherStatus_example", // String | 
  'contactName': "contactName_example", // String | 
  'dateFrom': new Date("2013-10-20"), // Date | 
  'dateTo': new Date("2013-10-20") // Date | 
};
apiInstance.listVouchers(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Number**|  | [optional] 
 **pageSize** | **Number**|  | [optional] 
 **voucherType** | **String**|  | [optional] 
 **voucherStatus** | **String**|  | [optional] 
 **contactName** | **String**|  | [optional] 
 **dateFrom** | **Date**|  | [optional] 
 **dateTo** | **Date**|  | [optional] 

### Return type

[**[Voucher]**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateVoucher

> Voucher updateVoucher(voucherId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.VoucherApi();
let voucherId = "voucherId_example"; // String | 
let body = null; // Object | 
apiInstance.updateVoucher(voucherId, body, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**Voucher**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## voucherRestore

> Voucher voucherRestore(voucherId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.VoucherApi();
let voucherId = "voucherId_example"; // String | 
apiInstance.voucherRestore(voucherId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherId** | **String**|  | 

### Return type

[**Voucher**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


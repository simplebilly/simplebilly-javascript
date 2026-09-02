# SimpleBillyApi.GoodsReceiptApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createGoodsReceipt**](GoodsReceiptApi.md#createGoodsReceipt) | **POST** /api/v1/goods-receipts | 
[**deleteGoodsReceipt**](GoodsReceiptApi.md#deleteGoodsReceipt) | **DELETE** /api/v1/goods-receipts/{goods_receipt_id} | 
[**getGoodsReceipt**](GoodsReceiptApi.md#getGoodsReceipt) | **GET** /api/v1/goods-receipts/{goods_receipt_id} | 
[**listGoodsReceipts**](GoodsReceiptApi.md#listGoodsReceipts) | **GET** /api/v1/goods-receipts/ | 



## createGoodsReceipt

> GoodsReceipt createGoodsReceipt(goodsReceipt)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.GoodsReceiptApi();
let goodsReceipt = new SimpleBillyApi.GoodsReceipt(); // GoodsReceipt | 
apiInstance.createGoodsReceipt(goodsReceipt, (error, data, response) => {
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
 **goodsReceipt** | [**GoodsReceipt**](GoodsReceipt.md)|  | 

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteGoodsReceipt

> deleteGoodsReceipt(goodsReceiptId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.GoodsReceiptApi();
let goodsReceiptId = "goodsReceiptId_example"; // String | 
apiInstance.deleteGoodsReceipt(goodsReceiptId, (error, data, response) => {
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
 **goodsReceiptId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getGoodsReceipt

> GoodsReceipt getGoodsReceipt(goodsReceiptId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.GoodsReceiptApi();
let goodsReceiptId = "goodsReceiptId_example"; // String | 
apiInstance.getGoodsReceipt(goodsReceiptId, (error, data, response) => {
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
 **goodsReceiptId** | **String**|  | 

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listGoodsReceipts

> [GoodsReceipt] listGoodsReceipts(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.GoodsReceiptApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'purchaseOrderId': "purchaseOrderId_example", // String | 
  'supplierName': "supplierName_example", // String | 
  'warehouseId': "warehouseId_example" // String | 
};
apiInstance.listGoodsReceipts(opts, (error, data, response) => {
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
 **purchaseOrderId** | **String**|  | [optional] 
 **supplierName** | **String**|  | [optional] 
 **warehouseId** | **String**|  | [optional] 

### Return type

[**[GoodsReceipt]**](GoodsReceipt.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


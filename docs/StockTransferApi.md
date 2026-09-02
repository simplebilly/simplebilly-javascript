# SimpleBillyApi.StockTransferApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createStockTransfer**](StockTransferApi.md#createStockTransfer) | **POST** /api/v1/stock-transfers | 
[**deleteStockTransfer**](StockTransferApi.md#deleteStockTransfer) | **DELETE** /api/v1/stock-transfers/{stock_transfer_id} | 
[**getStockTransfer**](StockTransferApi.md#getStockTransfer) | **GET** /api/v1/stock-transfers/{stock_transfer_id} | 
[**listStockTransfers**](StockTransferApi.md#listStockTransfers) | **GET** /api/v1/stock-transfers/ | 
[**updateStockTransferStatus**](StockTransferApi.md#updateStockTransferStatus) | **PUT** /api/v1/stock-transfers/{stock_transfer_id}/status | 



## createStockTransfer

> StockTransfer createStockTransfer(stockTransfer)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.StockTransferApi();
let stockTransfer = new SimpleBillyApi.StockTransfer(); // StockTransfer | 
apiInstance.createStockTransfer(stockTransfer, (error, data, response) => {
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
 **stockTransfer** | [**StockTransfer**](StockTransfer.md)|  | 

### Return type

[**StockTransfer**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteStockTransfer

> deleteStockTransfer(stockTransferId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.StockTransferApi();
let stockTransferId = "stockTransferId_example"; // String | 
apiInstance.deleteStockTransfer(stockTransferId, (error, data, response) => {
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
 **stockTransferId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getStockTransfer

> StockTransfer getStockTransfer(stockTransferId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.StockTransferApi();
let stockTransferId = "stockTransferId_example"; // String | 
apiInstance.getStockTransfer(stockTransferId, (error, data, response) => {
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
 **stockTransferId** | **String**|  | 

### Return type

[**StockTransfer**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listStockTransfers

> [StockTransfer] listStockTransfers(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.StockTransferApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'status': "status_example", // String | 
  'warehouseId': "warehouseId_example" // String | 
};
apiInstance.listStockTransfers(opts, (error, data, response) => {
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
 **status** | **String**|  | [optional] 
 **warehouseId** | **String**|  | [optional] 

### Return type

[**[StockTransfer]**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateStockTransferStatus

> StockTransfer updateStockTransferStatus(stockTransferId, stockTransferStatusUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.StockTransferApi();
let stockTransferId = "stockTransferId_example"; // String | 
let stockTransferStatusUpdate = new SimpleBillyApi.StockTransferStatusUpdate(); // StockTransferStatusUpdate | 
apiInstance.updateStockTransferStatus(stockTransferId, stockTransferStatusUpdate, (error, data, response) => {
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
 **stockTransferId** | **String**|  | 
 **stockTransferStatusUpdate** | [**StockTransferStatusUpdate**](StockTransferStatusUpdate.md)|  | 

### Return type

[**StockTransfer**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


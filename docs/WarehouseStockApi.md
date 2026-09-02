# SimpleBillyApi.WarehouseStockApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createWarehouseStock**](WarehouseStockApi.md#createWarehouseStock) | **POST** /api/v1/warehouses/{warehouse_id}/stock | 
[**deleteWarehouseStock**](WarehouseStockApi.md#deleteWarehouseStock) | **DELETE** /api/v1/warehouses/{warehouse_id}/stock/{product_id} | 
[**listWarehouseStock**](WarehouseStockApi.md#listWarehouseStock) | **GET** /api/v1/warehouses/{warehouse_id}/stock | 
[**updateWarehouseStock**](WarehouseStockApi.md#updateWarehouseStock) | **PUT** /api/v1/warehouses/{warehouse_id}/stock/{product_id} | 



## createWarehouseStock

> WarehouseStock createWarehouseStock(warehouseId, stockAdjustment)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.WarehouseStockApi();
let warehouseId = "warehouseId_example"; // String | 
let stockAdjustment = new SimpleBillyApi.StockAdjustment(); // StockAdjustment | 
apiInstance.createWarehouseStock(warehouseId, stockAdjustment, (error, data, response) => {
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
 **warehouseId** | **String**|  | 
 **stockAdjustment** | [**StockAdjustment**](StockAdjustment.md)|  | 

### Return type

[**WarehouseStock**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteWarehouseStock

> deleteWarehouseStock(warehouseId, productId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.WarehouseStockApi();
let warehouseId = "warehouseId_example"; // String | 
let productId = "productId_example"; // String | 
apiInstance.deleteWarehouseStock(warehouseId, productId, (error, data, response) => {
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
 **warehouseId** | **String**|  | 
 **productId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listWarehouseStock

> [WarehouseStock] listWarehouseStock(warehouseId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.WarehouseStockApi();
let warehouseId = "warehouseId_example"; // String | 
apiInstance.listWarehouseStock(warehouseId, (error, data, response) => {
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
 **warehouseId** | **String**|  | 

### Return type

[**[WarehouseStock]**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateWarehouseStock

> WarehouseStock updateWarehouseStock(warehouseId, productId, stockAdjustment)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.WarehouseStockApi();
let warehouseId = "warehouseId_example"; // String | 
let productId = "productId_example"; // String | 
let stockAdjustment = new SimpleBillyApi.StockAdjustment(); // StockAdjustment | 
apiInstance.updateWarehouseStock(warehouseId, productId, stockAdjustment, (error, data, response) => {
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
 **warehouseId** | **String**|  | 
 **productId** | **String**|  | 
 **stockAdjustment** | [**StockAdjustment**](StockAdjustment.md)|  | 

### Return type

[**WarehouseStock**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


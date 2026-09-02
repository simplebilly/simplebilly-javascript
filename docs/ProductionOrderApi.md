# SimpleBillyApi.ProductionOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createProductionOrder**](ProductionOrderApi.md#createProductionOrder) | **POST** /api/v1/production-orders | 
[**deleteProductionOrder**](ProductionOrderApi.md#deleteProductionOrder) | **DELETE** /api/v1/production-orders/{production_order_id} | 
[**getProductionOrder**](ProductionOrderApi.md#getProductionOrder) | **GET** /api/v1/production-orders/{production_order_id} | 
[**listProductionOrders**](ProductionOrderApi.md#listProductionOrders) | **GET** /api/v1/production-orders/ | 
[**productionOrderCosting**](ProductionOrderApi.md#productionOrderCosting) | **GET** /api/v1/production-orders/{production_order_id}/costing | Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product&#39;s sale price.
[**updateProductionOrder**](ProductionOrderApi.md#updateProductionOrder) | **PUT** /api/v1/production-orders/{production_order_id} | 
[**updateProductionOrderStatus**](ProductionOrderApi.md#updateProductionOrderStatus) | **PUT** /api/v1/production-orders/{production_order_id}/status | 



## createProductionOrder

> ProductionOrder createProductionOrder(productionOrder)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductionOrderApi();
let productionOrder = new SimpleBillyApi.ProductionOrder(); // ProductionOrder | 
apiInstance.createProductionOrder(productionOrder, (error, data, response) => {
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
 **productionOrder** | [**ProductionOrder**](ProductionOrder.md)|  | 

### Return type

[**ProductionOrder**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProductionOrder

> deleteProductionOrder(productionOrderId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductionOrderApi();
let productionOrderId = "productionOrderId_example"; // String | 
apiInstance.deleteProductionOrder(productionOrderId, (error, data, response) => {
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
 **productionOrderId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProductionOrder

> ProductionOrder getProductionOrder(productionOrderId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductionOrderApi();
let productionOrderId = "productionOrderId_example"; // String | 
apiInstance.getProductionOrder(productionOrderId, (error, data, response) => {
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
 **productionOrderId** | **String**|  | 

### Return type

[**ProductionOrder**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listProductionOrders

> [ProductionOrder] listProductionOrders(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductionOrderApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'search': "search_example", // String | 
  'status': "status_example" // String | Filter by status.
};
apiInstance.listProductionOrders(opts, (error, data, response) => {
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
 **search** | **String**|  | [optional] 
 **status** | **String**| Filter by status. | [optional] 

### Return type

[**[ProductionOrder]**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## productionOrderCosting

> ProductionOrderCosting productionOrderCosting(productionOrderId)

Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product&#39;s sale price.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductionOrderApi();
let productionOrderId = "productionOrderId_example"; // String | 
apiInstance.productionOrderCosting(productionOrderId, (error, data, response) => {
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
 **productionOrderId** | **String**|  | 

### Return type

[**ProductionOrderCosting**](ProductionOrderCosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProductionOrder

> ProductionOrder updateProductionOrder(productionOrderId, productionOrder)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductionOrderApi();
let productionOrderId = "productionOrderId_example"; // String | 
let productionOrder = new SimpleBillyApi.ProductionOrder(); // ProductionOrder | 
apiInstance.updateProductionOrder(productionOrderId, productionOrder, (error, data, response) => {
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
 **productionOrderId** | **String**|  | 
 **productionOrder** | [**ProductionOrder**](ProductionOrder.md)|  | 

### Return type

[**ProductionOrder**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateProductionOrderStatus

> ProductionOrder updateProductionOrderStatus(productionOrderId, productionOrderStatusUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductionOrderApi();
let productionOrderId = "productionOrderId_example"; // String | 
let productionOrderStatusUpdate = new SimpleBillyApi.ProductionOrderStatusUpdate(); // ProductionOrderStatusUpdate | 
apiInstance.updateProductionOrderStatus(productionOrderId, productionOrderStatusUpdate, (error, data, response) => {
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
 **productionOrderId** | **String**|  | 
 **productionOrderStatusUpdate** | [**ProductionOrderStatusUpdate**](ProductionOrderStatusUpdate.md)|  | 

### Return type

[**ProductionOrder**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


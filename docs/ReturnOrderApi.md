# SimpleBillyApi.ReturnOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createReturnOrder**](ReturnOrderApi.md#createReturnOrder) | **POST** /api/v1/returns | 
[**deleteReturnOrder**](ReturnOrderApi.md#deleteReturnOrder) | **DELETE** /api/v1/returns/{return_order_id} | 
[**getReturnOrder**](ReturnOrderApi.md#getReturnOrder) | **GET** /api/v1/returns/{return_order_id} | 
[**listReturnOrders**](ReturnOrderApi.md#listReturnOrders) | **GET** /api/v1/returns/ | 
[**returnLogisticsQueue**](ReturnOrderApi.md#returnLogisticsQueue) | **GET** /api/v1/returns/logistics-queue | 
[**returnLogisticsSummary**](ReturnOrderApi.md#returnLogisticsSummary) | **GET** /api/v1/returns/logistics-summary | Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.
[**updateReturnOrder**](ReturnOrderApi.md#updateReturnOrder) | **PUT** /api/v1/returns/{return_order_id} | 
[**updateReturnOrderStatus**](ReturnOrderApi.md#updateReturnOrderStatus) | **PUT** /api/v1/returns/{return_order_id}/status | 



## createReturnOrder

> ReturnOrder createReturnOrder(returnOrder)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReturnOrderApi();
let returnOrder = new SimpleBillyApi.ReturnOrder(); // ReturnOrder | 
apiInstance.createReturnOrder(returnOrder, (error, data, response) => {
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
 **returnOrder** | [**ReturnOrder**](ReturnOrder.md)|  | 

### Return type

[**ReturnOrder**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteReturnOrder

> deleteReturnOrder(returnOrderId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReturnOrderApi();
let returnOrderId = "returnOrderId_example"; // String | 
apiInstance.deleteReturnOrder(returnOrderId, (error, data, response) => {
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
 **returnOrderId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getReturnOrder

> ReturnOrder getReturnOrder(returnOrderId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReturnOrderApi();
let returnOrderId = "returnOrderId_example"; // String | 
apiInstance.getReturnOrder(returnOrderId, (error, data, response) => {
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
 **returnOrderId** | **String**|  | 

### Return type

[**ReturnOrder**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listReturnOrders

> [ReturnOrder] listReturnOrders(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReturnOrderApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'status': "status_example", // String | 
  'customerName': "customerName_example", // String | 
  'orderNumber': "orderNumber_example" // String | 
};
apiInstance.listReturnOrders(opts, (error, data, response) => {
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
 **customerName** | **String**|  | [optional] 
 **orderNumber** | **String**|  | [optional] 

### Return type

[**[ReturnOrder]**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## returnLogisticsQueue

> [ReturnLogisticsQueueItem] returnLogisticsQueue()



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReturnOrderApi();
apiInstance.returnLogisticsQueue((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**[ReturnLogisticsQueueItem]**](ReturnLogisticsQueueItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## returnLogisticsSummary

> ReturnLogisticsSummary returnLogisticsSummary()

Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReturnOrderApi();
apiInstance.returnLogisticsSummary((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ReturnLogisticsSummary**](ReturnLogisticsSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateReturnOrder

> ReturnOrder updateReturnOrder(returnOrderId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReturnOrderApi();
let returnOrderId = "returnOrderId_example"; // String | 
let body = null; // Object | 
apiInstance.updateReturnOrder(returnOrderId, body, (error, data, response) => {
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
 **returnOrderId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**ReturnOrder**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateReturnOrderStatus

> ReturnOrder updateReturnOrderStatus(returnOrderId, returnOrderStatusUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReturnOrderApi();
let returnOrderId = "returnOrderId_example"; // String | 
let returnOrderStatusUpdate = new SimpleBillyApi.ReturnOrderStatusUpdate(); // ReturnOrderStatusUpdate | 
apiInstance.updateReturnOrderStatus(returnOrderId, returnOrderStatusUpdate, (error, data, response) => {
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
 **returnOrderId** | **String**|  | 
 **returnOrderStatusUpdate** | [**ReturnOrderStatusUpdate**](ReturnOrderStatusUpdate.md)|  | 

### Return type

[**ReturnOrder**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


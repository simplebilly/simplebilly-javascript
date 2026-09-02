# SimpleBillyApi.PurchaseOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPurchaseOrder**](PurchaseOrderApi.md#createPurchaseOrder) | **POST** /api/v1/purchase-orders | 
[**deletePurchaseOrder**](PurchaseOrderApi.md#deletePurchaseOrder) | **DELETE** /api/v1/purchase-orders/{purchase_order_id} | 
[**getPurchaseOrder**](PurchaseOrderApi.md#getPurchaseOrder) | **GET** /api/v1/purchase-orders/{purchase_order_id} | 
[**listPurchaseOrders**](PurchaseOrderApi.md#listPurchaseOrders) | **GET** /api/v1/purchase-orders/ | 
[**matchInvoice**](PurchaseOrderApi.md#matchInvoice) | **POST** /api/v1/purchase-orders/{purchase_order_id}/match-invoice | 3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.
[**updatePurchaseOrder**](PurchaseOrderApi.md#updatePurchaseOrder) | **PUT** /api/v1/purchase-orders/{purchase_order_id} | 
[**updatePurchaseOrderStatus**](PurchaseOrderApi.md#updatePurchaseOrderStatus) | **PUT** /api/v1/purchase-orders/{purchase_order_id}/status | 



## createPurchaseOrder

> PurchaseOrder createPurchaseOrder(purchaseOrder)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PurchaseOrderApi();
let purchaseOrder = new SimpleBillyApi.PurchaseOrder(); // PurchaseOrder | 
apiInstance.createPurchaseOrder(purchaseOrder, (error, data, response) => {
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
 **purchaseOrder** | [**PurchaseOrder**](PurchaseOrder.md)|  | 

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletePurchaseOrder

> deletePurchaseOrder(purchaseOrderId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PurchaseOrderApi();
let purchaseOrderId = "purchaseOrderId_example"; // String | 
apiInstance.deletePurchaseOrder(purchaseOrderId, (error, data, response) => {
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
 **purchaseOrderId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPurchaseOrder

> PurchaseOrder getPurchaseOrder(purchaseOrderId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PurchaseOrderApi();
let purchaseOrderId = "purchaseOrderId_example"; // String | 
apiInstance.getPurchaseOrder(purchaseOrderId, (error, data, response) => {
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
 **purchaseOrderId** | **String**|  | 

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPurchaseOrders

> [PurchaseOrder] listPurchaseOrders(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PurchaseOrderApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'status': "status_example", // String | 
  'supplierName': "supplierName_example", // String | 
  'search': "search_example" // String | 
};
apiInstance.listPurchaseOrders(opts, (error, data, response) => {
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
 **supplierName** | **String**|  | [optional] 
 **search** | **String**|  | [optional] 

### Return type

[**[PurchaseOrder]**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## matchInvoice

> Object matchInvoice(purchaseOrderId, invoiceMatchRequest)

3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PurchaseOrderApi();
let purchaseOrderId = "purchaseOrderId_example"; // String | 
let invoiceMatchRequest = new SimpleBillyApi.InvoiceMatchRequest(); // InvoiceMatchRequest | 
apiInstance.matchInvoice(purchaseOrderId, invoiceMatchRequest, (error, data, response) => {
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
 **purchaseOrderId** | **String**|  | 
 **invoiceMatchRequest** | [**InvoiceMatchRequest**](InvoiceMatchRequest.md)|  | 

### Return type

**Object**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updatePurchaseOrder

> PurchaseOrder updatePurchaseOrder(purchaseOrderId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PurchaseOrderApi();
let purchaseOrderId = "purchaseOrderId_example"; // String | 
let body = null; // Object | 
apiInstance.updatePurchaseOrder(purchaseOrderId, body, (error, data, response) => {
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
 **purchaseOrderId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updatePurchaseOrderStatus

> PurchaseOrder updatePurchaseOrderStatus(purchaseOrderId, purchaseOrderStatusUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PurchaseOrderApi();
let purchaseOrderId = "purchaseOrderId_example"; // String | 
let purchaseOrderStatusUpdate = new SimpleBillyApi.PurchaseOrderStatusUpdate(); // PurchaseOrderStatusUpdate | 
apiInstance.updatePurchaseOrderStatus(purchaseOrderId, purchaseOrderStatusUpdate, (error, data, response) => {
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
 **purchaseOrderId** | **String**|  | 
 **purchaseOrderStatusUpdate** | [**PurchaseOrderStatusUpdate**](PurchaseOrderStatusUpdate.md)|  | 

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


# SimpleBillyApi.SupplierInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSupplierInvoice**](SupplierInvoiceApi.md#createSupplierInvoice) | **POST** /api/v1/supplier-invoices | 
[**deleteSupplierInvoice**](SupplierInvoiceApi.md#deleteSupplierInvoice) | **DELETE** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**getSupplierInvoice**](SupplierInvoiceApi.md#getSupplierInvoice) | **GET** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**listSupplierInvoices**](SupplierInvoiceApi.md#listSupplierInvoices) | **GET** /api/v1/supplier-invoices/ | 
[**updateSupplierInvoice**](SupplierInvoiceApi.md#updateSupplierInvoice) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**updateSupplierInvoiceStatus**](SupplierInvoiceApi.md#updateSupplierInvoiceStatus) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id}/status | 



## createSupplierInvoice

> SupplierInvoice createSupplierInvoice(supplierInvoice)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierInvoiceApi();
let supplierInvoice = new SimpleBillyApi.SupplierInvoice(); // SupplierInvoice | 
apiInstance.createSupplierInvoice(supplierInvoice, (error, data, response) => {
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
 **supplierInvoice** | [**SupplierInvoice**](SupplierInvoice.md)|  | 

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteSupplierInvoice

> deleteSupplierInvoice(supplierInvoiceId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierInvoiceApi();
let supplierInvoiceId = "supplierInvoiceId_example"; // String | 
apiInstance.deleteSupplierInvoice(supplierInvoiceId, (error, data, response) => {
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
 **supplierInvoiceId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getSupplierInvoice

> SupplierInvoice getSupplierInvoice(supplierInvoiceId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierInvoiceApi();
let supplierInvoiceId = "supplierInvoiceId_example"; // String | 
apiInstance.getSupplierInvoice(supplierInvoiceId, (error, data, response) => {
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
 **supplierInvoiceId** | **String**|  | 

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listSupplierInvoices

> [SupplierInvoice] listSupplierInvoices(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierInvoiceApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'status': "status_example", // String | 
  'purchaseOrderId': "purchaseOrderId_example", // String | 
  'supplierName': "supplierName_example" // String | 
};
apiInstance.listSupplierInvoices(opts, (error, data, response) => {
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
 **purchaseOrderId** | **String**|  | [optional] 
 **supplierName** | **String**|  | [optional] 

### Return type

[**[SupplierInvoice]**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateSupplierInvoice

> SupplierInvoice updateSupplierInvoice(supplierInvoiceId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierInvoiceApi();
let supplierInvoiceId = "supplierInvoiceId_example"; // String | 
let body = null; // Object | 
apiInstance.updateSupplierInvoice(supplierInvoiceId, body, (error, data, response) => {
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
 **supplierInvoiceId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateSupplierInvoiceStatus

> SupplierInvoice updateSupplierInvoiceStatus(supplierInvoiceId, supplierInvoiceStatusUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierInvoiceApi();
let supplierInvoiceId = "supplierInvoiceId_example"; // String | 
let supplierInvoiceStatusUpdate = new SimpleBillyApi.SupplierInvoiceStatusUpdate(); // SupplierInvoiceStatusUpdate | 
apiInstance.updateSupplierInvoiceStatus(supplierInvoiceId, supplierInvoiceStatusUpdate, (error, data, response) => {
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
 **supplierInvoiceId** | **String**|  | 
 **supplierInvoiceStatusUpdate** | [**SupplierInvoiceStatusUpdate**](SupplierInvoiceStatusUpdate.md)|  | 

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


# SimpleBillyApi.ProformaInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**convertProformaToInvoice**](ProformaInvoiceApi.md#convertProformaToInvoice) | **POST** /api/v1/proforma-invoices/{proforma_id}/convert | 
[**createProformaInvoice**](ProformaInvoiceApi.md#createProformaInvoice) | **POST** /api/v1/proforma-invoices | 
[**deleteProformaInvoice**](ProformaInvoiceApi.md#deleteProformaInvoice) | **DELETE** /api/v1/proforma-invoices/{proforma_id} | 
[**getProformaInvoice**](ProformaInvoiceApi.md#getProformaInvoice) | **GET** /api/v1/proforma-invoices/{proforma_id} | 
[**listProformaInvoices**](ProformaInvoiceApi.md#listProformaInvoices) | **GET** /api/v1/proforma-invoices/ | 
[**updateProformaInvoice**](ProformaInvoiceApi.md#updateProformaInvoice) | **PUT** /api/v1/proforma-invoices/{proforma_id} | 



## convertProformaToInvoice

> ConvertResponse convertProformaToInvoice(proformaId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProformaInvoiceApi();
let proformaId = "proformaId_example"; // String | 
apiInstance.convertProformaToInvoice(proformaId, (error, data, response) => {
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
 **proformaId** | **String**|  | 

### Return type

[**ConvertResponse**](ConvertResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## createProformaInvoice

> ProformaInvoice createProformaInvoice(proformaInvoice)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProformaInvoiceApi();
let proformaInvoice = new SimpleBillyApi.ProformaInvoice(); // ProformaInvoice | 
apiInstance.createProformaInvoice(proformaInvoice, (error, data, response) => {
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
 **proformaInvoice** | [**ProformaInvoice**](ProformaInvoice.md)|  | 

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProformaInvoice

> deleteProformaInvoice(proformaId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProformaInvoiceApi();
let proformaId = "proformaId_example"; // String | 
apiInstance.deleteProformaInvoice(proformaId, (error, data, response) => {
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
 **proformaId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProformaInvoice

> ProformaInvoice getProformaInvoice(proformaId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProformaInvoiceApi();
let proformaId = "proformaId_example"; // String | 
apiInstance.getProformaInvoice(proformaId, (error, data, response) => {
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
 **proformaId** | **String**|  | 

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listProformaInvoices

> [ProformaInvoice] listProformaInvoices(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProformaInvoiceApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'status': "status_example", // String | 
  'customerId': "customerId_example", // String | 
  'orderNumber': "orderNumber_example" // String | 
};
apiInstance.listProformaInvoices(opts, (error, data, response) => {
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
 **customerId** | **String**|  | [optional] 
 **orderNumber** | **String**|  | [optional] 

### Return type

[**[ProformaInvoice]**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProformaInvoice

> ProformaInvoice updateProformaInvoice(proformaId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProformaInvoiceApi();
let proformaId = "proformaId_example"; // String | 
let body = null; // Object | 
apiInstance.updateProformaInvoice(proformaId, body, (error, data, response) => {
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
 **proformaId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


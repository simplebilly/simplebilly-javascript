# SimpleBillyApi.InventoryCountApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createInventoryCount**](InventoryCountApi.md#createInventoryCount) | **POST** /api/v1/inventory-counts | 
[**deleteInventoryCount**](InventoryCountApi.md#deleteInventoryCount) | **DELETE** /api/v1/inventory-counts/{inventory_count_id} | 
[**generateInventoryCount**](InventoryCountApi.md#generateInventoryCount) | **POST** /api/v1/inventory-counts/generate | 
[**getInventoryCount**](InventoryCountApi.md#getInventoryCount) | **GET** /api/v1/inventory-counts/{inventory_count_id} | 
[**listInventoryCounts**](InventoryCountApi.md#listInventoryCounts) | **GET** /api/v1/inventory-counts/ | 
[**updateInventoryCount**](InventoryCountApi.md#updateInventoryCount) | **PUT** /api/v1/inventory-counts/{inventory_count_id} | 
[**updateInventoryCountStatus**](InventoryCountApi.md#updateInventoryCountStatus) | **PUT** /api/v1/inventory-counts/{inventory_count_id}/status | 



## createInventoryCount

> InventoryCount createInventoryCount(inventoryCount)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.InventoryCountApi();
let inventoryCount = new SimpleBillyApi.InventoryCount(); // InventoryCount | 
apiInstance.createInventoryCount(inventoryCount, (error, data, response) => {
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
 **inventoryCount** | [**InventoryCount**](InventoryCount.md)|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteInventoryCount

> deleteInventoryCount(inventoryCountId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.InventoryCountApi();
let inventoryCountId = "inventoryCountId_example"; // String | 
apiInstance.deleteInventoryCount(inventoryCountId, (error, data, response) => {
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
 **inventoryCountId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## generateInventoryCount

> InventoryCount generateInventoryCount(generateCountRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.InventoryCountApi();
let generateCountRequest = new SimpleBillyApi.GenerateCountRequest(); // GenerateCountRequest | 
apiInstance.generateInventoryCount(generateCountRequest, (error, data, response) => {
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
 **generateCountRequest** | [**GenerateCountRequest**](GenerateCountRequest.md)|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## getInventoryCount

> InventoryCount getInventoryCount(inventoryCountId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.InventoryCountApi();
let inventoryCountId = "inventoryCountId_example"; // String | 
apiInstance.getInventoryCount(inventoryCountId, (error, data, response) => {
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
 **inventoryCountId** | **String**|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listInventoryCounts

> [InventoryCount] listInventoryCounts(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.InventoryCountApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'status': "status_example", // String | 
  'warehouseId': "warehouseId_example" // String | 
};
apiInstance.listInventoryCounts(opts, (error, data, response) => {
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

[**[InventoryCount]**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateInventoryCount

> InventoryCount updateInventoryCount(inventoryCountId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.InventoryCountApi();
let inventoryCountId = "inventoryCountId_example"; // String | 
let body = null; // Object | 
apiInstance.updateInventoryCount(inventoryCountId, body, (error, data, response) => {
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
 **inventoryCountId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateInventoryCountStatus

> InventoryCount updateInventoryCountStatus(inventoryCountId, inventoryCountStatusUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.InventoryCountApi();
let inventoryCountId = "inventoryCountId_example"; // String | 
let inventoryCountStatusUpdate = new SimpleBillyApi.InventoryCountStatusUpdate(); // InventoryCountStatusUpdate | 
apiInstance.updateInventoryCountStatus(inventoryCountId, inventoryCountStatusUpdate, (error, data, response) => {
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
 **inventoryCountId** | **String**|  | 
 **inventoryCountStatusUpdate** | [**InventoryCountStatusUpdate**](InventoryCountStatusUpdate.md)|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


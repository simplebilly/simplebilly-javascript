# SimpleBillyApi.SupplierConditionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSupplierCondition**](SupplierConditionApi.md#createSupplierCondition) | **POST** /api/v1/supplier-conditions | 
[**deleteSupplierCondition**](SupplierConditionApi.md#deleteSupplierCondition) | **DELETE** /api/v1/supplier-conditions/{supplier_condition_id} | 
[**getSupplierCondition**](SupplierConditionApi.md#getSupplierCondition) | **GET** /api/v1/supplier-conditions/{supplier_condition_id} | 
[**listSupplierConditions**](SupplierConditionApi.md#listSupplierConditions) | **GET** /api/v1/supplier-conditions/ | 
[**updateSupplierCondition**](SupplierConditionApi.md#updateSupplierCondition) | **PUT** /api/v1/supplier-conditions/{supplier_condition_id} | 



## createSupplierCondition

> SupplierCondition createSupplierCondition(supplierConditionCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierConditionApi();
let supplierConditionCreate = new SimpleBillyApi.SupplierConditionCreate(); // SupplierConditionCreate | 
apiInstance.createSupplierCondition(supplierConditionCreate, (error, data, response) => {
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
 **supplierConditionCreate** | [**SupplierConditionCreate**](SupplierConditionCreate.md)|  | 

### Return type

[**SupplierCondition**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteSupplierCondition

> deleteSupplierCondition(supplierConditionId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierConditionApi();
let supplierConditionId = "supplierConditionId_example"; // String | 
apiInstance.deleteSupplierCondition(supplierConditionId, (error, data, response) => {
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
 **supplierConditionId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getSupplierCondition

> SupplierCondition getSupplierCondition(supplierConditionId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierConditionApi();
let supplierConditionId = "supplierConditionId_example"; // String | 
apiInstance.getSupplierCondition(supplierConditionId, (error, data, response) => {
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
 **supplierConditionId** | **String**|  | 

### Return type

[**SupplierCondition**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listSupplierConditions

> [SupplierCondition] listSupplierConditions(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierConditionApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'supplierContactId': "supplierContactId_example", // String | 
  'search': "search_example" // String | 
};
apiInstance.listSupplierConditions(opts, (error, data, response) => {
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
 **supplierContactId** | **String**|  | [optional] 
 **search** | **String**|  | [optional] 

### Return type

[**[SupplierCondition]**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateSupplierCondition

> SupplierCondition updateSupplierCondition(supplierConditionId, supplierConditionUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupplierConditionApi();
let supplierConditionId = "supplierConditionId_example"; // String | 
let supplierConditionUpdate = new SimpleBillyApi.SupplierConditionUpdate(); // SupplierConditionUpdate | 
apiInstance.updateSupplierCondition(supplierConditionId, supplierConditionUpdate, (error, data, response) => {
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
 **supplierConditionId** | **String**|  | 
 **supplierConditionUpdate** | [**SupplierConditionUpdate**](SupplierConditionUpdate.md)|  | 

### Return type

[**SupplierCondition**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


# SimpleBillyApi.ProductAttributeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createProductAttribute**](ProductAttributeApi.md#createProductAttribute) | **POST** /api/v1/product-attributes | 
[**deleteProductAttribute**](ProductAttributeApi.md#deleteProductAttribute) | **DELETE** /api/v1/product-attributes/{attribute_id} | 
[**getProductAttribute**](ProductAttributeApi.md#getProductAttribute) | **GET** /api/v1/product-attributes/{attribute_id} | 
[**listProductAttributes**](ProductAttributeApi.md#listProductAttributes) | **GET** /api/v1/product-attributes/ | 
[**updateProductAttribute**](ProductAttributeApi.md#updateProductAttribute) | **PUT** /api/v1/product-attributes/{attribute_id} | 



## createProductAttribute

> ProductAttribute createProductAttribute(productAttributeCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductAttributeApi();
let productAttributeCreate = new SimpleBillyApi.ProductAttributeCreate(); // ProductAttributeCreate | 
apiInstance.createProductAttribute(productAttributeCreate, (error, data, response) => {
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
 **productAttributeCreate** | [**ProductAttributeCreate**](ProductAttributeCreate.md)|  | 

### Return type

[**ProductAttribute**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProductAttribute

> deleteProductAttribute(attributeId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductAttributeApi();
let attributeId = "attributeId_example"; // String | 
apiInstance.deleteProductAttribute(attributeId, (error, data, response) => {
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
 **attributeId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProductAttribute

> ProductAttribute getProductAttribute(attributeId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductAttributeApi();
let attributeId = "attributeId_example"; // String | 
apiInstance.getProductAttribute(attributeId, (error, data, response) => {
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
 **attributeId** | **String**|  | 

### Return type

[**ProductAttribute**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listProductAttributes

> [ProductAttribute] listProductAttributes(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductAttributeApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'productId': "productId_example", // String | 
  'isFilterable': true, // Boolean | 
  'search': "search_example" // String | 
};
apiInstance.listProductAttributes(opts, (error, data, response) => {
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
 **productId** | **String**|  | [optional] 
 **isFilterable** | **Boolean**|  | [optional] 
 **search** | **String**|  | [optional] 

### Return type

[**[ProductAttribute]**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProductAttribute

> ProductAttribute updateProductAttribute(attributeId, productAttributeUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductAttributeApi();
let attributeId = "attributeId_example"; // String | 
let productAttributeUpdate = new SimpleBillyApi.ProductAttributeUpdate(); // ProductAttributeUpdate | 
apiInstance.updateProductAttribute(attributeId, productAttributeUpdate, (error, data, response) => {
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
 **attributeId** | **String**|  | 
 **productAttributeUpdate** | [**ProductAttributeUpdate**](ProductAttributeUpdate.md)|  | 

### Return type

[**ProductAttribute**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


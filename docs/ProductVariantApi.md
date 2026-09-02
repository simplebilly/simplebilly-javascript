# SimpleBillyApi.ProductVariantApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createProductVariant**](ProductVariantApi.md#createProductVariant) | **POST** /api/v1/product-variants | 
[**deleteProductVariant**](ProductVariantApi.md#deleteProductVariant) | **DELETE** /api/v1/product-variants/{variant_id} | 
[**generateProductVariants**](ProductVariantApi.md#generateProductVariants) | **POST** /api/v1/product-variants/generate | 
[**getProductVariant**](ProductVariantApi.md#getProductVariant) | **GET** /api/v1/product-variants/{variant_id} | 
[**listProductVariants**](ProductVariantApi.md#listProductVariants) | **GET** /api/v1/product-variants/ | 
[**updateProductVariant**](ProductVariantApi.md#updateProductVariant) | **PUT** /api/v1/product-variants/{variant_id} | 



## createProductVariant

> ProductVariant createProductVariant(productVariant)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductVariantApi();
let productVariant = new SimpleBillyApi.ProductVariant(); // ProductVariant | 
apiInstance.createProductVariant(productVariant, (error, data, response) => {
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
 **productVariant** | [**ProductVariant**](ProductVariant.md)|  | 

### Return type

[**ProductVariant**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProductVariant

> deleteProductVariant(variantId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductVariantApi();
let variantId = "variantId_example"; // String | 
apiInstance.deleteProductVariant(variantId, (error, data, response) => {
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
 **variantId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## generateProductVariants

> [ProductVariant] generateProductVariants(generateVariantsRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductVariantApi();
let generateVariantsRequest = new SimpleBillyApi.GenerateVariantsRequest(); // GenerateVariantsRequest | 
apiInstance.generateProductVariants(generateVariantsRequest, (error, data, response) => {
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
 **generateVariantsRequest** | [**GenerateVariantsRequest**](GenerateVariantsRequest.md)|  | 

### Return type

[**[ProductVariant]**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## getProductVariant

> ProductVariant getProductVariant(variantId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductVariantApi();
let variantId = "variantId_example"; // String | 
apiInstance.getProductVariant(variantId, (error, data, response) => {
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
 **variantId** | **String**|  | 

### Return type

[**ProductVariant**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listProductVariants

> [ProductVariant] listProductVariants(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductVariantApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'productId': "productId_example", // String | 
  'isActive': true // Boolean | 
};
apiInstance.listProductVariants(opts, (error, data, response) => {
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
 **isActive** | **Boolean**|  | [optional] 

### Return type

[**[ProductVariant]**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProductVariant

> ProductVariant updateProductVariant(variantId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProductVariantApi();
let variantId = "variantId_example"; // String | 
let body = null; // Object | 
apiInstance.updateProductVariant(variantId, body, (error, data, response) => {
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
 **variantId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**ProductVariant**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


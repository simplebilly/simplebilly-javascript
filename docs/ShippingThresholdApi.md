# SimpleBillyApi.ShippingThresholdApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createShippingThreshold**](ShippingThresholdApi.md#createShippingThreshold) | **POST** /api/v1/shipping-thresholds | 
[**deleteShippingThreshold**](ShippingThresholdApi.md#deleteShippingThreshold) | **DELETE** /api/v1/shipping-thresholds/{threshold_id} | 
[**getDeliverable**](ShippingThresholdApi.md#getDeliverable) | **GET** /api/v1/shipping-thresholds/deliverable | 
[**getShippingThreshold**](ShippingThresholdApi.md#getShippingThreshold) | **GET** /api/v1/shipping-thresholds/{threshold_id} | 
[**listShippingThresholds**](ShippingThresholdApi.md#listShippingThresholds) | **GET** /api/v1/shipping-thresholds/ | 
[**updateShippingThreshold**](ShippingThresholdApi.md#updateShippingThreshold) | **PUT** /api/v1/shipping-thresholds/{threshold_id} | 



## createShippingThreshold

> ShippingThreshold createShippingThreshold(shippingThresholdCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingThresholdApi();
let shippingThresholdCreate = new SimpleBillyApi.ShippingThresholdCreate(); // ShippingThresholdCreate | 
apiInstance.createShippingThreshold(shippingThresholdCreate, (error, data, response) => {
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
 **shippingThresholdCreate** | [**ShippingThresholdCreate**](ShippingThresholdCreate.md)|  | 

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteShippingThreshold

> deleteShippingThreshold(thresholdId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingThresholdApi();
let thresholdId = "thresholdId_example"; // String | 
apiInstance.deleteShippingThreshold(thresholdId, (error, data, response) => {
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
 **thresholdId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDeliverable

> DeliverableResponse getDeliverable(productId, opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingThresholdApi();
let productId = "productId_example"; // String | 
let opts = {
  'warehouseId': "warehouseId_example" // String | 
};
apiInstance.getDeliverable(productId, opts, (error, data, response) => {
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
 **productId** | **String**|  | 
 **warehouseId** | **String**|  | [optional] 

### Return type

[**DeliverableResponse**](DeliverableResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getShippingThreshold

> ShippingThreshold getShippingThreshold(thresholdId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingThresholdApi();
let thresholdId = "thresholdId_example"; // String | 
apiInstance.getShippingThreshold(thresholdId, (error, data, response) => {
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
 **thresholdId** | **String**|  | 

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listShippingThresholds

> [ShippingThreshold] listShippingThresholds(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingThresholdApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'productId': "productId_example", // String | 
  'warehouseId': "warehouseId_example", // String | 
  'isActive': true // Boolean | 
};
apiInstance.listShippingThresholds(opts, (error, data, response) => {
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
 **warehouseId** | **String**|  | [optional] 
 **isActive** | **Boolean**|  | [optional] 

### Return type

[**[ShippingThreshold]**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateShippingThreshold

> ShippingThreshold updateShippingThreshold(thresholdId, shippingThresholdUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingThresholdApi();
let thresholdId = "thresholdId_example"; // String | 
let shippingThresholdUpdate = new SimpleBillyApi.ShippingThresholdUpdate(); // ShippingThresholdUpdate | 
apiInstance.updateShippingThreshold(thresholdId, shippingThresholdUpdate, (error, data, response) => {
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
 **thresholdId** | **String**|  | 
 **shippingThresholdUpdate** | [**ShippingThresholdUpdate**](ShippingThresholdUpdate.md)|  | 

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


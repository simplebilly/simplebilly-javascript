# SimpleBillyApi.PriceTierApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPriceTier**](PriceTierApi.md#createPriceTier) | **POST** /api/v1/price-tiers | 
[**deletePriceTier**](PriceTierApi.md#deletePriceTier) | **DELETE** /api/v1/price-tiers/{price_tier_id} | 
[**getPriceTier**](PriceTierApi.md#getPriceTier) | **GET** /api/v1/price-tiers/{price_tier_id} | 
[**getResolvedPrice**](PriceTierApi.md#getResolvedPrice) | **GET** /api/v1/price-tiers/resolved | 
[**listPriceTiers**](PriceTierApi.md#listPriceTiers) | **GET** /api/v1/price-tiers/ | 
[**updatePriceTier**](PriceTierApi.md#updatePriceTier) | **PUT** /api/v1/price-tiers/{price_tier_id} | 



## createPriceTier

> PriceTier createPriceTier(priceTierCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PriceTierApi();
let priceTierCreate = new SimpleBillyApi.PriceTierCreate(); // PriceTierCreate | 
apiInstance.createPriceTier(priceTierCreate, (error, data, response) => {
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
 **priceTierCreate** | [**PriceTierCreate**](PriceTierCreate.md)|  | 

### Return type

[**PriceTier**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletePriceTier

> deletePriceTier(priceTierId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PriceTierApi();
let priceTierId = "priceTierId_example"; // String | 
apiInstance.deletePriceTier(priceTierId, (error, data, response) => {
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
 **priceTierId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPriceTier

> PriceTier getPriceTier(priceTierId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PriceTierApi();
let priceTierId = "priceTierId_example"; // String | 
apiInstance.getPriceTier(priceTierId, (error, data, response) => {
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
 **priceTierId** | **String**|  | 

### Return type

[**PriceTier**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getResolvedPrice

> ResolvedPriceResponse getResolvedPrice(productId, opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PriceTierApi();
let productId = "productId_example"; // String | 
let opts = {
  'quantity': 789, // Number | 
  'contactId': "contactId_example" // String | Contact used to match customer-group-scoped tiers.
};
apiInstance.getResolvedPrice(productId, opts, (error, data, response) => {
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
 **quantity** | **Number**|  | [optional] 
 **contactId** | **String**| Contact used to match customer-group-scoped tiers. | [optional] 

### Return type

[**ResolvedPriceResponse**](ResolvedPriceResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPriceTiers

> [PriceTier] listPriceTiers(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PriceTierApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'productId': "productId_example", // String | 
  'customerGroupId': "customerGroupId_example" // String | 
};
apiInstance.listPriceTiers(opts, (error, data, response) => {
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
 **customerGroupId** | **String**|  | [optional] 

### Return type

[**[PriceTier]**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updatePriceTier

> PriceTier updatePriceTier(priceTierId, priceTierUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PriceTierApi();
let priceTierId = "priceTierId_example"; // String | 
let priceTierUpdate = new SimpleBillyApi.PriceTierUpdate(); // PriceTierUpdate | 
apiInstance.updatePriceTier(priceTierId, priceTierUpdate, (error, data, response) => {
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
 **priceTierId** | **String**|  | 
 **priceTierUpdate** | [**PriceTierUpdate**](PriceTierUpdate.md)|  | 

### Return type

[**PriceTier**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


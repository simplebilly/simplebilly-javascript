# SimpleBillyApi.ShippingRuleApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createShippingRule**](ShippingRuleApi.md#createShippingRule) | **POST** /api/v1/shipping-rules | 
[**deleteShippingRule**](ShippingRuleApi.md#deleteShippingRule) | **DELETE** /api/v1/shipping-rules/{rule_id} | 
[**getShippingRule**](ShippingRuleApi.md#getShippingRule) | **GET** /api/v1/shipping-rules/{rule_id} | 
[**listShippingRules**](ShippingRuleApi.md#listShippingRules) | **GET** /api/v1/shipping-rules/ | 
[**updateShippingRule**](ShippingRuleApi.md#updateShippingRule) | **PUT** /api/v1/shipping-rules/{rule_id} | 



## createShippingRule

> ShippingRule createShippingRule(shippingRuleCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingRuleApi();
let shippingRuleCreate = new SimpleBillyApi.ShippingRuleCreate(); // ShippingRuleCreate | 
apiInstance.createShippingRule(shippingRuleCreate, (error, data, response) => {
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
 **shippingRuleCreate** | [**ShippingRuleCreate**](ShippingRuleCreate.md)|  | 

### Return type

[**ShippingRule**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteShippingRule

> deleteShippingRule(ruleId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingRuleApi();
let ruleId = "ruleId_example"; // String | 
apiInstance.deleteShippingRule(ruleId, (error, data, response) => {
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
 **ruleId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getShippingRule

> ShippingRule getShippingRule(ruleId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingRuleApi();
let ruleId = "ruleId_example"; // String | 
apiInstance.getShippingRule(ruleId, (error, data, response) => {
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
 **ruleId** | **String**|  | 

### Return type

[**ShippingRule**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listShippingRules

> [ShippingRule] listShippingRules(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingRuleApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'country': "country_example" // String | 
};
apiInstance.listShippingRules(opts, (error, data, response) => {
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
 **country** | **String**|  | [optional] 

### Return type

[**[ShippingRule]**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateShippingRule

> ShippingRule updateShippingRule(ruleId, shippingRuleUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShippingRuleApi();
let ruleId = "ruleId_example"; // String | 
let shippingRuleUpdate = new SimpleBillyApi.ShippingRuleUpdate(); // ShippingRuleUpdate | 
apiInstance.updateShippingRule(ruleId, shippingRuleUpdate, (error, data, response) => {
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
 **ruleId** | **String**|  | 
 **shippingRuleUpdate** | [**ShippingRuleUpdate**](ShippingRuleUpdate.md)|  | 

### Return type

[**ShippingRule**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


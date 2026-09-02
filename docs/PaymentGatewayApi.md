# SimpleBillyApi.PaymentGatewayApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPaymentGatewayApi**](PaymentGatewayApi.md#createPaymentGatewayApi) | **POST** /api/v1/payment-gateways | 
[**deletePaymentGatewayApi**](PaymentGatewayApi.md#deletePaymentGatewayApi) | **DELETE** /api/v1/payment-gateways/{gateway_id} | 
[**listPaymentGatewaysApi**](PaymentGatewayApi.md#listPaymentGatewaysApi) | **GET** /api/v1/payment-gateways/ | 
[**oauthAuthorizeApi**](PaymentGatewayApi.md#oauthAuthorizeApi) | **POST** /api/v1/payment-gateways/oauth/authorize | 
[**oauthCallbackApi**](PaymentGatewayApi.md#oauthCallbackApi) | **POST** /api/v1/payment-gateways/oauth/callback | 
[**updatePaymentGatewayApi**](PaymentGatewayApi.md#updatePaymentGatewayApi) | **PUT** /api/v1/payment-gateways/{gateway_id} | 



## createPaymentGatewayApi

> PaymentGateway createPaymentGatewayApi(body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PaymentGatewayApi();
let body = null; // Object | 
apiInstance.createPaymentGatewayApi(body, (error, data, response) => {
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
 **body** | **Object**|  | 

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletePaymentGatewayApi

> deletePaymentGatewayApi(gatewayId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PaymentGatewayApi();
let gatewayId = "gatewayId_example"; // String | 
apiInstance.deletePaymentGatewayApi(gatewayId, (error, data, response) => {
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
 **gatewayId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPaymentGatewaysApi

> [PaymentGateway] listPaymentGatewaysApi()



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PaymentGatewayApi();
apiInstance.listPaymentGatewaysApi((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**[PaymentGateway]**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## oauthAuthorizeApi

> GatewayOAuthAuthorizeResponse oauthAuthorizeApi(gatewayOAuthAuthorizeRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PaymentGatewayApi();
let gatewayOAuthAuthorizeRequest = new SimpleBillyApi.GatewayOAuthAuthorizeRequest(); // GatewayOAuthAuthorizeRequest | 
apiInstance.oauthAuthorizeApi(gatewayOAuthAuthorizeRequest, (error, data, response) => {
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
 **gatewayOAuthAuthorizeRequest** | [**GatewayOAuthAuthorizeRequest**](GatewayOAuthAuthorizeRequest.md)|  | 

### Return type

[**GatewayOAuthAuthorizeResponse**](GatewayOAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## oauthCallbackApi

> PaymentGateway oauthCallbackApi(gatewayOAuthCallbackRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PaymentGatewayApi();
let gatewayOAuthCallbackRequest = new SimpleBillyApi.GatewayOAuthCallbackRequest(); // GatewayOAuthCallbackRequest | 
apiInstance.oauthCallbackApi(gatewayOAuthCallbackRequest, (error, data, response) => {
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
 **gatewayOAuthCallbackRequest** | [**GatewayOAuthCallbackRequest**](GatewayOAuthCallbackRequest.md)|  | 

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updatePaymentGatewayApi

> PaymentGateway updatePaymentGatewayApi(gatewayId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PaymentGatewayApi();
let gatewayId = "gatewayId_example"; // String | 
let body = null; // Object | 
apiInstance.updatePaymentGatewayApi(gatewayId, body, (error, data, response) => {
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
 **gatewayId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


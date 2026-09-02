# SimpleBillyApi.PublicReturnsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getPublicReturnStatus**](PublicReturnsApi.md#getPublicReturnStatus) | **GET** /api/v1/public/returns/status | Customer checks the status of a return (public, no auth). The return is only revealed when its linked order&#39;s email matches.
[**listPublicReturns**](PublicReturnsApi.md#listPublicReturns) | **GET** /api/v1/public/returns/list | List all returns for an order (public, no auth).
[**requestPublicReturn**](PublicReturnsApi.md#requestPublicReturn) | **POST** /api/v1/public/returns/request | Customer requests a return for an order (public, no auth).



## getPublicReturnStatus

> PublicReturnStatusResponse getPublicReturnStatus(email, opts)

Customer checks the status of a return (public, no auth). The return is only revealed when its linked order&#39;s email matches.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PublicReturnsApi();
let email = "email_example"; // String | 
let opts = {
  'returnNumber': "returnNumber_example", // String | Either return_number or return_order_id must be provided.
  'returnOrderId': "returnOrderId_example", // String | 
  'orderNumber': "orderNumber_example" // String | 
};
apiInstance.getPublicReturnStatus(email, opts, (error, data, response) => {
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
 **email** | **String**|  | 
 **returnNumber** | **String**| Either return_number or return_order_id must be provided. | [optional] 
 **returnOrderId** | **String**|  | [optional] 
 **orderNumber** | **String**|  | [optional] 

### Return type

[**PublicReturnStatusResponse**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPublicReturns

> [PublicReturnStatusResponse] listPublicReturns(orderNumber, email)

List all returns for an order (public, no auth).

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PublicReturnsApi();
let orderNumber = "orderNumber_example"; // String | 
let email = "email_example"; // String | 
apiInstance.listPublicReturns(orderNumber, email, (error, data, response) => {
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
 **orderNumber** | **String**|  | 
 **email** | **String**|  | 

### Return type

[**[PublicReturnStatusResponse]**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## requestPublicReturn

> PublicReturnResponse requestPublicReturn(publicReturnRequest)

Customer requests a return for an order (public, no auth).

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PublicReturnsApi();
let publicReturnRequest = new SimpleBillyApi.PublicReturnRequest(); // PublicReturnRequest | 
apiInstance.requestPublicReturn(publicReturnRequest, (error, data, response) => {
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
 **publicReturnRequest** | [**PublicReturnRequest**](PublicReturnRequest.md)|  | 

### Return type

[**PublicReturnResponse**](PublicReturnResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


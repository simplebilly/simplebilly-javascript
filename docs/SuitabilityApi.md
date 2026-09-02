# SimpleBillyApi.SuitabilityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**shippingSuitabilityApi**](SuitabilityApi.md#shippingSuitabilityApi) | **POST** /api/v1/shipping/suitability | 



## shippingSuitabilityApi

> SuitabilityResult shippingSuitabilityApi(suitabilityRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SuitabilityApi();
let suitabilityRequest = new SimpleBillyApi.SuitabilityRequest(); // SuitabilityRequest | 
apiInstance.shippingSuitabilityApi(suitabilityRequest, (error, data, response) => {
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
 **suitabilityRequest** | [**SuitabilityRequest**](SuitabilityRequest.md)|  | 

### Return type

[**SuitabilityResult**](SuitabilityResult.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


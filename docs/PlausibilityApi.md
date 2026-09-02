# SimpleBillyApi.PlausibilityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**plausibilityCheckApi**](PlausibilityApi.md#plausibilityCheckApi) | **GET** /api/v1/bookkeeping/plausibility | 



## plausibilityCheckApi

> PlausibilityReport plausibilityCheckApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.PlausibilityApi();
let opts = {
  'dateFrom': "dateFrom_example", // String | 
  'dateTo': "dateTo_example" // String | 
};
apiInstance.plausibilityCheckApi(opts, (error, data, response) => {
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
 **dateFrom** | **String**|  | [optional] 
 **dateTo** | **String**|  | [optional] 

### Return type

[**PlausibilityReport**](PlausibilityReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


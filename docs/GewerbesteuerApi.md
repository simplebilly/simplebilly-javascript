# SimpleBillyApi.GewerbesteuerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gewerbesteuerApi**](GewerbesteuerApi.md#gewerbesteuerApi) | **GET** /api/v1/bookkeeping/gewerbesteuer | 



## gewerbesteuerApi

> GewerbesteuerErgebnis gewerbesteuerApi(year, opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.GewerbesteuerApi();
let year = 56; // Number | 
let opts = {
  'hebesatz': "hebesatz_example", // String | 
  'gewerbeertrag': "gewerbeertrag_example", // String | 
  'country': "country_example", // String | 
  'gemeindeschluessel': "gemeindeschluessel_example" // String | 
};
apiInstance.gewerbesteuerApi(year, opts, (error, data, response) => {
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
 **year** | **Number**|  | 
 **hebesatz** | **String**|  | [optional] 
 **gewerbeertrag** | **String**|  | [optional] 
 **country** | **String**|  | [optional] 
 **gemeindeschluessel** | **String**|  | [optional] 

### Return type

[**GewerbesteuerErgebnis**](GewerbesteuerErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


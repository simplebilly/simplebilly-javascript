# SimpleBillyApi.KstApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**kstApi**](KstApi.md#kstApi) | **GET** /api/v1/bookkeeping/kst | 



## kstApi

> KstErgebnis kstApi(year, opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.KstApi();
let year = 56; // Number | 
let opts = {
  'gewinn': "gewinn_example" // String | 
};
apiInstance.kstApi(year, opts, (error, data, response) => {
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
 **gewinn** | **String**|  | [optional] 

### Return type

[**KstErgebnis**](KstErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


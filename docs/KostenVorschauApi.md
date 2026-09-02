# SimpleBillyApi.KostenVorschauApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**kostenVorschauApi**](KostenVorschauApi.md#kostenVorschauApi) | **GET** /api/v1/bookkeeping/kosten-vorschau | 



## kostenVorschauApi

> KostenVorschau kostenVorschauApi(year, month)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.KostenVorschauApi();
let year = 56; // Number | 
let month = 56; // Number | 
apiInstance.kostenVorschauApi(year, month, (error, data, response) => {
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
 **month** | **Number**|  | 

### Return type

[**KostenVorschau**](KostenVorschau.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


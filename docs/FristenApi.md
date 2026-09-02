# SimpleBillyApi.FristenApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fristenApi**](FristenApi.md#fristenApi) | **GET** /api/v1/bookkeeping/fristen | 



## fristenApi

> FristenErgebnis fristenApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.FristenApi();
let opts = {
  'bundesland': "bundesland_example", // String | 
  'voranmeldungsrhythmus': "voranmeldungsrhythmus_example", // String | 
  'dauerfristverlaengerung': true, // Boolean | 
  'estAktiv': true, // Boolean | 
  'gewstAktiv': true, // Boolean | 
  'monate': 56 // Number | 
};
apiInstance.fristenApi(opts, (error, data, response) => {
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
 **bundesland** | **String**|  | [optional] 
 **voranmeldungsrhythmus** | **String**|  | [optional] 
 **dauerfristverlaengerung** | **Boolean**|  | [optional] 
 **estAktiv** | **Boolean**|  | [optional] 
 **gewstAktiv** | **Boolean**|  | [optional] 
 **monate** | **Number**|  | [optional] 

### Return type

[**FristenErgebnis**](FristenErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


# SimpleBillyApi.GezApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gezApi**](GezApi.md#gezApi) | **GET** /api/v1/bookkeeping/gez | 



## gezApi

> GezReport gezApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.GezApi();
let opts = {
  'jahr': 56, // Number | 
  'betriebsstaetten': "betriebsstaetten_example", // String | Liste der Betriebsstätten als JSON, z.B. `[{\"name\":\"Filiale 1\",\"beschaefigte\":12}]`.
  'kfz': 789, // Number | Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind).
  'hotelzimmer': 789, // Number | Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen.
  'beschaefigte': 789 // Number | Gesamtzahl der Beschäftigten (verwendet nur, wenn `betriebsstaetten` fehlt; dann wird eine einzelne Betriebsstätte angenommen).
};
apiInstance.gezApi(opts, (error, data, response) => {
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
 **jahr** | **Number**|  | [optional] 
 **betriebsstaetten** | **String**| Liste der Betriebsstätten als JSON, z.B. &#x60;[{\&quot;name\&quot;:\&quot;Filiale 1\&quot;,\&quot;beschaefigte\&quot;:12}]&#x60;. | [optional] 
 **kfz** | **Number**| Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind). | [optional] 
 **hotelzimmer** | **Number**| Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen. | [optional] 
 **beschaefigte** | **Number**| Gesamtzahl der Beschäftigten (verwendet nur, wenn &#x60;betriebsstaetten&#x60; fehlt; dann wird eine einzelne Betriebsstätte angenommen). | [optional] 

### Return type

[**GezReport**](GezReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


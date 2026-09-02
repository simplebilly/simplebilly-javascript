# SimpleBillyApi.ListOpenItemsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listOpenItemsApi**](ListOpenItemsApi.md#listOpenItemsApi) | **GET** /api/v1/bookkeeping/open-items | 



## listOpenItemsApi

> [OpenItem] listOpenItemsApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ListOpenItemsApi();
let opts = {
  'reminderLevel1Days': 789, // Number | 
  'reminderLevel2Days': 789, // Number | 
  'reminderLevel3Days': 789, // Number | 
  'customerId': "customerId_example" // String | 
};
apiInstance.listOpenItemsApi(opts, (error, data, response) => {
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
 **reminderLevel1Days** | **Number**|  | [optional] 
 **reminderLevel2Days** | **Number**|  | [optional] 
 **reminderLevel3Days** | **Number**|  | [optional] 
 **customerId** | **String**|  | [optional] 

### Return type

[**[OpenItem]**](OpenItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


# SimpleBillyApi.ProposeAssignmentsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**proposeAssignmentsApi**](ProposeAssignmentsApi.md#proposeAssignmentsApi) | **GET** /api/v1/bookkeeping/propose-assignments | 



## proposeAssignmentsApi

> [ProposedAssignment] proposeAssignmentsApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ProposeAssignmentsApi();
let opts = {
  'minConfidence': 3.4, // Number | 
  'customerId': "customerId_example" // String | 
};
apiInstance.proposeAssignmentsApi(opts, (error, data, response) => {
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
 **minConfidence** | **Number**|  | [optional] 
 **customerId** | **String**|  | [optional] 

### Return type

[**[ProposedAssignment]**](ProposedAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


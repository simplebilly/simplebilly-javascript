# SimpleBillyApi.ReorderProposalApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**applyReorderProposal**](ReorderProposalApi.md#applyReorderProposal) | **POST** /api/v1/reorder-proposals/apply | Convert a reorder proposal into a draft purchase order.
[**getReorderProposal**](ReorderProposalApi.md#getReorderProposal) | **GET** /api/v1/reorder-proposals | 



## applyReorderProposal

> Object applyReorderProposal(opts)

Convert a reorder proposal into a draft purchase order.

Returns the created purchase order id. Suggested line items are generated with the current reorder quantity per product.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReorderProposalApi();
let opts = {
  'configuredOnly': true, // Boolean | Only include products with a reorder point configured (`min_stock`).
  'warehouseId': "warehouseId_example" // String | Limit to a single warehouse id.
};
apiInstance.applyReorderProposal(opts, (error, data, response) => {
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
 **configuredOnly** | **Boolean**| Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [optional] 
 **warehouseId** | **String**| Limit to a single warehouse id. | [optional] 

### Return type

**Object**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getReorderProposal

> ReorderProposalResponse getReorderProposal(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReorderProposalApi();
let opts = {
  'configuredOnly': true, // Boolean | Only include products with a reorder point configured (`min_stock`).
  'warehouseId': "warehouseId_example" // String | Limit to a single warehouse id.
};
apiInstance.getReorderProposal(opts, (error, data, response) => {
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
 **configuredOnly** | **Boolean**| Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [optional] 
 **warehouseId** | **String**| Limit to a single warehouse id. | [optional] 

### Return type

[**ReorderProposalResponse**](ReorderProposalResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


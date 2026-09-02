# SimpleBillyApi.ReplenishmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**applyReplenishments**](ReplenishmentApi.md#applyReplenishments) | **POST** /api/v1/replenishments/apply | Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.
[**getReplenishments**](ReplenishmentApi.md#getReplenishments) | **GET** /api/v1/replenishments | 



## applyReplenishments

> Object applyReplenishments(opts)

Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReplenishmentApi();
let opts = {
  'targetWarehouseId': "targetWarehouseId_example", // String | Warehouse to be replenished. Defaults to the tenant's default warehouse.
  'sourceWarehouseId': "sourceWarehouseId_example" // String | Restrict source warehouses to this id.
};
apiInstance.applyReplenishments(opts, (error, data, response) => {
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
 **targetWarehouseId** | **String**| Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [optional] 
 **sourceWarehouseId** | **String**| Restrict source warehouses to this id. | [optional] 

### Return type

**Object**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getReplenishments

> ReplenishmentResponse getReplenishments(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReplenishmentApi();
let opts = {
  'targetWarehouseId': "targetWarehouseId_example", // String | Warehouse to be replenished. Defaults to the tenant's default warehouse.
  'sourceWarehouseId': "sourceWarehouseId_example" // String | Restrict source warehouses to this id.
};
apiInstance.getReplenishments(opts, (error, data, response) => {
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
 **targetWarehouseId** | **String**| Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [optional] 
 **sourceWarehouseId** | **String**| Restrict source warehouses to this id. | [optional] 

### Return type

[**ReplenishmentResponse**](ReplenishmentResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


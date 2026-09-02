# SimpleBillyApi.StockMovementApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getStockMovement**](StockMovementApi.md#getStockMovement) | **GET** /api/v1/stock-movements/{movement_id} | 
[**listStockMovements**](StockMovementApi.md#listStockMovements) | **GET** /api/v1/stock-movements/ | 



## getStockMovement

> StockMovement getStockMovement(movementId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.StockMovementApi();
let movementId = "movementId_example"; // String | 
apiInstance.getStockMovement(movementId, (error, data, response) => {
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
 **movementId** | **String**|  | 

### Return type

[**StockMovement**](StockMovement.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listStockMovements

> [StockMovement] listStockMovements(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.StockMovementApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'productId': "productId_example", // String | 
  'warehouseId': "warehouseId_example", // String | 
  'movementType': "movementType_example", // String | 
  'from': new Date("2013-10-20"), // Date | Only movements on or after this date (inclusive).
  'to': new Date("2013-10-20") // Date | Only movements on or before this date (inclusive).
};
apiInstance.listStockMovements(opts, (error, data, response) => {
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
 **page** | **Number**|  | [optional] 
 **pageSize** | **Number**|  | [optional] 
 **productId** | **String**|  | [optional] 
 **warehouseId** | **String**|  | [optional] 
 **movementType** | **String**|  | [optional] 
 **from** | **Date**| Only movements on or after this date (inclusive). | [optional] 
 **to** | **Date**| Only movements on or before this date (inclusive). | [optional] 

### Return type

[**[StockMovement]**](StockMovement.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


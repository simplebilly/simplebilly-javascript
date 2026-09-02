# SimpleBillyApi.ShareholderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createShareholder**](ShareholderApi.md#createShareholder) | **POST** /api/v1/shareholders | 
[**deleteShareholder**](ShareholderApi.md#deleteShareholder) | **DELETE** /api/v1/shareholders/{id} | 
[**getShareholder**](ShareholderApi.md#getShareholder) | **GET** /api/v1/shareholders/{id} | 
[**getShareholders**](ShareholderApi.md#getShareholders) | **GET** /api/v1/shareholders/ | 
[**updateShareholder**](ShareholderApi.md#updateShareholder) | **PUT** /api/v1/shareholders/{id} | 



## createShareholder

> Shareholder createShareholder(shareholderCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShareholderApi();
let shareholderCreate = new SimpleBillyApi.ShareholderCreate(); // ShareholderCreate | 
apiInstance.createShareholder(shareholderCreate, (error, data, response) => {
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
 **shareholderCreate** | [**ShareholderCreate**](ShareholderCreate.md)|  | 

### Return type

[**Shareholder**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteShareholder

> deleteShareholder(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShareholderApi();
let id = "id_example"; // String | 
apiInstance.deleteShareholder(id, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getShareholder

> Shareholder getShareholder(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShareholderApi();
let id = "id_example"; // String | 
apiInstance.getShareholder(id, (error, data, response) => {
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
 **id** | **String**|  | 

### Return type

[**Shareholder**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getShareholders

> [Shareholder] getShareholders(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShareholderApi();
let opts = {
  'page': 1, // Number | 
  'pageSize': 56, // Number | 
  'search': "search_example", // String | 
  'includeDeleted': true // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
};
apiInstance.getShareholders(opts, (error, data, response) => {
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
 **search** | **String**|  | [optional] 
 **includeDeleted** | **Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] 

### Return type

[**[Shareholder]**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateShareholder

> Shareholder updateShareholder(id, shareholderUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ShareholderApi();
let id = "id_example"; // String | 
let shareholderUpdate = new SimpleBillyApi.ShareholderUpdate(); // ShareholderUpdate | 
apiInstance.updateShareholder(id, shareholderUpdate, (error, data, response) => {
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
 **id** | **String**|  | 
 **shareholderUpdate** | [**ShareholderUpdate**](ShareholderUpdate.md)|  | 

### Return type

[**Shareholder**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


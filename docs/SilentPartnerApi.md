# SimpleBillyApi.SilentPartnerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSilentPartner**](SilentPartnerApi.md#createSilentPartner) | **POST** /api/v1/silent-partners | 
[**deleteSilentPartner**](SilentPartnerApi.md#deleteSilentPartner) | **DELETE** /api/v1/silent-partners/{id} | 
[**getSilentPartner**](SilentPartnerApi.md#getSilentPartner) | **GET** /api/v1/silent-partners/{id} | 
[**getSilentPartners**](SilentPartnerApi.md#getSilentPartners) | **GET** /api/v1/silent-partners/ | 
[**updateSilentPartner**](SilentPartnerApi.md#updateSilentPartner) | **PUT** /api/v1/silent-partners/{id} | 



## createSilentPartner

> SilentPartner createSilentPartner(silentPartnerCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SilentPartnerApi();
let silentPartnerCreate = new SimpleBillyApi.SilentPartnerCreate(); // SilentPartnerCreate | 
apiInstance.createSilentPartner(silentPartnerCreate, (error, data, response) => {
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
 **silentPartnerCreate** | [**SilentPartnerCreate**](SilentPartnerCreate.md)|  | 

### Return type

[**SilentPartner**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteSilentPartner

> deleteSilentPartner(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SilentPartnerApi();
let id = "id_example"; // String | 
apiInstance.deleteSilentPartner(id, (error, data, response) => {
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


## getSilentPartner

> SilentPartner getSilentPartner(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SilentPartnerApi();
let id = "id_example"; // String | 
apiInstance.getSilentPartner(id, (error, data, response) => {
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

[**SilentPartner**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getSilentPartners

> [SilentPartner] getSilentPartners(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SilentPartnerApi();
let opts = {
  'page': 1, // Number | 
  'pageSize': 56, // Number | 
  'search': "search_example", // String | 
  'includeDeleted': true // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
};
apiInstance.getSilentPartners(opts, (error, data, response) => {
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

[**[SilentPartner]**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateSilentPartner

> SilentPartner updateSilentPartner(id, silentPartnerUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SilentPartnerApi();
let id = "id_example"; // String | 
let silentPartnerUpdate = new SimpleBillyApi.SilentPartnerUpdate(); // SilentPartnerUpdate | 
apiInstance.updateSilentPartner(id, silentPartnerUpdate, (error, data, response) => {
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
 **silentPartnerUpdate** | [**SilentPartnerUpdate**](SilentPartnerUpdate.md)|  | 

### Return type

[**SilentPartner**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


# SimpleBillyApi.KycRecordApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createKycRecord**](KycRecordApi.md#createKycRecord) | **POST** /api/v1/kyc-records | 
[**deleteKycRecord**](KycRecordApi.md#deleteKycRecord) | **DELETE** /api/v1/kyc-records/{id} | 
[**getKycRecord**](KycRecordApi.md#getKycRecord) | **GET** /api/v1/kyc-records/{id} | 
[**getKycRecords**](KycRecordApi.md#getKycRecords) | **GET** /api/v1/kyc-records/ | 
[**updateKycRecord**](KycRecordApi.md#updateKycRecord) | **PUT** /api/v1/kyc-records/{id} | 



## createKycRecord

> KycRecord createKycRecord(kycRecordCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.KycRecordApi();
let kycRecordCreate = new SimpleBillyApi.KycRecordCreate(); // KycRecordCreate | 
apiInstance.createKycRecord(kycRecordCreate, (error, data, response) => {
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
 **kycRecordCreate** | [**KycRecordCreate**](KycRecordCreate.md)|  | 

### Return type

[**KycRecord**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteKycRecord

> deleteKycRecord(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.KycRecordApi();
let id = "id_example"; // String | 
apiInstance.deleteKycRecord(id, (error, data, response) => {
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


## getKycRecord

> KycRecord getKycRecord(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.KycRecordApi();
let id = "id_example"; // String | 
apiInstance.getKycRecord(id, (error, data, response) => {
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

[**KycRecord**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getKycRecords

> [KycRecord] getKycRecords(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.KycRecordApi();
let opts = {
  'page': 1, // Number | 
  'pageSize': 56, // Number | 
  'search': "search_example", // String | 
  'includeDeleted': true // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
};
apiInstance.getKycRecords(opts, (error, data, response) => {
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

[**[KycRecord]**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateKycRecord

> KycRecord updateKycRecord(id, kycRecordUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.KycRecordApi();
let id = "id_example"; // String | 
let kycRecordUpdate = new SimpleBillyApi.KycRecordUpdate(); // KycRecordUpdate | 
apiInstance.updateKycRecord(id, kycRecordUpdate, (error, data, response) => {
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
 **kycRecordUpdate** | [**KycRecordUpdate**](KycRecordUpdate.md)|  | 

### Return type

[**KycRecord**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


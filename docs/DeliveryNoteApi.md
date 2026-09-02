# SimpleBillyApi.DeliveryNoteApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDeliveryNote**](DeliveryNoteApi.md#createDeliveryNote) | **POST** /api/v1/delivery-notes | 
[**deleteDeliveryNote**](DeliveryNoteApi.md#deleteDeliveryNote) | **DELETE** /api/v1/delivery-notes/{delivery_note_id} | 
[**deliverynoteRestore**](DeliveryNoteApi.md#deliverynoteRestore) | **POST** /api/v1/delivery-notes/{delivery_note_id}/restore | 
[**downloadDeliveryNotePdf**](DeliveryNoteApi.md#downloadDeliveryNotePdf) | **GET** /api/v1/delivery-notes/{delivery_note_id}/pdf | 
[**getDeliveryNote**](DeliveryNoteApi.md#getDeliveryNote) | **GET** /api/v1/delivery-notes/{delivery_note_id} | 
[**listDeliveryNotes**](DeliveryNoteApi.md#listDeliveryNotes) | **GET** /api/v1/delivery-notes/ | 
[**pursueDeliveryNote**](DeliveryNoteApi.md#pursueDeliveryNote) | **POST** /api/v1/delivery-notes/{delivery_note_id}/pursue | 



## createDeliveryNote

> DeliveryNote createDeliveryNote(deliveryNoteCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryNoteApi();
let deliveryNoteCreate = new SimpleBillyApi.DeliveryNoteCreate(); // DeliveryNoteCreate | 
apiInstance.createDeliveryNote(deliveryNoteCreate, (error, data, response) => {
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
 **deliveryNoteCreate** | [**DeliveryNoteCreate**](DeliveryNoteCreate.md)|  | 

### Return type

[**DeliveryNote**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteDeliveryNote

> deleteDeliveryNote(deliveryNoteId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryNoteApi();
let deliveryNoteId = "deliveryNoteId_example"; // String | 
apiInstance.deleteDeliveryNote(deliveryNoteId, (error, data, response) => {
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
 **deliveryNoteId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## deliverynoteRestore

> DeliveryNote deliverynoteRestore(deliveryNoteId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryNoteApi();
let deliveryNoteId = "deliveryNoteId_example"; // String | 
apiInstance.deliverynoteRestore(deliveryNoteId, (error, data, response) => {
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
 **deliveryNoteId** | **String**|  | 

### Return type

[**DeliveryNote**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## downloadDeliveryNotePdf

> downloadDeliveryNotePdf(deliveryNoteId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryNoteApi();
let deliveryNoteId = "deliveryNoteId_example"; // String | 
apiInstance.downloadDeliveryNotePdf(deliveryNoteId, (error, data, response) => {
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
 **deliveryNoteId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf, application/json


## getDeliveryNote

> DeliveryNote getDeliveryNote(deliveryNoteId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryNoteApi();
let deliveryNoteId = "deliveryNoteId_example"; // String | 
apiInstance.getDeliveryNote(deliveryNoteId, (error, data, response) => {
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
 **deliveryNoteId** | **String**|  | 

### Return type

[**DeliveryNote**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listDeliveryNotes

> [DeliveryNote] listDeliveryNotes(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryNoteApi();
let opts = {
  'page': 1, // Number | 
  'pageSize': 56, // Number | 
  'search': "search_example", // String | 
  'includeDeleted': true // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
};
apiInstance.listDeliveryNotes(opts, (error, data, response) => {
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

[**[DeliveryNote]**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## pursueDeliveryNote

> Invoice pursueDeliveryNote(deliveryNoteId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryNoteApi();
let deliveryNoteId = "deliveryNoteId_example"; // String | 
apiInstance.pursueDeliveryNote(deliveryNoteId, (error, data, response) => {
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
 **deliveryNoteId** | **String**|  | 

### Return type

[**Invoice**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


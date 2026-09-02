# SimpleBillyApi.DeliveryDateApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDeliveryDate**](DeliveryDateApi.md#createDeliveryDate) | **POST** /api/v1/delivery-dates | 
[**deleteDeliveryDate**](DeliveryDateApi.md#deleteDeliveryDate) | **DELETE** /api/v1/delivery-dates/{delivery_date_id} | 
[**getDeliveryDate**](DeliveryDateApi.md#getDeliveryDate) | **GET** /api/v1/delivery-dates/{delivery_date_id} | 
[**getDeliveryPerformance**](DeliveryDateApi.md#getDeliveryPerformance) | **GET** /api/v1/delivery-dates/performance | On-time performance summary: how many promised delivery dates were met within a period.
[**listDeliveryDates**](DeliveryDateApi.md#listDeliveryDates) | **GET** /api/v1/delivery-dates/ | 
[**updateDeliveryDate**](DeliveryDateApi.md#updateDeliveryDate) | **PUT** /api/v1/delivery-dates/{delivery_date_id} | 
[**updateDeliveryDateStatus**](DeliveryDateApi.md#updateDeliveryDateStatus) | **PUT** /api/v1/delivery-dates/{delivery_date_id}/status | 



## createDeliveryDate

> DeliveryDate createDeliveryDate(deliveryDateCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryDateApi();
let deliveryDateCreate = new SimpleBillyApi.DeliveryDateCreate(); // DeliveryDateCreate | 
apiInstance.createDeliveryDate(deliveryDateCreate, (error, data, response) => {
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
 **deliveryDateCreate** | [**DeliveryDateCreate**](DeliveryDateCreate.md)|  | 

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteDeliveryDate

> deleteDeliveryDate(deliveryDateId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryDateApi();
let deliveryDateId = "deliveryDateId_example"; // String | 
apiInstance.deleteDeliveryDate(deliveryDateId, (error, data, response) => {
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
 **deliveryDateId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDeliveryDate

> DeliveryDate getDeliveryDate(deliveryDateId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryDateApi();
let deliveryDateId = "deliveryDateId_example"; // String | 
apiInstance.getDeliveryDate(deliveryDateId, (error, data, response) => {
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
 **deliveryDateId** | **String**|  | 

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDeliveryPerformance

> Object getDeliveryPerformance(opts)

On-time performance summary: how many promised delivery dates were met within a period.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryDateApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'orderNumber': "orderNumber_example", // String | 
  'status': "status_example", // String | 
  'from': new Date("2013-10-20"), // Date | Only dates on or after this date.
  'to': new Date("2013-10-20") // Date | Only dates on or before this date.
};
apiInstance.getDeliveryPerformance(opts, (error, data, response) => {
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
 **orderNumber** | **String**|  | [optional] 
 **status** | **String**|  | [optional] 
 **from** | **Date**| Only dates on or after this date. | [optional] 
 **to** | **Date**| Only dates on or before this date. | [optional] 

### Return type

**Object**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listDeliveryDates

> [DeliveryDate] listDeliveryDates(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryDateApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'orderNumber': "orderNumber_example", // String | 
  'status': "status_example", // String | 
  'from': new Date("2013-10-20"), // Date | Only dates on or after this date.
  'to': new Date("2013-10-20") // Date | Only dates on or before this date.
};
apiInstance.listDeliveryDates(opts, (error, data, response) => {
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
 **orderNumber** | **String**|  | [optional] 
 **status** | **String**|  | [optional] 
 **from** | **Date**| Only dates on or after this date. | [optional] 
 **to** | **Date**| Only dates on or before this date. | [optional] 

### Return type

[**[DeliveryDate]**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateDeliveryDate

> DeliveryDate updateDeliveryDate(deliveryDateId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryDateApi();
let deliveryDateId = "deliveryDateId_example"; // String | 
let body = null; // Object | 
apiInstance.updateDeliveryDate(deliveryDateId, body, (error, data, response) => {
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
 **deliveryDateId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateDeliveryDateStatus

> DeliveryDate updateDeliveryDateStatus(deliveryDateId, deliveryDateStatusUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryDateApi();
let deliveryDateId = "deliveryDateId_example"; // String | 
let deliveryDateStatusUpdate = new SimpleBillyApi.DeliveryDateStatusUpdate(); // DeliveryDateStatusUpdate | 
apiInstance.updateDeliveryDateStatus(deliveryDateId, deliveryDateStatusUpdate, (error, data, response) => {
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
 **deliveryDateId** | **String**|  | 
 **deliveryDateStatusUpdate** | [**DeliveryDateStatusUpdate**](DeliveryDateStatusUpdate.md)|  | 

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


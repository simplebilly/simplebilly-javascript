# SimpleBillyApi.DeliveryAppointmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDeliveryAppointment**](DeliveryAppointmentApi.md#createDeliveryAppointment) | **POST** /api/v1/delivery-appointments | 
[**deleteDeliveryAppointment**](DeliveryAppointmentApi.md#deleteDeliveryAppointment) | **DELETE** /api/v1/delivery-appointments/{appointment_id} | 
[**getDeliveryAppointment**](DeliveryAppointmentApi.md#getDeliveryAppointment) | **GET** /api/v1/delivery-appointments/{appointment_id} | 
[**getPublicDeliveryAppointmentStatus**](DeliveryAppointmentApi.md#getPublicDeliveryAppointmentStatus) | **GET** /api/v1/public/delivery-appointments/status | Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.
[**listDeliveryAppointments**](DeliveryAppointmentApi.md#listDeliveryAppointments) | **GET** /api/v1/delivery-appointments | 
[**requestPublicDeliveryAppointment**](DeliveryAppointmentApi.md#requestPublicDeliveryAppointment) | **POST** /api/v1/public/delivery-appointments/request | Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request.
[**updateDeliveryAppointment**](DeliveryAppointmentApi.md#updateDeliveryAppointment) | **PUT** /api/v1/delivery-appointments/{appointment_id} | 
[**updateDeliveryAppointmentStatus**](DeliveryAppointmentApi.md#updateDeliveryAppointmentStatus) | **PUT** /api/v1/delivery-appointments/{appointment_id}/status | 



## createDeliveryAppointment

> DeliveryAppointment createDeliveryAppointment(deliveryAppointmentCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryAppointmentApi();
let deliveryAppointmentCreate = new SimpleBillyApi.DeliveryAppointmentCreate(); // DeliveryAppointmentCreate | 
apiInstance.createDeliveryAppointment(deliveryAppointmentCreate, (error, data, response) => {
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
 **deliveryAppointmentCreate** | [**DeliveryAppointmentCreate**](DeliveryAppointmentCreate.md)|  | 

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteDeliveryAppointment

> deleteDeliveryAppointment(appointmentId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryAppointmentApi();
let appointmentId = "appointmentId_example"; // String | 
apiInstance.deleteDeliveryAppointment(appointmentId, (error, data, response) => {
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
 **appointmentId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDeliveryAppointment

> DeliveryAppointment getDeliveryAppointment(appointmentId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryAppointmentApi();
let appointmentId = "appointmentId_example"; // String | 
apiInstance.getDeliveryAppointment(appointmentId, (error, data, response) => {
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
 **appointmentId** | **String**|  | 

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPublicDeliveryAppointmentStatus

> PublicDeliveryAppointmentStatusResponse getPublicDeliveryAppointmentStatus(appointmentId, email, token)

Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryAppointmentApi();
let appointmentId = "appointmentId_example"; // String | 
let email = "email_example"; // String | 
let token = "token_example"; // String | 
apiInstance.getPublicDeliveryAppointmentStatus(appointmentId, email, token, (error, data, response) => {
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
 **appointmentId** | **String**|  | 
 **email** | **String**|  | 
 **token** | **String**|  | 

### Return type

[**PublicDeliveryAppointmentStatusResponse**](PublicDeliveryAppointmentStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listDeliveryAppointments

> [DeliveryAppointment] listDeliveryAppointments(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryAppointmentApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'status': "status_example", // String | 
  'warehouseId': "warehouseId_example", // String | 
  'from': new Date("2013-10-20"), // Date | 
  'to': new Date("2013-10-20") // Date | 
};
apiInstance.listDeliveryAppointments(opts, (error, data, response) => {
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
 **status** | **String**|  | [optional] 
 **warehouseId** | **String**|  | [optional] 
 **from** | **Date**|  | [optional] 
 **to** | **Date**|  | [optional] 

### Return type

[**[DeliveryAppointment]**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## requestPublicDeliveryAppointment

> PublicDeliveryAppointmentResponse requestPublicDeliveryAppointment(publicDeliveryAppointmentRequest)

Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryAppointmentApi();
let publicDeliveryAppointmentRequest = new SimpleBillyApi.PublicDeliveryAppointmentRequest(); // PublicDeliveryAppointmentRequest | 
apiInstance.requestPublicDeliveryAppointment(publicDeliveryAppointmentRequest, (error, data, response) => {
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
 **publicDeliveryAppointmentRequest** | [**PublicDeliveryAppointmentRequest**](PublicDeliveryAppointmentRequest.md)|  | 

### Return type

[**PublicDeliveryAppointmentResponse**](PublicDeliveryAppointmentResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateDeliveryAppointment

> DeliveryAppointment updateDeliveryAppointment(appointmentId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryAppointmentApi();
let appointmentId = "appointmentId_example"; // String | 
let body = null; // Object | 
apiInstance.updateDeliveryAppointment(appointmentId, body, (error, data, response) => {
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
 **appointmentId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateDeliveryAppointmentStatus

> DeliveryAppointment updateDeliveryAppointmentStatus(appointmentId, appointmentStatusUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DeliveryAppointmentApi();
let appointmentId = "appointmentId_example"; // String | 
let appointmentStatusUpdate = new SimpleBillyApi.AppointmentStatusUpdate(); // AppointmentStatusUpdate | 
apiInstance.updateDeliveryAppointmentStatus(appointmentId, appointmentStatusUpdate, (error, data, response) => {
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
 **appointmentId** | **String**|  | 
 **appointmentStatusUpdate** | [**AppointmentStatusUpdate**](AppointmentStatusUpdate.md)|  | 

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


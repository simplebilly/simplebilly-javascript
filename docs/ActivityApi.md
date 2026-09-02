# SimpleBillyApi.ActivityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createActivity**](ActivityApi.md#createActivity) | **POST** /api/v1/activities | 
[**deleteActivity**](ActivityApi.md#deleteActivity) | **DELETE** /api/v1/activities/{activity_id} | 
[**getActivity**](ActivityApi.md#getActivity) | **GET** /api/v1/activities/{activity_id} | 
[**listActivities**](ActivityApi.md#listActivities) | **GET** /api/v1/activities/ | 
[**updateActivity**](ActivityApi.md#updateActivity) | **PUT** /api/v1/activities/{activity_id} | 
[**updateActivityStatus**](ActivityApi.md#updateActivityStatus) | **PUT** /api/v1/activities/{activity_id}/status | 



## createActivity

> Activity createActivity(activity)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ActivityApi();
let activity = new SimpleBillyApi.Activity(); // Activity | 
apiInstance.createActivity(activity, (error, data, response) => {
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
 **activity** | [**Activity**](Activity.md)|  | 

### Return type

[**Activity**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteActivity

> deleteActivity(activityId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ActivityApi();
let activityId = "activityId_example"; // String | 
apiInstance.deleteActivity(activityId, (error, data, response) => {
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
 **activityId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getActivity

> Activity getActivity(activityId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ActivityApi();
let activityId = "activityId_example"; // String | 
apiInstance.getActivity(activityId, (error, data, response) => {
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
 **activityId** | **String**|  | 

### Return type

[**Activity**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listActivities

> [Activity] listActivities(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ActivityApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'contactId': "contactId_example", // String | 
  'activityType': "activityType_example", // String | 
  'status': "status_example", // String | 
  'assignedTo': "assignedTo_example", // String | 
  'overdueOnly': true // Boolean | Only show overdue follow-ups.
};
apiInstance.listActivities(opts, (error, data, response) => {
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
 **contactId** | **String**|  | [optional] 
 **activityType** | **String**|  | [optional] 
 **status** | **String**|  | [optional] 
 **assignedTo** | **String**|  | [optional] 
 **overdueOnly** | **Boolean**| Only show overdue follow-ups. | [optional] 

### Return type

[**[Activity]**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateActivity

> Activity updateActivity(activityId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ActivityApi();
let activityId = "activityId_example"; // String | 
let body = null; // Object | 
apiInstance.updateActivity(activityId, body, (error, data, response) => {
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
 **activityId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**Activity**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateActivityStatus

> Activity updateActivityStatus(activityId, activityStatusUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ActivityApi();
let activityId = "activityId_example"; // String | 
let activityStatusUpdate = new SimpleBillyApi.ActivityStatusUpdate(); // ActivityStatusUpdate | 
apiInstance.updateActivityStatus(activityId, activityStatusUpdate, (error, data, response) => {
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
 **activityId** | **String**|  | 
 **activityStatusUpdate** | [**ActivityStatusUpdate**](ActivityStatusUpdate.md)|  | 

### Return type

[**Activity**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


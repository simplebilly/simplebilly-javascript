# SimpleBillyApi.TrainingAssignmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createTrainingAssignment**](TrainingAssignmentApi.md#createTrainingAssignment) | **POST** /api/v1/training-assignments | 
[**deleteTrainingAssignment**](TrainingAssignmentApi.md#deleteTrainingAssignment) | **DELETE** /api/v1/training-assignments/{id} | 
[**getTrainingAssignment**](TrainingAssignmentApi.md#getTrainingAssignment) | **GET** /api/v1/training-assignments/{id} | 
[**getTrainingAssignments**](TrainingAssignmentApi.md#getTrainingAssignments) | **GET** /api/v1/training-assignments/ | 
[**updateTrainingAssignment**](TrainingAssignmentApi.md#updateTrainingAssignment) | **PUT** /api/v1/training-assignments/{id} | 



## createTrainingAssignment

> TrainingAssignment createTrainingAssignment(trainingAssignmentCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TrainingAssignmentApi();
let trainingAssignmentCreate = new SimpleBillyApi.TrainingAssignmentCreate(); // TrainingAssignmentCreate | 
apiInstance.createTrainingAssignment(trainingAssignmentCreate, (error, data, response) => {
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
 **trainingAssignmentCreate** | [**TrainingAssignmentCreate**](TrainingAssignmentCreate.md)|  | 

### Return type

[**TrainingAssignment**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteTrainingAssignment

> deleteTrainingAssignment(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TrainingAssignmentApi();
let id = "id_example"; // String | 
apiInstance.deleteTrainingAssignment(id, (error, data, response) => {
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


## getTrainingAssignment

> TrainingAssignment getTrainingAssignment(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TrainingAssignmentApi();
let id = "id_example"; // String | 
apiInstance.getTrainingAssignment(id, (error, data, response) => {
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

[**TrainingAssignment**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTrainingAssignments

> [TrainingAssignment] getTrainingAssignments(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TrainingAssignmentApi();
let opts = {
  'page': 1, // Number | 
  'pageSize': 56, // Number | 
  'search': "search_example", // String | 
  'includeDeleted': true // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
};
apiInstance.getTrainingAssignments(opts, (error, data, response) => {
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

[**[TrainingAssignment]**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateTrainingAssignment

> TrainingAssignment updateTrainingAssignment(id, trainingAssignmentUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TrainingAssignmentApi();
let id = "id_example"; // String | 
let trainingAssignmentUpdate = new SimpleBillyApi.TrainingAssignmentUpdate(); // TrainingAssignmentUpdate | 
apiInstance.updateTrainingAssignment(id, trainingAssignmentUpdate, (error, data, response) => {
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
 **trainingAssignmentUpdate** | [**TrainingAssignmentUpdate**](TrainingAssignmentUpdate.md)|  | 

### Return type

[**TrainingAssignment**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


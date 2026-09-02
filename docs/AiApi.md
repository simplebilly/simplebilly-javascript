# SimpleBillyApi.AiApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**aiSuggestApi**](AiApi.md#aiSuggestApi) | **POST** /api/v1/support/ai/suggest | 
[**createWorkerApi**](AiApi.md#createWorkerApi) | **POST** /api/v1/support/ai/workers | 
[**listWorkersApi**](AiApi.md#listWorkersApi) | **GET** /api/v1/support/ai/workers | 
[**runWorkerApi**](AiApi.md#runWorkerApi) | **POST** /api/v1/support/ai/workers/{worker_id}/run | 



## aiSuggestApi

> AiSuggestion aiSuggestApi(aiSuggestionRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.AiApi();
let aiSuggestionRequest = new SimpleBillyApi.AiSuggestionRequest(); // AiSuggestionRequest | 
apiInstance.aiSuggestApi(aiSuggestionRequest, (error, data, response) => {
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
 **aiSuggestionRequest** | [**AiSuggestionRequest**](AiSuggestionRequest.md)|  | 

### Return type

[**AiSuggestion**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createWorkerApi

> AiWorkerConfig createWorkerApi(aiConfigDto)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.AiApi();
let aiConfigDto = new SimpleBillyApi.AiConfigDto(); // AiConfigDto | 
apiInstance.createWorkerApi(aiConfigDto, (error, data, response) => {
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
 **aiConfigDto** | [**AiConfigDto**](AiConfigDto.md)|  | 

### Return type

[**AiWorkerConfig**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## listWorkersApi

> [AiWorkerConfig] listWorkersApi()



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.AiApi();
apiInstance.listWorkersApi((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**[AiWorkerConfig]**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## runWorkerApi

> AiSuggestion runWorkerApi(workerId, aiSuggestionRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.AiApi();
let workerId = "workerId_example"; // String | 
let aiSuggestionRequest = new SimpleBillyApi.AiSuggestionRequest(); // AiSuggestionRequest | 
apiInstance.runWorkerApi(workerId, aiSuggestionRequest, (error, data, response) => {
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
 **workerId** | **String**|  | 
 **aiSuggestionRequest** | [**AiSuggestionRequest**](AiSuggestionRequest.md)|  | 

### Return type

[**AiSuggestion**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


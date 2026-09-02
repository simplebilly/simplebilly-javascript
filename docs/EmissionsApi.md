# SimpleBillyApi.EmissionsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createEmissionEntryApi**](EmissionsApi.md#createEmissionEntryApi) | **POST** /api/v1/bookkeeping/emissions/entries | 
[**createEmissionTargetApi**](EmissionsApi.md#createEmissionTargetApi) | **POST** /api/v1/bookkeeping/emissions/targets | 
[**deleteEmissionEntryApi**](EmissionsApi.md#deleteEmissionEntryApi) | **DELETE** /api/v1/bookkeeping/emissions/entries/{id} | 
[**deleteEmissionTargetApi**](EmissionsApi.md#deleteEmissionTargetApi) | **DELETE** /api/v1/bookkeeping/emissions/targets/{id} | 
[**emissionsEntriesApi**](EmissionsApi.md#emissionsEntriesApi) | **GET** /api/v1/bookkeeping/emissions/entries | 
[**emissionsExportApi**](EmissionsApi.md#emissionsExportApi) | **GET** /api/v1/bookkeeping/emissions/export | 
[**emissionsFactorsApi**](EmissionsApi.md#emissionsFactorsApi) | **GET** /api/v1/bookkeeping/emissions/factors | 
[**emissionsReportApi**](EmissionsApi.md#emissionsReportApi) | **GET** /api/v1/bookkeeping/emissions/report | 
[**emissionsTargetsApi**](EmissionsApi.md#emissionsTargetsApi) | **GET** /api/v1/bookkeeping/emissions/targets | 



## createEmissionEntryApi

> EmissionEntry createEmissionEntryApi(createEmissionEntry)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmissionsApi();
let createEmissionEntry = new SimpleBillyApi.CreateEmissionEntry(); // CreateEmissionEntry | 
apiInstance.createEmissionEntryApi(createEmissionEntry, (error, data, response) => {
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
 **createEmissionEntry** | [**CreateEmissionEntry**](CreateEmissionEntry.md)|  | 

### Return type

[**EmissionEntry**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createEmissionTargetApi

> EmissionTarget createEmissionTargetApi(createEmissionTarget)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmissionsApi();
let createEmissionTarget = new SimpleBillyApi.CreateEmissionTarget(); // CreateEmissionTarget | 
apiInstance.createEmissionTargetApi(createEmissionTarget, (error, data, response) => {
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
 **createEmissionTarget** | [**CreateEmissionTarget**](CreateEmissionTarget.md)|  | 

### Return type

[**EmissionTarget**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteEmissionEntryApi

> deleteEmissionEntryApi(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmissionsApi();
let id = "id_example"; // String | 
apiInstance.deleteEmissionEntryApi(id, (error, data, response) => {
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


## deleteEmissionTargetApi

> deleteEmissionTargetApi(id)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmissionsApi();
let id = "id_example"; // String | 
apiInstance.deleteEmissionTargetApi(id, (error, data, response) => {
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


## emissionsEntriesApi

> [EmissionEntry] emissionsEntriesApi(year)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmissionsApi();
let year = 56; // Number | 
apiInstance.emissionsEntriesApi(year, (error, data, response) => {
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
 **year** | **Number**|  | 

### Return type

[**[EmissionEntry]**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## emissionsExportApi

> EmissionsExportResponse emissionsExportApi(year)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmissionsApi();
let year = 56; // Number | 
apiInstance.emissionsExportApi(year, (error, data, response) => {
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
 **year** | **Number**|  | 

### Return type

[**EmissionsExportResponse**](EmissionsExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## emissionsFactorsApi

> [EmissionFactorResponse] emissionsFactorsApi()



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmissionsApi();
apiInstance.emissionsFactorsApi((error, data, response) => {
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

[**[EmissionFactorResponse]**](EmissionFactorResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## emissionsReportApi

> EmissionsReport emissionsReportApi(year)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmissionsApi();
let year = 56; // Number | 
apiInstance.emissionsReportApi(year, (error, data, response) => {
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
 **year** | **Number**|  | 

### Return type

[**EmissionsReport**](EmissionsReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## emissionsTargetsApi

> [EmissionTarget] emissionsTargetsApi()



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmissionsApi();
apiInstance.emissionsTargetsApi((error, data, response) => {
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

[**[EmissionTarget]**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


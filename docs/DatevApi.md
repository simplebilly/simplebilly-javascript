# SimpleBillyApi.DatevApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**datevExportApi**](DatevApi.md#datevExportApi) | **GET** /api/v1/bookkeeping/datev/export | Export bookkeeping data as DATEV CSV
[**datevPreviewApi**](DatevApi.md#datevPreviewApi) | **GET** /api/v1/bookkeeping/datev/preview | Exported_datev_bookings: returns formed bookings for review



## datevExportApi

> DatevExportResponse datevExportApi(opts)

Export bookkeeping data as DATEV CSV

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DatevApi();
let opts = {
  'accountSchema': "accountSchema_example", // String | 
  'dateFrom': "dateFrom_example", // String | 
  'dateTo': "dateTo_example", // String | 
  'page': 56, // Number | 
  'pageSize': 56 // Number | 
};
apiInstance.datevExportApi(opts, (error, data, response) => {
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
 **accountSchema** | **String**|  | [optional] 
 **dateFrom** | **String**|  | [optional] 
 **dateTo** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] 
 **pageSize** | **Number**|  | [optional] 

### Return type

[**DatevExportResponse**](DatevExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## datevPreviewApi

> [DatevBookingPreview] datevPreviewApi(opts)

Exported_datev_bookings: returns formed bookings for review

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.DatevApi();
let opts = {
  'accountSchema': "accountSchema_example", // String | 
  'dateFrom': "dateFrom_example", // String | 
  'dateTo': "dateTo_example", // String | 
  'page': 56, // Number | 
  'pageSize': 56 // Number | 
};
apiInstance.datevPreviewApi(opts, (error, data, response) => {
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
 **accountSchema** | **String**|  | [optional] 
 **dateFrom** | **String**|  | [optional] 
 **dateTo** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] 
 **pageSize** | **Number**|  | [optional] 

### Return type

[**[DatevBookingPreview]**](DatevBookingPreview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


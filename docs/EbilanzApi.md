# SimpleBillyApi.EbilanzApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ebilanzReportApi**](EbilanzApi.md#ebilanzReportApi) | **GET** /api/v1/bookkeeping/ebilanz | 
[**ebilanzXbrlExportApi**](EbilanzApi.md#ebilanzXbrlExportApi) | **GET** /api/v1/bookkeeping/ebilanz/xbrl | 



## ebilanzReportApi

> EBilanzReport ebilanzReportApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EbilanzApi();
let opts = {
  'year': 56, // Number | 
  'dateFrom': "dateFrom_example", // String | 
  'dateTo': "dateTo_example" // String | 
};
apiInstance.ebilanzReportApi(opts, (error, data, response) => {
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
 **year** | **Number**|  | [optional] 
 **dateFrom** | **String**|  | [optional] 
 **dateTo** | **String**|  | [optional] 

### Return type

[**EBilanzReport**](EBilanzReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## ebilanzXbrlExportApi

> ebilanzXbrlExportApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EbilanzApi();
let opts = {
  'year': 56, // Number | 
  'dateFrom': "dateFrom_example", // String | 
  'dateTo': "dateTo_example" // String | 
};
apiInstance.ebilanzXbrlExportApi(opts, (error, data, response) => {
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
 **year** | **Number**|  | [optional] 
 **dateFrom** | **String**|  | [optional] 
 **dateTo** | **String**|  | [optional] 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/xml


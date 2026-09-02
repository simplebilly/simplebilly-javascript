# SimpleBillyApi.ReportsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bilanzReportApi**](ReportsApi.md#bilanzReportApi) | **GET** /api/v1/bookkeeping/reports/bilanz | Bilanz (Balance Sheet)
[**guvReportApi**](ReportsApi.md#guvReportApi) | **GET** /api/v1/bookkeeping/reports/guv | Gewinn- und Verlustrechnung (P&amp;L statement)
[**kontenansichtReportApi**](ReportsApi.md#kontenansichtReportApi) | **GET** /api/v1/bookkeeping/reports/kontenansicht | Kontenansicht (Account Overview)
[**umsatzsteuerReportApi**](ReportsApi.md#umsatzsteuerReportApi) | **GET** /api/v1/bookkeeping/reports/umsatzsteuer | Umsatzsteuer-Voranmeldung (VAT report)



## bilanzReportApi

> BilanzReport bilanzReportApi(opts)

Bilanz (Balance Sheet)

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReportsApi();
let opts = {
  'year': 56, // Number | 
  'month': 56, // Number | 
  'dateFrom': "dateFrom_example", // String | 
  'dateTo': "dateTo_example", // String | 
  'page': 56, // Number | 
  'pageSize': 56 // Number | 
};
apiInstance.bilanzReportApi(opts, (error, data, response) => {
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
 **month** | **Number**|  | [optional] 
 **dateFrom** | **String**|  | [optional] 
 **dateTo** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] 
 **pageSize** | **Number**|  | [optional] 

### Return type

[**BilanzReport**](BilanzReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## guvReportApi

> GuVReport guvReportApi(opts)

Gewinn- und Verlustrechnung (P&amp;L statement)

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReportsApi();
let opts = {
  'year': 56, // Number | 
  'month': 56, // Number | 
  'dateFrom': "dateFrom_example", // String | 
  'dateTo': "dateTo_example", // String | 
  'page': 56, // Number | 
  'pageSize': 56 // Number | 
};
apiInstance.guvReportApi(opts, (error, data, response) => {
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
 **month** | **Number**|  | [optional] 
 **dateFrom** | **String**|  | [optional] 
 **dateTo** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] 
 **pageSize** | **Number**|  | [optional] 

### Return type

[**GuVReport**](GuVReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## kontenansichtReportApi

> KontoReport kontenansichtReportApi(opts)

Kontenansicht (Account Overview)

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReportsApi();
let opts = {
  'year': 56, // Number | 
  'month': 56, // Number | 
  'dateFrom': "dateFrom_example", // String | 
  'dateTo': "dateTo_example", // String | 
  'page': 56, // Number | 
  'pageSize': 56 // Number | 
};
apiInstance.kontenansichtReportApi(opts, (error, data, response) => {
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
 **month** | **Number**|  | [optional] 
 **dateFrom** | **String**|  | [optional] 
 **dateTo** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] 
 **pageSize** | **Number**|  | [optional] 

### Return type

[**KontoReport**](KontoReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## umsatzsteuerReportApi

> UmsatzsteuerReport umsatzsteuerReportApi(opts)

Umsatzsteuer-Voranmeldung (VAT report)

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.ReportsApi();
let opts = {
  'year': 56, // Number | 
  'month': 56, // Number | 
  'dateFrom': "dateFrom_example", // String | 
  'dateTo': "dateTo_example", // String | 
  'page': 56, // Number | 
  'pageSize': 56 // Number | 
};
apiInstance.umsatzsteuerReportApi(opts, (error, data, response) => {
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
 **month** | **Number**|  | [optional] 
 **dateFrom** | **String**|  | [optional] 
 **dateTo** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] 
 **pageSize** | **Number**|  | [optional] 

### Return type

[**UmsatzsteuerReport**](UmsatzsteuerReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


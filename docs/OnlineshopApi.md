# SimpleBillyApi.OnlineshopApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getSmtpConfigApi**](OnlineshopApi.md#getSmtpConfigApi) | **GET** /api/v1/settings/smtp | 
[**saveSmtpConfigApi**](OnlineshopApi.md#saveSmtpConfigApi) | **PUT** /api/v1/settings/smtp | 



## getSmtpConfigApi

> SmtpConfig getSmtpConfigApi()



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.OnlineshopApi();
apiInstance.getSmtpConfigApi((error, data, response) => {
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

[**SmtpConfig**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## saveSmtpConfigApi

> SmtpConfig saveSmtpConfigApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.OnlineshopApi();
let opts = {
  'smtpConfig': new SimpleBillyApi.SmtpConfig() // SmtpConfig | 
};
apiInstance.saveSmtpConfigApi(opts, (error, data, response) => {
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
 **smtpConfig** | [**SmtpConfig**](SmtpConfig.md)|  | [optional] 

### Return type

[**SmtpConfig**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


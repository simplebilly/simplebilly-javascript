# SimpleBillyApi.EmailTemplateApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createEmailTemplate**](EmailTemplateApi.md#createEmailTemplate) | **POST** /api/v1/email-templates | 
[**deleteEmailTemplate**](EmailTemplateApi.md#deleteEmailTemplate) | **DELETE** /api/v1/email-templates/{email_template_id} | 
[**getEmailTemplate**](EmailTemplateApi.md#getEmailTemplate) | **GET** /api/v1/email-templates/{email_template_id} | 
[**listEmailTemplates**](EmailTemplateApi.md#listEmailTemplates) | **GET** /api/v1/email-templates/ | 
[**renderEmailTemplate**](EmailTemplateApi.md#renderEmailTemplate) | **POST** /api/v1/email-templates/{email_template_id}/render | 
[**updateEmailTemplate**](EmailTemplateApi.md#updateEmailTemplate) | **PUT** /api/v1/email-templates/{email_template_id} | 



## createEmailTemplate

> EmailTemplate createEmailTemplate(emailTemplateCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmailTemplateApi();
let emailTemplateCreate = new SimpleBillyApi.EmailTemplateCreate(); // EmailTemplateCreate | 
apiInstance.createEmailTemplate(emailTemplateCreate, (error, data, response) => {
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
 **emailTemplateCreate** | [**EmailTemplateCreate**](EmailTemplateCreate.md)|  | 

### Return type

[**EmailTemplate**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteEmailTemplate

> deleteEmailTemplate(emailTemplateId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmailTemplateApi();
let emailTemplateId = "emailTemplateId_example"; // String | 
apiInstance.deleteEmailTemplate(emailTemplateId, (error, data, response) => {
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
 **emailTemplateId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getEmailTemplate

> EmailTemplate getEmailTemplate(emailTemplateId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmailTemplateApi();
let emailTemplateId = "emailTemplateId_example"; // String | 
apiInstance.getEmailTemplate(emailTemplateId, (error, data, response) => {
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
 **emailTemplateId** | **String**|  | 

### Return type

[**EmailTemplate**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listEmailTemplates

> [EmailTemplate] listEmailTemplates(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmailTemplateApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'status': "status_example", // String | 
  'search': "search_example" // String | 
};
apiInstance.listEmailTemplates(opts, (error, data, response) => {
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
 **search** | **String**|  | [optional] 

### Return type

[**[EmailTemplate]**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## renderEmailTemplate

> Object renderEmailTemplate(emailTemplateId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmailTemplateApi();
let emailTemplateId = "emailTemplateId_example"; // String | 
let body = null; // Object | 
apiInstance.renderEmailTemplate(emailTemplateId, body, (error, data, response) => {
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
 **emailTemplateId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

**Object**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateEmailTemplate

> EmailTemplate updateEmailTemplate(emailTemplateId, emailTemplateUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.EmailTemplateApi();
let emailTemplateId = "emailTemplateId_example"; // String | 
let emailTemplateUpdate = new SimpleBillyApi.EmailTemplateUpdate(); // EmailTemplateUpdate | 
apiInstance.updateEmailTemplate(emailTemplateId, emailTemplateUpdate, (error, data, response) => {
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
 **emailTemplateId** | **String**|  | 
 **emailTemplateUpdate** | [**EmailTemplateUpdate**](EmailTemplateUpdate.md)|  | 

### Return type

[**EmailTemplate**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


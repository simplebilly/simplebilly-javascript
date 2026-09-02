# SimpleBillyApi.AttachmentVersionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAttachmentVersion**](AttachmentVersionApi.md#createAttachmentVersion) | **POST** /api/v1/attachments/{attachment_id}/versions | 
[**listAttachmentVersions**](AttachmentVersionApi.md#listAttachmentVersions) | **GET** /api/v1/attachments/{attachment_id}/versions | 
[**restoreAttachmentVersion**](AttachmentVersionApi.md#restoreAttachmentVersion) | **POST** /api/v1/attachments/{attachment_id}/versions/{version_id}/restore | 



## createAttachmentVersion

> AttachmentVersion createAttachmentVersion(attachmentId, newVersionRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.AttachmentVersionApi();
let attachmentId = "attachmentId_example"; // String | 
let newVersionRequest = new SimpleBillyApi.NewVersionRequest(); // NewVersionRequest | 
apiInstance.createAttachmentVersion(attachmentId, newVersionRequest, (error, data, response) => {
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
 **attachmentId** | **String**|  | 
 **newVersionRequest** | [**NewVersionRequest**](NewVersionRequest.md)|  | 

### Return type

[**AttachmentVersion**](AttachmentVersion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## listAttachmentVersions

> [AttachmentVersion] listAttachmentVersions(attachmentId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.AttachmentVersionApi();
let attachmentId = "attachmentId_example"; // String | 
apiInstance.listAttachmentVersions(attachmentId, (error, data, response) => {
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
 **attachmentId** | **String**|  | 

### Return type

[**[AttachmentVersion]**](AttachmentVersion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## restoreAttachmentVersion

> Attachment restoreAttachmentVersion(attachmentId, versionId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.AttachmentVersionApi();
let attachmentId = "attachmentId_example"; // String | 
let versionId = "versionId_example"; // String | 
apiInstance.restoreAttachmentVersion(attachmentId, versionId, (error, data, response) => {
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
 **attachmentId** | **String**|  | 
 **versionId** | **String**|  | 

### Return type

[**Attachment**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


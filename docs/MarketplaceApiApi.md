# SimpleBillyApi.MarketplaceApiApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createConnectionApi**](MarketplaceApiApi.md#createConnectionApi) | **POST** /api/v1/marketplace/connections | Create a new connection (for API-key based platforms)
[**deleteConnectionApi**](MarketplaceApiApi.md#deleteConnectionApi) | **DELETE** /api/v1/marketplace/connections/{connection_id} | Soft-delete a connection
[**getConnectionApi**](MarketplaceApiApi.md#getConnectionApi) | **GET** /api/v1/marketplace/connections/{connection_id} | Get a single connection
[**getSyncDirectionApi**](MarketplaceApiApi.md#getSyncDirectionApi) | **GET** /api/v1/marketplace/connections/{connection_id}/directions | Get current sync direction configuration for a connection
[**getSyncLogsApi**](MarketplaceApiApi.md#getSyncLogsApi) | **GET** /api/v1/marketplace/connections/{connection_id}/logs | Get sync logs for a connection
[**listConnectionsApi**](MarketplaceApiApi.md#listConnectionsApi) | **GET** /api/v1/marketplace/connections | List connections for the current tenant
[**listPlatformsApi**](MarketplaceApiApi.md#listPlatformsApi) | **GET** /api/v1/marketplace/platforms | List all supported platforms
[**oauthAuthorizeApi**](MarketplaceApiApi.md#oauthAuthorizeApi) | **POST** /api/v1/marketplace/oauth/authorize | OAuth: initiate authorization flow
[**oauthCallbackApi**](MarketplaceApiApi.md#oauthCallbackApi) | **POST** /api/v1/marketplace/oauth/callback | OAuth: handle callback after authorization
[**triggerSyncApi**](MarketplaceApiApi.md#triggerSyncApi) | **POST** /api/v1/marketplace/connections/{connection_id}/sync | Trigger sync for a connection
[**updateConnectionApi**](MarketplaceApiApi.md#updateConnectionApi) | **PUT** /api/v1/marketplace/connections/{connection_id} | Update a connection
[**updateSyncDirectionApi**](MarketplaceApiApi.md#updateSyncDirectionApi) | **PUT** /api/v1/marketplace/connections/{connection_id}/directions | Update per-entity sync direction configuration for a connection
[**webhookReceiverApi**](MarketplaceApiApi.md#webhookReceiverApi) | **POST** /api/v1/marketplace/webhook/{platform}/{connection_id} | Webhook receiver



## createConnectionApi

> MarketplaceConnection createConnectionApi(createConnectionRequest)

Create a new connection (for API-key based platforms)

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let createConnectionRequest = new SimpleBillyApi.CreateConnectionRequest(); // CreateConnectionRequest | 
apiInstance.createConnectionApi(createConnectionRequest, (error, data, response) => {
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
 **createConnectionRequest** | [**CreateConnectionRequest**](CreateConnectionRequest.md)|  | 

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteConnectionApi

> deleteConnectionApi(connectionId)

Soft-delete a connection

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let connectionId = "connectionId_example"; // String | 
apiInstance.deleteConnectionApi(connectionId, (error, data, response) => {
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
 **connectionId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getConnectionApi

> MarketplaceConnection getConnectionApi(connectionId)

Get a single connection

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let connectionId = "connectionId_example"; // String | 
apiInstance.getConnectionApi(connectionId, (error, data, response) => {
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
 **connectionId** | **String**|  | 

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getSyncDirectionApi

> getSyncDirectionApi(connectionId)

Get current sync direction configuration for a connection

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let connectionId = "connectionId_example"; // String | 
apiInstance.getSyncDirectionApi(connectionId, (error, data, response) => {
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
 **connectionId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getSyncLogsApi

> [SyncLog] getSyncLogsApi(connectionId)

Get sync logs for a connection

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let connectionId = "connectionId_example"; // String | 
apiInstance.getSyncLogsApi(connectionId, (error, data, response) => {
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
 **connectionId** | **String**|  | 

### Return type

[**[SyncLog]**](SyncLog.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listConnectionsApi

> [MarketplaceConnection] listConnectionsApi()

List connections for the current tenant

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
apiInstance.listConnectionsApi((error, data, response) => {
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

[**[MarketplaceConnection]**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPlatformsApi

> [PlatformInfo] listPlatformsApi()

List all supported platforms

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
apiInstance.listPlatformsApi((error, data, response) => {
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

[**[PlatformInfo]**](PlatformInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## oauthAuthorizeApi

> OAuthAuthorizeResponse oauthAuthorizeApi(oAuthAuthorizeRequest)

OAuth: initiate authorization flow

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let oAuthAuthorizeRequest = new SimpleBillyApi.OAuthAuthorizeRequest(); // OAuthAuthorizeRequest | 
apiInstance.oauthAuthorizeApi(oAuthAuthorizeRequest, (error, data, response) => {
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
 **oAuthAuthorizeRequest** | [**OAuthAuthorizeRequest**](OAuthAuthorizeRequest.md)|  | 

### Return type

[**OAuthAuthorizeResponse**](OAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## oauthCallbackApi

> MarketplaceConnection oauthCallbackApi(oAuthCallbackRequest)

OAuth: handle callback after authorization

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let oAuthCallbackRequest = new SimpleBillyApi.OAuthCallbackRequest(); // OAuthCallbackRequest | 
apiInstance.oauthCallbackApi(oAuthCallbackRequest, (error, data, response) => {
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
 **oAuthCallbackRequest** | [**OAuthCallbackRequest**](OAuthCallbackRequest.md)|  | 

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## triggerSyncApi

> SyncSummary triggerSyncApi(connectionId, opts)

Trigger sync for a connection

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let connectionId = "connectionId_example"; // String | 
let opts = {
  'syncType': "syncType_example", // String | 
  'direction': "direction_example" // String | 
};
apiInstance.triggerSyncApi(connectionId, opts, (error, data, response) => {
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
 **connectionId** | **String**|  | 
 **syncType** | **String**|  | [optional] 
 **direction** | **String**|  | [optional] 

### Return type

[**SyncSummary**](SyncSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateConnectionApi

> MarketplaceConnection updateConnectionApi(connectionId, updateConnectionRequest)

Update a connection

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let connectionId = "connectionId_example"; // String | 
let updateConnectionRequest = new SimpleBillyApi.UpdateConnectionRequest(); // UpdateConnectionRequest | 
apiInstance.updateConnectionApi(connectionId, updateConnectionRequest, (error, data, response) => {
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
 **connectionId** | **String**|  | 
 **updateConnectionRequest** | [**UpdateConnectionRequest**](UpdateConnectionRequest.md)|  | 

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateSyncDirectionApi

> updateSyncDirectionApi(connectionId, updateSyncDirectionRequest)

Update per-entity sync direction configuration for a connection

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let connectionId = "connectionId_example"; // String | 
let updateSyncDirectionRequest = new SimpleBillyApi.UpdateSyncDirectionRequest(); // UpdateSyncDirectionRequest | 
apiInstance.updateSyncDirectionApi(connectionId, updateSyncDirectionRequest, (error, data, response) => {
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
 **connectionId** | **String**|  | 
 **updateSyncDirectionRequest** | [**UpdateSyncDirectionRequest**](UpdateSyncDirectionRequest.md)|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## webhookReceiverApi

> webhookReceiverApi(platform, connectionId)

Webhook receiver

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.MarketplaceApiApi();
let platform = "platform_example"; // String | 
let connectionId = "connectionId_example"; // String | 
apiInstance.webhookReceiverApi(platform, connectionId, (error, data, response) => {
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
 **platform** | **String**|  | 
 **connectionId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


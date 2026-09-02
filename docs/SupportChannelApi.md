# SimpleBillyApi.SupportChannelApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createChannelApi**](SupportChannelApi.md#createChannelApi) | **POST** /api/v1/support/channels | 
[**deleteChannelApi**](SupportChannelApi.md#deleteChannelApi) | **DELETE** /api/v1/support/channels/{channel_id} | 
[**listChannelsApi**](SupportChannelApi.md#listChannelsApi) | **GET** /api/v1/support/channels | 
[**updateChannelApi**](SupportChannelApi.md#updateChannelApi) | **PUT** /api/v1/support/channels/{channel_id} | 



## createChannelApi

> SupportChannel createChannelApi(createChannelDto)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupportChannelApi();
let createChannelDto = new SimpleBillyApi.CreateChannelDto(); // CreateChannelDto | 
apiInstance.createChannelApi(createChannelDto, (error, data, response) => {
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
 **createChannelDto** | [**CreateChannelDto**](CreateChannelDto.md)|  | 

### Return type

[**SupportChannel**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteChannelApi

> deleteChannelApi(channelId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupportChannelApi();
let channelId = "channelId_example"; // String | 
apiInstance.deleteChannelApi(channelId, (error, data, response) => {
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
 **channelId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## listChannelsApi

> [SupportChannel] listChannelsApi()



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupportChannelApi();
apiInstance.listChannelsApi((error, data, response) => {
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

[**[SupportChannel]**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateChannelApi

> SupportChannel updateChannelApi(channelId, updateChannelDto)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupportChannelApi();
let channelId = "channelId_example"; // String | 
let updateChannelDto = new SimpleBillyApi.UpdateChannelDto(); // UpdateChannelDto | 
apiInstance.updateChannelApi(channelId, updateChannelDto, (error, data, response) => {
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
 **channelId** | **String**|  | 
 **updateChannelDto** | [**UpdateChannelDto**](UpdateChannelDto.md)|  | 

### Return type

[**SupportChannel**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


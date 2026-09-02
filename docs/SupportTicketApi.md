# SimpleBillyApi.SupportTicketApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createTicketApi**](SupportTicketApi.md#createTicketApi) | **POST** /api/v1/support/tickets | 
[**deleteTicketApi**](SupportTicketApi.md#deleteTicketApi) | **DELETE** /api/v1/support/tickets/{ticket_id} | 
[**getTicketApi**](SupportTicketApi.md#getTicketApi) | **GET** /api/v1/support/tickets/{ticket_id} | 
[**listTicketsApi**](SupportTicketApi.md#listTicketsApi) | **GET** /api/v1/support/tickets | 
[**updateTicketApi**](SupportTicketApi.md#updateTicketApi) | **PUT** /api/v1/support/tickets/{ticket_id} | 



## createTicketApi

> SupportTicket createTicketApi(createTicketRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupportTicketApi();
let createTicketRequest = new SimpleBillyApi.CreateTicketRequest(); // CreateTicketRequest | 
apiInstance.createTicketApi(createTicketRequest, (error, data, response) => {
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
 **createTicketRequest** | [**CreateTicketRequest**](CreateTicketRequest.md)|  | 

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteTicketApi

> deleteTicketApi(ticketId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupportTicketApi();
let ticketId = "ticketId_example"; // String | 
apiInstance.deleteTicketApi(ticketId, (error, data, response) => {
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
 **ticketId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getTicketApi

> SupportTicket getTicketApi(ticketId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupportTicketApi();
let ticketId = "ticketId_example"; // String | 
apiInstance.getTicketApi(ticketId, (error, data, response) => {
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
 **ticketId** | **String**|  | 

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listTicketsApi

> [SupportTicket] listTicketsApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupportTicketApi();
let opts = {
  'status': "status_example", // String | 
  'priority': "priority_example", // String | 
  'assignedTo': "assignedTo_example", // String | 
  'channelType': "channelType_example", // String | 
  'customerId': "customerId_example", // String | 
  'search': "search_example", // String | 
  'page': 56, // Number | 
  'pageSize': 56 // Number | 
};
apiInstance.listTicketsApi(opts, (error, data, response) => {
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
 **status** | **String**|  | [optional] 
 **priority** | **String**|  | [optional] 
 **assignedTo** | **String**|  | [optional] 
 **channelType** | **String**|  | [optional] 
 **customerId** | **String**|  | [optional] 
 **search** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] 
 **pageSize** | **Number**|  | [optional] 

### Return type

[**[SupportTicket]**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateTicketApi

> SupportTicket updateTicketApi(ticketId, supportTicketUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.SupportTicketApi();
let ticketId = "ticketId_example"; // String | 
let supportTicketUpdate = new SimpleBillyApi.SupportTicketUpdate(); // SupportTicketUpdate | 
apiInstance.updateTicketApi(ticketId, supportTicketUpdate, (error, data, response) => {
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
 **ticketId** | **String**|  | 
 **supportTicketUpdate** | [**SupportTicketUpdate**](SupportTicketUpdate.md)|  | 

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


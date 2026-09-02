# SimpleBillyApi.TicketMessageApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listMessagesApi**](TicketMessageApi.md#listMessagesApi) | **GET** /api/v1/support/tickets/{ticket_id}/messages | 
[**sendMessageApi**](TicketMessageApi.md#sendMessageApi) | **POST** /api/v1/support/tickets/{ticket_id}/messages | 



## listMessagesApi

> [TicketMessage] listMessagesApi(ticketId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TicketMessageApi();
let ticketId = "ticketId_example"; // String | 
apiInstance.listMessagesApi(ticketId, (error, data, response) => {
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

[**[TicketMessage]**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## sendMessageApi

> TicketMessage sendMessageApi(ticketId, sendMessageDto)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TicketMessageApi();
let ticketId = "ticketId_example"; // String | 
let sendMessageDto = new SimpleBillyApi.SendMessageDto(); // SendMessageDto | 
apiInstance.sendMessageApi(ticketId, sendMessageDto, (error, data, response) => {
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
 **sendMessageDto** | [**SendMessageDto**](SendMessageDto.md)|  | 

### Return type

[**TicketMessage**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


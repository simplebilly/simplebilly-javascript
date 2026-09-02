# SimpleBillyApi.CustomerCommunicationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createCommunication**](CustomerCommunicationApi.md#createCommunication) | **POST** /api/v1/communications | 
[**customercommunicationRestore**](CustomerCommunicationApi.md#customercommunicationRestore) | **POST** /api/v1/communications/{communication_id}/restore | 
[**deleteCommunication**](CustomerCommunicationApi.md#deleteCommunication) | **DELETE** /api/v1/communications/{communication_id} | 
[**getCommunication**](CustomerCommunicationApi.md#getCommunication) | **GET** /api/v1/communications/{communication_id} | 
[**getContactHistory**](CustomerCommunicationApi.md#getContactHistory) | **GET** /api/v1/contacts/{contact_id}/communications | 
[**listCommunications**](CustomerCommunicationApi.md#listCommunications) | **GET** /api/v1/communications/ | 
[**updateCommunication**](CustomerCommunicationApi.md#updateCommunication) | **PUT** /api/v1/communications/{communication_id} | 



## createCommunication

> CustomerCommunication createCommunication(customerCommunicationCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerCommunicationApi();
let customerCommunicationCreate = new SimpleBillyApi.CustomerCommunicationCreate(); // CustomerCommunicationCreate | 
apiInstance.createCommunication(customerCommunicationCreate, (error, data, response) => {
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
 **customerCommunicationCreate** | [**CustomerCommunicationCreate**](CustomerCommunicationCreate.md)|  | 

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## customercommunicationRestore

> CustomerCommunication customercommunicationRestore(communicationId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerCommunicationApi();
let communicationId = "communicationId_example"; // String | 
apiInstance.customercommunicationRestore(communicationId, (error, data, response) => {
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
 **communicationId** | **String**|  | 

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## deleteCommunication

> deleteCommunication(communicationId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerCommunicationApi();
let communicationId = "communicationId_example"; // String | 
apiInstance.deleteCommunication(communicationId, (error, data, response) => {
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
 **communicationId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCommunication

> CustomerCommunication getCommunication(communicationId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerCommunicationApi();
let communicationId = "communicationId_example"; // String | 
apiInstance.getCommunication(communicationId, (error, data, response) => {
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
 **communicationId** | **String**|  | 

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getContactHistory

> ContactHistoryResponse getContactHistory(contactId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerCommunicationApi();
let contactId = "contactId_example"; // String | 
apiInstance.getContactHistory(contactId, (error, data, response) => {
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
 **contactId** | **String**|  | 

### Return type

[**ContactHistoryResponse**](ContactHistoryResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listCommunications

> [CustomerCommunication] listCommunications(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerCommunicationApi();
let opts = {
  'page': 56, // Number | 
  'pageSize': 56, // Number | 
  'contactId': "contactId_example", // String | Filter history to a single contact.
  'channel': new SimpleBillyApi.CommunicationChannel(), // CommunicationChannel | 
  'direction': new SimpleBillyApi.CommunicationDirection(), // CommunicationDirection | 
  'from': new Date("2013-10-20"), // Date | Only include communications after this ISO date (inclusive).
  'to': new Date("2013-10-20") // Date | Only include communications before this ISO date (inclusive).
};
apiInstance.listCommunications(opts, (error, data, response) => {
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
 **contactId** | **String**| Filter history to a single contact. | [optional] 
 **channel** | [**CommunicationChannel**](.md)|  | [optional] 
 **direction** | [**CommunicationDirection**](.md)|  | [optional] 
 **from** | **Date**| Only include communications after this ISO date (inclusive). | [optional] 
 **to** | **Date**| Only include communications before this ISO date (inclusive). | [optional] 

### Return type

[**[CustomerCommunication]**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateCommunication

> CustomerCommunication updateCommunication(communicationId, customerCommunicationUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerCommunicationApi();
let communicationId = "communicationId_example"; // String | 
let customerCommunicationUpdate = new SimpleBillyApi.CustomerCommunicationUpdate(); // CustomerCommunicationUpdate | 
apiInstance.updateCommunication(communicationId, customerCommunicationUpdate, (error, data, response) => {
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
 **communicationId** | **String**|  | 
 **customerCommunicationUpdate** | [**CustomerCommunicationUpdate**](CustomerCommunicationUpdate.md)|  | 

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


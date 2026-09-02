# SimpleBillyApi.CustomerGroupApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addGroupMembers**](CustomerGroupApi.md#addGroupMembers) | **POST** /api/v1/customer-groups/{customer_group_id}/members | 
[**createCustomerGroup**](CustomerGroupApi.md#createCustomerGroup) | **POST** /api/v1/customer-groups | 
[**deleteCustomerGroup**](CustomerGroupApi.md#deleteCustomerGroup) | **DELETE** /api/v1/customer-groups/{customer_group_id} | 
[**getCustomerGroup**](CustomerGroupApi.md#getCustomerGroup) | **GET** /api/v1/customer-groups/{customer_group_id} | 
[**listCustomerGroups**](CustomerGroupApi.md#listCustomerGroups) | **GET** /api/v1/customer-groups/ | 
[**updateCustomerGroup**](CustomerGroupApi.md#updateCustomerGroup) | **PUT** /api/v1/customer-groups/{customer_group_id} | 



## addGroupMembers

> CustomerGroup addGroupMembers(customerGroupId, body)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerGroupApi();
let customerGroupId = "customerGroupId_example"; // String | 
let body = null; // Object | 
apiInstance.addGroupMembers(customerGroupId, body, (error, data, response) => {
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
 **customerGroupId** | **String**|  | 
 **body** | **Object**|  | 

### Return type

[**CustomerGroup**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createCustomerGroup

> CustomerGroup createCustomerGroup(customerGroupCreate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerGroupApi();
let customerGroupCreate = new SimpleBillyApi.CustomerGroupCreate(); // CustomerGroupCreate | 
apiInstance.createCustomerGroup(customerGroupCreate, (error, data, response) => {
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
 **customerGroupCreate** | [**CustomerGroupCreate**](CustomerGroupCreate.md)|  | 

### Return type

[**CustomerGroup**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteCustomerGroup

> deleteCustomerGroup(customerGroupId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerGroupApi();
let customerGroupId = "customerGroupId_example"; // String | 
apiInstance.deleteCustomerGroup(customerGroupId, (error, data, response) => {
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
 **customerGroupId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCustomerGroup

> CustomerGroup getCustomerGroup(customerGroupId)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerGroupApi();
let customerGroupId = "customerGroupId_example"; // String | 
apiInstance.getCustomerGroup(customerGroupId, (error, data, response) => {
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
 **customerGroupId** | **String**|  | 

### Return type

[**CustomerGroup**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listCustomerGroups

> [CustomerGroup] listCustomerGroups(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerGroupApi();
let opts = {
  'page': 1, // Number | 
  'pageSize': 56, // Number | 
  'search': "search_example", // String | 
  'includeDeleted': true // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
};
apiInstance.listCustomerGroups(opts, (error, data, response) => {
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
 **search** | **String**|  | [optional] 
 **includeDeleted** | **Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] 

### Return type

[**[CustomerGroup]**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateCustomerGroup

> CustomerGroup updateCustomerGroup(customerGroupId, customerGroupUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CustomerGroupApi();
let customerGroupId = "customerGroupId_example"; // String | 
let customerGroupUpdate = new SimpleBillyApi.CustomerGroupUpdate(); // CustomerGroupUpdate | 
apiInstance.updateCustomerGroup(customerGroupId, customerGroupUpdate, (error, data, response) => {
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
 **customerGroupId** | **String**|  | 
 **customerGroupUpdate** | [**CustomerGroupUpdate**](CustomerGroupUpdate.md)|  | 

### Return type

[**CustomerGroup**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


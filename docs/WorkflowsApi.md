# SimpleBillyApi.WorkflowsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listWorkflowsApi**](WorkflowsApi.md#listWorkflowsApi) | **GET** /api/v1/workflows | 
[**setWorkflowEnabledApi**](WorkflowsApi.md#setWorkflowEnabledApi) | **PUT** /api/v1/workflows/{workflow_id}/enabled | 



## listWorkflowsApi

> [Workflow] listWorkflowsApi()



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.WorkflowsApi();
apiInstance.listWorkflowsApi((error, data, response) => {
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

[**[Workflow]**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## setWorkflowEnabledApi

> Workflow setWorkflowEnabledApi(workflowId, workflowEnabledUpdate)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.WorkflowsApi();
let workflowId = "workflowId_example"; // String | 
let workflowEnabledUpdate = new SimpleBillyApi.WorkflowEnabledUpdate(); // WorkflowEnabledUpdate | 
apiInstance.setWorkflowEnabledApi(workflowId, workflowEnabledUpdate, (error, data, response) => {
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
 **workflowId** | **String**|  | 
 **workflowEnabledUpdate** | [**WorkflowEnabledUpdate**](WorkflowEnabledUpdate.md)|  | 

### Return type

[**Workflow**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


# SimpleBillyApi.BudgetsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**budgetsApi**](BudgetsApi.md#budgetsApi) | **GET** /api/v1/bookkeeping/budgets | 
[**upsertBudgetGoalApi**](BudgetsApi.md#upsertBudgetGoalApi) | **PUT** /api/v1/bookkeeping/budgets/goals/{category} | 



## budgetsApi

> BudgetErgebnis budgetsApi(year, month)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.BudgetsApi();
let year = 56; // Number | 
let month = 56; // Number | 
apiInstance.budgetsApi(year, month, (error, data, response) => {
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
 **year** | **Number**|  | 
 **month** | **Number**|  | 

### Return type

[**BudgetErgebnis**](BudgetErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## upsertBudgetGoalApi

> Budget upsertBudgetGoalApi(category, budgetGoalRequest)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.BudgetsApi();
let category = "category_example"; // String | 
let budgetGoalRequest = new SimpleBillyApi.BudgetGoalRequest(); // BudgetGoalRequest | 
apiInstance.upsertBudgetGoalApi(category, budgetGoalRequest, (error, data, response) => {
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
 **category** | **String**|  | 
 **budgetGoalRequest** | [**BudgetGoalRequest**](BudgetGoalRequest.md)|  | 

### Return type

[**Budget**](Budget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


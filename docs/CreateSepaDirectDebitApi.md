# SimpleBillyApi.CreateSepaDirectDebitApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSepaDirectDebitApi**](CreateSepaDirectDebitApi.md#createSepaDirectDebitApi) | **POST** /api/v1/bookkeeping/sepa-direct-debit | 



## createSepaDirectDebitApi

> SepaDirectDebitResponse createSepaDirectDebitApi(creditorName, creditorIban, creditorId, mandateId, mandateDate, debtorName, debtorIban, amount, collectionDate, opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.CreateSepaDirectDebitApi();
let creditorName = "creditorName_example"; // String | 
let creditorIban = "creditorIban_example"; // String | 
let creditorId = "creditorId_example"; // String | 
let mandateId = "mandateId_example"; // String | 
let mandateDate = "mandateDate_example"; // String | 
let debtorName = "debtorName_example"; // String | 
let debtorIban = "debtorIban_example"; // String | 
let amount = "amount_example"; // String | 
let collectionDate = "collectionDate_example"; // String | 
let opts = {
  'creditorBic': "creditorBic_example", // String | 
  'debtorBic': "debtorBic_example", // String | 
  'description': "description_example" // String | 
};
apiInstance.createSepaDirectDebitApi(creditorName, creditorIban, creditorId, mandateId, mandateDate, debtorName, debtorIban, amount, collectionDate, opts, (error, data, response) => {
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
 **creditorName** | **String**|  | 
 **creditorIban** | **String**|  | 
 **creditorId** | **String**|  | 
 **mandateId** | **String**|  | 
 **mandateDate** | **String**|  | 
 **debtorName** | **String**|  | 
 **debtorIban** | **String**|  | 
 **amount** | **String**|  | 
 **collectionDate** | **String**|  | 
 **creditorBic** | **String**|  | [optional] 
 **debtorBic** | **String**|  | [optional] 
 **description** | **String**|  | [optional] 

### Return type

[**SepaDirectDebitResponse**](SepaDirectDebitResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


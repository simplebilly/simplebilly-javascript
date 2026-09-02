# SimpleBillyApi.BankingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bankLookupApi**](BankingApi.md#bankLookupApi) | **GET** /api/v1/bookkeeping/banking/lookup | 
[**bankTransactionsApi**](BankingApi.md#bankTransactionsApi) | **GET** /api/v1/bookkeeping/banking/transactions | 
[**hebesatzLookupApi**](BankingApi.md#hebesatzLookupApi) | **GET** /api/v1/bookkeeping/hebesatz | 



## bankLookupApi

> BankLookup bankLookupApi(iban)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.BankingApi();
let iban = "iban_example"; // String | 
apiInstance.bankLookupApi(iban, (error, data, response) => {
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
 **iban** | **String**|  | 

### Return type

[**BankLookup**](BankLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## bankTransactionsApi

> bankTransactionsApi()



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.BankingApi();
apiInstance.bankTransactionsApi((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## hebesatzLookupApi

> [HebesatzLookup] hebesatzLookupApi(opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.BankingApi();
let opts = {
  'gemeindeschluessel': "gemeindeschluessel_example", // String | 
  'plz': "plz_example", // String | 
  'name': "name_example", // String | 
  'stichtag': "stichtag_example", // String | Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from <= date <= valid_to.
  'countryCode': "countryCode_example" // String | 
};
apiInstance.hebesatzLookupApi(opts, (error, data, response) => {
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
 **gemeindeschluessel** | **String**|  | [optional] 
 **plz** | **String**|  | [optional] 
 **name** | **String**|  | [optional] 
 **stichtag** | **String**| Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from &lt;&#x3D; date &lt;&#x3D; valid_to. | [optional] 
 **countryCode** | **String**|  | [optional] 

### Return type

[**[HebesatzLookup]**](HebesatzLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


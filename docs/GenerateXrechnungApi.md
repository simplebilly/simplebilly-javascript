# SimpleBillyApi.GenerateXrechnungApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generateXrechnungApi**](GenerateXrechnungApi.md#generateXrechnungApi) | **GET** /api/v1/invoices/{id}/xrechnung | 



## generateXrechnungApi

> XRechnungResponse generateXrechnungApi(id, opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.GenerateXrechnungApi();
let id = "id_example"; // String | 
let opts = {
  'supplierName': "supplierName_example", // String | 
  'supplierStreet': "supplierStreet_example", // String | 
  'supplierCity': "supplierCity_example", // String | 
  'supplierZip': "supplierZip_example", // String | 
  'supplierCountry': "supplierCountry_example", // String | 
  'supplierVatId': "supplierVatId_example" // String | 
};
apiInstance.generateXrechnungApi(id, opts, (error, data, response) => {
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
 **id** | **String**|  | 
 **supplierName** | **String**|  | [optional] 
 **supplierStreet** | **String**|  | [optional] 
 **supplierCity** | **String**|  | [optional] 
 **supplierZip** | **String**|  | [optional] 
 **supplierCountry** | **String**|  | [optional] 
 **supplierVatId** | **String**|  | [optional] 

### Return type

[**XRechnungResponse**](XRechnungResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


# SimpleBillyApi.GenerateQrcodeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generateQrcodeApi**](GenerateQrcodeApi.md#generateQrcodeApi) | **GET** /api/v1/invoices/{id}/qrcode | 



## generateQrcodeApi

> QRCodeResponse generateQrcodeApi(iban, id, opts)



### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.GenerateQrcodeApi();
let iban = "iban_example"; // String | 
let id = "id_example"; // String | 
let opts = {
  'holderName': "holderName_example", // String | 
  'bic': "bic_example", // String | 
  'amount': "amount_example", // String | 
  'reference': "reference_example", // String | 
  'purpose': "purpose_example" // String | 
};
apiInstance.generateQrcodeApi(iban, id, opts, (error, data, response) => {
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
 **id** | **String**|  | 
 **holderName** | **String**|  | [optional] 
 **bic** | **String**|  | [optional] 
 **amount** | **String**|  | [optional] 
 **reference** | **String**|  | [optional] 
 **purpose** | **String**|  | [optional] 

### Return type

[**QRCodeResponse**](QRCodeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


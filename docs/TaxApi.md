# SimpleBillyApi.TaxApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createTaxRate**](TaxApi.md#createTaxRate) | **POST** /api/v1/tax-rates | Create a tax rate (&#x60;admin:settings&#x60;).
[**deleteTaxRate**](TaxApi.md#deleteTaxRate) | **DELETE** /api/v1/tax-rates/{id} | Delete a tax rate by id (&#x60;admin:settings&#x60;).
[**listTaxRates**](TaxApi.md#listTaxRates) | **GET** /api/v1/tax-rates | List the calling tenant&#39;s tax rates.
[**updateTaxRate**](TaxApi.md#updateTaxRate) | **PUT** /api/v1/tax-rates/{id} | Update a tax rate by id (&#x60;admin:settings&#x60;). Replaces all body fields.



## createTaxRate

> createTaxRate(taxRateCreate)

Create a tax rate (&#x60;admin:settings&#x60;).

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TaxApi();
let taxRateCreate = new SimpleBillyApi.TaxRateCreate(); // TaxRateCreate | 
apiInstance.createTaxRate(taxRateCreate, (error, data, response) => {
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
 **taxRateCreate** | [**TaxRateCreate**](TaxRateCreate.md)|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## deleteTaxRate

> deleteTaxRate(id)

Delete a tax rate by id (&#x60;admin:settings&#x60;).

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TaxApi();
let id = "id_example"; // String | 
apiInstance.deleteTaxRate(id, (error, data, response) => {
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
 **id** | **String**|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## listTaxRates

> listTaxRates()

List the calling tenant&#39;s tax rates.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TaxApi();
apiInstance.listTaxRates((error, data, response) => {
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


## updateTaxRate

> updateTaxRate(id, taxRateCreate)

Update a tax rate by id (&#x60;admin:settings&#x60;). Replaces all body fields.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TaxApi();
let id = "id_example"; // String | 
let taxRateCreate = new SimpleBillyApi.TaxRateCreate(); // TaxRateCreate | 
apiInstance.updateTaxRate(id, taxRateCreate, (error, data, response) => {
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
 **id** | **String**|  | 
 **taxRateCreate** | [**TaxRateCreate**](TaxRateCreate.md)|  | 

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


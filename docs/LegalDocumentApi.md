# SimpleBillyApi.LegalDocumentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getLegalDocuments**](LegalDocumentApi.md#getLegalDocuments) | **GET** /api/v1/legal/documents | List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.
[**resetLegalDocuments**](LegalDocumentApi.md#resetLegalDocuments) | **POST** /api/v1/legal/documents/reset | Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.
[**upsertLegalDocuments**](LegalDocumentApi.md#upsertLegalDocuments) | **PUT** /api/v1/legal/documents | Upsert legal documents per (doc_type, lang). Returns the full tenant list.



## getLegalDocuments

> [LegalDocument] getLegalDocuments()

List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.LegalDocumentApi();
apiInstance.getLegalDocuments((error, data, response) => {
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

[**[LegalDocument]**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## resetLegalDocuments

> [LegalDocument] resetLegalDocuments(legalDocumentReset)

Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.LegalDocumentApi();
let legalDocumentReset = new SimpleBillyApi.LegalDocumentReset(); // LegalDocumentReset | 
apiInstance.resetLegalDocuments(legalDocumentReset, (error, data, response) => {
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
 **legalDocumentReset** | [**LegalDocumentReset**](LegalDocumentReset.md)|  | 

### Return type

[**[LegalDocument]**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## upsertLegalDocuments

> [LegalDocument] upsertLegalDocuments(legalDocumentUpsert)

Upsert legal documents per (doc_type, lang). Returns the full tenant list.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.LegalDocumentApi();
let legalDocumentUpsert = [new SimpleBillyApi.LegalDocumentUpsert()]; // [LegalDocumentUpsert] | 
apiInstance.upsertLegalDocuments(legalDocumentUpsert, (error, data, response) => {
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
 **legalDocumentUpsert** | [**[LegalDocumentUpsert]**](LegalDocumentUpsert.md)|  | 

### Return type

[**[LegalDocument]**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


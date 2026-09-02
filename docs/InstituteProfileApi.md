# SimpleBillyApi.InstituteProfileApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getInstituteProfile**](InstituteProfileApi.md#getInstituteProfile) | **GET** /api/v1/institute-profile | Current institute profile (created with defaults when missing).
[**updateInstituteProfile**](InstituteProfileApi.md#updateInstituteProfile) | **PUT** /api/v1/institute-profile | Update the institute profile (institute_type and/or kapitalmarktorientiert).



## getInstituteProfile

> InstituteProfile getInstituteProfile()

Current institute profile (created with defaults when missing).

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.InstituteProfileApi();
apiInstance.getInstituteProfile((error, data, response) => {
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

[**InstituteProfile**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateInstituteProfile

> InstituteProfile updateInstituteProfile(instituteProfileUpdate)

Update the institute profile (institute_type and/or kapitalmarktorientiert).

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.InstituteProfileApi();
let instituteProfileUpdate = new SimpleBillyApi.InstituteProfileUpdate(); // InstituteProfileUpdate | 
apiInstance.updateInstituteProfile(instituteProfileUpdate, (error, data, response) => {
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
 **instituteProfileUpdate** | [**InstituteProfileUpdate**](InstituteProfileUpdate.md)|  | 

### Return type

[**InstituteProfile**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


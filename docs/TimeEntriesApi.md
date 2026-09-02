# SimpleBillyApi.TimeEntriesApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**clockInTimeEntry**](TimeEntriesApi.md#clockInTimeEntry) | **POST** /api/v1/time-entries | Clock in for the authenticated user (resolved via their employee profile).
[**clockOutTimeEntry**](TimeEntriesApi.md#clockOutTimeEntry) | **PATCH** /api/v1/time-entries/{id} | Clock out an entry: the entry&#39;s owner, or anyone with &#x60;time_entries:write&#x60;.
[**getLaborCosts**](TimeEntriesApi.md#getLaborCosts) | **GET** /api/v1/labor-costs | Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee&#39;s hourly cost rate.
[**listTimeEntries**](TimeEntriesApi.md#listTimeEntries) | **GET** /api/v1/time-entries | List time entries with optional date-range / active / employee filters.



## clockInTimeEntry

> TimeEntryDto clockInTimeEntry(timeEntryClockIn)

Clock in for the authenticated user (resolved via their employee profile).

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TimeEntriesApi();
let timeEntryClockIn = new SimpleBillyApi.TimeEntryClockIn(); // TimeEntryClockIn | 
apiInstance.clockInTimeEntry(timeEntryClockIn, (error, data, response) => {
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
 **timeEntryClockIn** | [**TimeEntryClockIn**](TimeEntryClockIn.md)|  | 

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## clockOutTimeEntry

> TimeEntryDto clockOutTimeEntry(id, timeEntryClockOut)

Clock out an entry: the entry&#39;s owner, or anyone with &#x60;time_entries:write&#x60;.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TimeEntriesApi();
let id = "id_example"; // String | 
let timeEntryClockOut = new SimpleBillyApi.TimeEntryClockOut(); // TimeEntryClockOut | 
apiInstance.clockOutTimeEntry(id, timeEntryClockOut, (error, data, response) => {
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
 **timeEntryClockOut** | [**TimeEntryClockOut**](TimeEntryClockOut.md)|  | 

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## getLaborCosts

> [LaborCostRow] getLaborCosts(from, to, groupBy)

Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee&#39;s hourly cost rate.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TimeEntriesApi();
let from = new Date("2013-10-20"); // Date | 
let to = new Date("2013-10-20"); // Date | 
let groupBy = "groupBy_example"; // String | One of \"employee\", \"order\" or \"day\".
apiInstance.getLaborCosts(from, to, groupBy, (error, data, response) => {
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
 **from** | **Date**|  | 
 **to** | **Date**|  | 
 **groupBy** | **String**| One of \&quot;employee\&quot;, \&quot;order\&quot; or \&quot;day\&quot;. | 

### Return type

[**[LaborCostRow]**](LaborCostRow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listTimeEntries

> [TimeEntryDto] listTimeEntries(opts)

List time entries with optional date-range / active / employee filters.

### Example

```javascript
import SimpleBillyApi from 'simple_billy_api';
let defaultClient = SimpleBillyApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearer_token
let bearer_token = defaultClient.authentications['bearer_token'];
bearer_token.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new SimpleBillyApi.TimeEntriesApi();
let opts = {
  'from': new Date("2013-10-20"), // Date | 
  'to': new Date("2013-10-20"), // Date | 
  'active': true, // Boolean | Only currently running shifts (clock_in set, clock_out null).
  'employeeId': "employeeId_example" // String | 
};
apiInstance.listTimeEntries(opts, (error, data, response) => {
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
 **from** | **Date**|  | [optional] 
 **to** | **Date**|  | [optional] 
 **active** | **Boolean**| Only currently running shifts (clock_in set, clock_out null). | [optional] 
 **employeeId** | **String**|  | [optional] 

### Return type

[**[TimeEntryDto]**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


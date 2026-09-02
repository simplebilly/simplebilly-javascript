# SimpleBillyApi.Absence

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**absenceType** | [**AbsenceType**](AbsenceType.md) | One of \&quot;vacation\&quot;, \&quot;sick\&quot;, \&quot;sabbatical\&quot;, \&quot;parental\&quot;, \&quot;other\&quot;. | [optional] 
**approvedAt** | **Date** |  | [optional] 
**approvedBy** | **String** | References the user entity. | [optional] 
**createdAt** | **Date** |  | [optional] 
**deletedAt** | **Date** |  | [optional] 
**employeeId** | **String** | References the employee entity. | [optional] 
**endDate** | **Date** |  | [optional] 
**id** | **String** |  | [optional] 
**notes** | **String** |  | [optional] 
**startDate** | **Date** |  | [optional] 
**status** | [**AbsenceStatus**](AbsenceStatus.md) | One of \&quot;pending\&quot;, \&quot;approved\&quot;, \&quot;rejected\&quot;, \&quot;cancelled\&quot;. | [optional] 
**tenantId** | **String** |  | [optional] 
**updatedAt** | **Date** |  | [optional] 



# SimpleBillyApi.ServiceJobUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **String** | Street + zip + city of the job location. | [optional] 
**customerEmail** | **String** | Customer email for email notifications. | [optional] 
**customerId** | **String** | References the customer entity. | [optional] 
**customerName** | **String** | Denormalized customer name for quick display. | [optional] 
**customerPhone** | **String** | Customer phone for SMS notifications later. | [optional] 
**description** | **String** | What work needs to be done. | [optional] 
**estimatedDurationMinutes** | **Number** | Estimated time for the job in minutes. | [optional] 
**lat** | **Number** | Latitude for map display (OpenStreetMap). | [optional] 
**lng** | **Number** | Longitude for map display (OpenStreetMap). | [optional] 
**notes** | **String** |  | [optional] 
**status** | [**ServiceJobStatus**](ServiceJobStatus.md) | Dispatch status: \&quot;pending\&quot;, \&quot;assigned\&quot;, \&quot;en_route\&quot;, \&quot;in_progress\&quot;, \&quot;completed\&quot;, \&quot;cancelled\&quot;. | [optional] 



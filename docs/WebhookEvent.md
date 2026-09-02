# SimpleBillyApi.WebhookEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attempts** | **Number** |  | [optional] 
**channel** | **String** | source for inbound, target URL for outbound. | [optional] 
**direction** | [**WebhookDirection**](WebhookDirection.md) | inbound | outbound | 
**eventType** | **String** |  | 
**lastError** | **String** |  | [optional] 
**payload** | **Object** |  | [optional] 
**status** | [**WebhookEventStatus**](WebhookEventStatus.md) | accepted | delivered | failed | [optional] 



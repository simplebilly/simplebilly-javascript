# SimpleBillyApi.SubscriptionOverview

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currentPeriodEnd** | **Date** |  | [optional] 
**features** | [**PlanFeatures**](PlanFeatures.md) |  | 
**isTrialing** | **Boolean** |  | 
**limits** | [**PlanLimits**](PlanLimits.md) |  | 
**manageUrl** | **String** |  | [optional] 
**plan** | **String** | Resolved plan id (free/starter/business/enterprise, or a custom override id). | 
**planName** | **String** |  | 
**priceEur** | **Number** | Monthly price in EUR; &#x60;-1.0&#x60; &#x3D; custom pricing (enterprise). | 
**quantity** | **Number** |  | [optional] 
**status** | **String** |  | [optional] 
**subscriptionId** | **String** |  | [optional] 
**trialEndsAt** | **Date** |  | [optional] 
**usage** | [**UsageSnapshot**](UsageSnapshot.md) |  | 



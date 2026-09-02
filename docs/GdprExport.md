# SimpleBillyApi.GdprExport

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activityLog** | [**[GdprActivity]**](GdprActivity.md) |  | 
**apiKeys** | [**[GdprApiKey]**](GdprApiKey.md) | Key identifiers and names only — never a usable credential. | 
**billing** | [**[GdprBillingInfo]**](GdprBillingInfo.md) |  | 
**exportedAt** | **Date** |  | 
**generatedByAi** | **Boolean** | Honesty field: this document is a plain data dump, never AI-generated. | 
**notifications** | [**[GdprNotification]**](GdprNotification.md) |  | 
**refreshTokens** | [**[GdprRefreshToken]**](GdprRefreshToken.md) | Session records: metadata only, never the token hash. | 
**tenants** | [**[GdprTenant]**](GdprTenant.md) |  | 
**usageEvents** | [**[GdprUsageEvent]**](GdprUsageEvent.md) |  | 
**user** | [**GdprUser**](GdprUser.md) |  | 



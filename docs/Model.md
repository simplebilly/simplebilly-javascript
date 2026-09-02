# SimpleBillyApi.Model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**backupCodes** | **[String]** |  | 
**createdAt** | **Date** |  | 
**deletedAt** | **Date** |  | [optional] 
**email** | **String** |  | 
**emailVerified** | **Boolean** |  | 
**id** | **String** |  | 
**isActive** | **Boolean** |  | 
**isTotpEnabled** | **Boolean** |  | 
**lastLogin** | **Date** |  | [optional] 
**name** | **String** |  | 
**oauthId** | **String** |  | [optional] 
**oauthProvider** | **String** |  | [optional] 
**passwordChangedAt** | **Date** | Set on password change; auth/refresh tokens issued before this timestamp are rejected by the auth middleware. | [optional] 
**passwordHash** | **String** |  | 
**picture** | **String** |  | [optional] 
**privacyAcceptedAt** | **Date** | When the user accepted the data privacy policy (GDPR consent record). | [optional] 
**totpSecret** | **String** |  | [optional] 
**updatedAt** | **Date** |  | 



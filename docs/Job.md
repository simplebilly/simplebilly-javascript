# SimpleBillyApi.Job

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attempts** | **Number** |  | [optional] 
**jobType** | **String** | Discriminator the worker dispatches on (e.g. \&quot;webhook.deliver\&quot;). | 
**maxAttempts** | **Number** |  | 
**payload** | **Object** |  | [optional] 
**runAt** | **Date** | Earliest execution time; None &#x3D; run now. | [optional] 
**status** | [**JobStatus**](JobStatus.md) | pending | running | done | failed | 



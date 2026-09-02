# SimpleBillyApi.SubmitResultDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**answers** | **[Number]** | Selected answer indices (required for scored builtin trainings). | 
**assignmentId** | **String** |  | [optional] 
**score** | **Number** | Score 0–100. Only trusted for plugin trainings without server-side scoring; builtin trainings are always re-scored from &#x60;answers&#x60;. | 
**trainingCode** | **String** |  | 



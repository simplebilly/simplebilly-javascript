# SimpleBillyApi.JobPostingUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **String** |  | [optional] 
**department** | **String** |  | [optional] 
**description** | **String** | What the job is; markdown/HTML. | [optional] 
**employmentType** | [**EmploymentType**](EmploymentType.md) | full_time | part_time | contract | internship | temporary | [optional] 
**location** | **String** |  | [optional] 
**remote** | **Boolean** |  | [optional] 
**requiredSkills** | **Object** | List of required skill names (JSON array of strings). | [optional] 
**requirements** | **String** | Structured profile of the required candidate (skills, experience). | [optional] 
**salaryMax** | **Number** |  | [optional] 
**salaryMin** | **Number** |  | [optional] 
**status** | [**JobPostingStatus**](JobPostingStatus.md) | draft | published | closed | [optional] 
**title** | **String** |  | [optional] 



# SimpleBillyApi.CustomerCommunication

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**body** | **String** | The message body, call summary or note text. | [optional] 
**channel** | [**CommunicationChannel**](CommunicationChannel.md) |  | 
**contactId** | **String** | The contact (customer/supplier) this communication belongs to. References the contact entity. | 
**counterparty** | **String** | Email/phone of the counterparty, if applicable. | [optional] 
**direction** | [**CommunicationDirection**](CommunicationDirection.md) |  | 
**occurredAt** | **Date** | When the communication happened (defaults to now on create). | [optional] 
**subject** | **String** |  | [optional] 
**tags** | **Object** | Free-form tags, e.g. &#x60;[\&quot;follow-up-required\&quot;]&#x60;. | [optional] 



# SimpleBillyApi.RfqUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **String** |  | [optional] 
**lineItems** | **Object** | JSON array of &#x60;{product_id, name, sku, quantity, requested_unit_price?, quoted_unit_price?}&#x60;. | [optional] 
**notes** | **String** |  | [optional] 
**requestedDate** | **Date** |  | [optional] 
**responseDate** | **Date** |  | [optional] 
**rfqNumber** | **String** |  | [optional] 
**status** | [**RfqStatus**](RfqStatus.md) | One of: draft | sent | offer_received | rejected | converted | [optional] 
**supplierContactId** | **String** | References the supplier entity. | [optional] 
**supplierName** | **String** |  | [optional] 



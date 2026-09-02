# SimpleBillyApi.ProformaInvoiceCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**convertedAt** | **Date** |  | [optional] 
**convertedToInvoiceId** | **String** | Set when the proforma was converted into a real invoice. References the invoice entity. | [optional] 
**currency** | [**CurrencyCode**](CurrencyCode.md) |  | 
**customerId** | **String** | References the customer entity. | [optional] 
**customerSnapshot** | **Object** | Snapshot of the recipient at issue time (address, VAT id, …). | [optional] 
**issueDate** | **Date** |  | 
**lineItems** | **Object** |  | 
**notes** | **String** |  | [optional] 
**orderNumber** | **String** | Reference to the order/quote this proforma belongs to. | [optional] 
**paymentDueDate** | **Date** | Optional deadline the real invoice should carry after conversion. | [optional] 
**quotationId** | **String** | References the quotation entity. | [optional] 
**status** | [**ProformaInvoiceStatus**](ProformaInvoiceStatus.md) | &#x60;draft&#x60; | &#x60;sent&#x60; | &#x60;converted&#x60;. | 
**subtotal** | **String** |  | 
**totalAmount** | **String** |  | 
**totalTax** | **String** |  | 



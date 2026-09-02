# SimpleBillyApi.InvoiceCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attachments** | **Object** |  | [optional] 
**billingPeriodEnd** | **Date** |  | [optional] 
**billingPeriodStart** | **Date** |  | [optional] 
**cancellationDate** | **Date** |  | [optional] 
**cancellationInvoiceId** | **String** | References the invoice entity. | [optional] 
**cancellationReason** | **String** |  | [optional] 
**contractId** | **String** | References the contract entity. | [optional] 
**currency** | [**CurrencyCode**](CurrencyCode.md) |  | 
**customerId** | **String** | References the customer entity. | [optional] 
**discountAmount** | **String** |  | [optional] 
**discountDays** | **Number** |  | [optional] 
**discountPercentage** | **String** |  | [optional] 
**documentType** | [**DocumentType**](DocumentType.md) |  | [optional] 
**dunningLevel** | **Number** |  | [optional] 
**inputVatAmount** | **String** |  | [optional] 
**inputVatDeductible** | **Boolean** |  | [optional] 
**inputVatPercentage** | **String** |  | [optional] 
**introductionText** | **String** |  | [optional] 
**invoiceType** | [**InvoiceType**](InvoiceType.md) |  | 
**isCancelled** | **Boolean** |  | [optional] 
**isDraft** | **Boolean** |  | [optional] 
**isEuAcquisition** | **Boolean** |  | [optional] 
**isEuDelivery** | **Boolean** |  | [optional] 
**isIntraCommunityAcquisition** | **Boolean** |  | [optional] 
**isReverseCharge** | **Boolean** |  | [optional] 
**issueDate** | **Date** |  | 
**ledgerAccount** | **String** |  | [optional] 
**lineItems** | **Object** |  | 
**margin25a** | **Boolean** |  | [optional] 
**margin25aGross** | **String** |  | [optional] 
**margin25aPurchasePrice** | **String** |  | [optional] 
**notes** | **String** |  | [optional] 
**orderNumber** | **String** |  | [optional] 
**originalPdfPath** | **String** |  | [optional] 
**paidAmount** | **String** |  | [optional] 
**paymentDueDate** | **Date** |  | [optional] 
**paymentStatus** | [**PaymentStatus**](PaymentStatus.md) |  | [optional] 
**paymentTermsText** | **String** |  | [optional] 
**precedingSalesVoucherId** | **String** | References the preceding sales voucher entity. | [optional] 
**precedingSalesVoucherType** | [**PrecedingSalesVoucherType**](PrecedingSalesVoucherType.md) |  | [optional] 
**receiptConfirmationAvailable** | **Boolean** |  | [optional] 
**relatedInvoiceId** | **String** | References the invoice entity. | [optional] 
**relationshipType** | **String** |  | [optional] 
**senderSnapshot** | **Object** |  | [optional] 
**sentAt** | **Date** |  | [optional] 
**servicePeriodEnd** | **Date** |  | [optional] 
**servicePeriodStart** | **Date** |  | [optional] 
**status** | [**InvoiceStatus**](InvoiceStatus.md) |  | 
**subtotal** | **String** |  | 
**supplierId** | **String** | References the supplier entity. | [optional] 
**taxExemptionReason** | **String** |  | [optional] 
**totalAmount** | **String** |  | 
**totalTax** | **String** |  | 
**vatCountry** | [**CountryCode**](CountryCode.md) |  | [optional] 
**vatSpecialCase** | **String** |  | [optional] 



# SimpleBillyApi.ReturnLogisticsSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**byStatus** | **Object** | Number of return orders per status. | 
**byWarehouse** | [**[ReturnWarehouseSummary]**](ReturnWarehouseSummary.md) | Per-warehouse aggregation. | 
**itemsRestocked** | **Number** | Sum of &#x60;restock: true&#x60; line-item quantities. | 
**itemsScrapped** | **Number** | Sum of &#x60;restock: false&#x60; line-item quantities (scrapped/disposed). | 
**totalItems** | **Number** | Sum of all line-item quantities across returns. | 
**totalReturns** | **Number** | Total number of return orders (excluding soft-deleted). | 



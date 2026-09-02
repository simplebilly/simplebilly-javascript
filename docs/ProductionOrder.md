# SimpleBillyApi.ProductionOrder

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bomId** | **String** | References the BOM entity. | [optional] 
**components** | **Object** | JSON snapshot of the BOM components at creation time. | [optional] 
**endDate** | **Date** |  | [optional] 
**notes** | **String** |  | [optional] 
**orderNumber** | **String** |  | 
**productId** | **String** | The finished product to manufacture. References the product entity. | 
**quantity** | **Number** | Quantity of finished product to produce. | 
**sourceWarehouseId** | **String** | Warehouse components are consumed from. References the warehouse entity. | [optional] 
**startDate** | **Date** |  | [optional] 
**status** | [**ProductionOrderStatus**](ProductionOrderStatus.md) | One of: planned | in_production | completed | cancelled | [optional] 
**targetWarehouseId** | **String** | Warehouse the finished product is added to. References the warehouse entity. | [optional] 



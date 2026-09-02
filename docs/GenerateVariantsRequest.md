# SimpleBillyApi.GenerateVariantsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**options** | **{String: [String]}** | Option name → list of values, e.g. &#x60;{\&quot;Color\&quot;: [\&quot;Red\&quot;, \&quot;Blue\&quot;], \&quot;Size\&quot;: [\&quot;S\&quot;, \&quot;M\&quot;]}&#x60;. The cartesian product of these lists is generated. | [optional] 
**priceDelta** | **String** | Optional per-variant price delta applied to every generated variant. | [optional] 
**productId** | **String** |  | 
**skuPrefix** | **String** | Optional prefix for the generated SKUs (suffix is the option values joined by &#x60;-&#x60;). Falls back to the parent product&#39;s SKU. | [optional] 



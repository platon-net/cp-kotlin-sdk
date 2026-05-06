
# SpamDetection200ResponseData

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **classification** | [**inline**](#Classification) | Normalized classification returned by the LLM. |  |
| **confidence** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Normalized confidence from 0 to 100. |  |
| **reason** | **kotlin.String** | Short explanation in Slovak. |  |
| **signals** | **kotlin.collections.List&lt;kotlin.String&gt;** | Most important signals used for the classification. |  |
| **error** | **kotlin.Boolean** | True when the LLM call or response validation failed. |  |
| **errorMessage** | **kotlin.String** | Short technical error reason. Raw LLM response is never returned here. |  |


<a id="Classification"></a>
## Enum: classification
| Name | Value |
| ---- | ----- |
| classification | spam, ham, unknown |




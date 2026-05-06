# LLMApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**spamDetection**](LLMApi.md#spamDetection) | **POST** /llm/spam-detection | Classify a web form message as spam or ham using the local LLM |


<a id="spamDetection"></a>
# **spamDetection**
> SpamDetection200Response spamDetection(spamDetectionRequest)

Classify a web form message as spam or ham using the local LLM

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = LLMApi()
val spamDetectionRequest : SpamDetectionRequest =  // SpamDetectionRequest | Spam detection payload
try {
    val result : SpamDetection200Response = apiInstance.spamDetection(spamDetectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LLMApi#spamDetection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LLMApi#spamDetection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **spamDetectionRequest** | [**SpamDetectionRequest**](SpamDetectionRequest.md)| Spam detection payload | |

### Return type

[**SpamDetection200Response**](SpamDetection200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


# AntispamApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**addAntispamMaildata**](AntispamApi.md#addAntispamMaildata) | **POST** /antispam/maildata | Add maildata to antispam engine |
| [**checkAntispamMaildataRules**](AntispamApi.md#checkAntispamMaildataRules) | **POST** /antispam/maildata/check | Check maildata against existing antispam rules |
| [**createAntispamEmailRule**](AntispamApi.md#createAntispamEmailRule) | **POST** /antispam/rules | Create antispam email rule or increment existing rule hitcount |


<a id="addAntispamMaildata"></a>
# **addAntispamMaildata**
> CreateDnsRecord200Response addAntispamMaildata(addAntispamMaildataRequest)

Add maildata to antispam engine

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = AntispamApi()
val addAntispamMaildataRequest : AddAntispamMaildataRequest =  // AddAntispamMaildataRequest | Maildata payload
try {
    val result : CreateDnsRecord200Response = apiInstance.addAntispamMaildata(addAntispamMaildataRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AntispamApi#addAntispamMaildata")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AntispamApi#addAntispamMaildata")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **addAntispamMaildataRequest** | [**AddAntispamMaildataRequest**](AddAntispamMaildataRequest.md)| Maildata payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="checkAntispamMaildataRules"></a>
# **checkAntispamMaildataRules**
> CreateDnsRecord200Response checkAntispamMaildataRules(checkAntispamMaildataRulesRequest)

Check maildata against existing antispam rules

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = AntispamApi()
val checkAntispamMaildataRulesRequest : CheckAntispamMaildataRulesRequest =  // CheckAntispamMaildataRulesRequest | Maildata payload
try {
    val result : CreateDnsRecord200Response = apiInstance.checkAntispamMaildataRules(checkAntispamMaildataRulesRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AntispamApi#checkAntispamMaildataRules")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AntispamApi#checkAntispamMaildataRules")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **checkAntispamMaildataRulesRequest** | [**CheckAntispamMaildataRulesRequest**](CheckAntispamMaildataRulesRequest.md)| Maildata payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="createAntispamEmailRule"></a>
# **createAntispamEmailRule**
> CreateDnsRecord200Response createAntispamEmailRule(createAntispamEmailRuleRequest)

Create antispam email rule or increment existing rule hitcount

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = AntispamApi()
val createAntispamEmailRuleRequest : CreateAntispamEmailRuleRequest =  // CreateAntispamEmailRuleRequest | Antispam email rule payload
try {
    val result : CreateDnsRecord200Response = apiInstance.createAntispamEmailRule(createAntispamEmailRuleRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AntispamApi#createAntispamEmailRule")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AntispamApi#createAntispamEmailRule")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createAntispamEmailRuleRequest** | [**CreateAntispamEmailRuleRequest**](CreateAntispamEmailRuleRequest.md)| Antispam email rule payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


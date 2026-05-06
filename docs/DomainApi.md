# DomainApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**changeDomainNameservers**](DomainApi.md#changeDomainNameservers) | **PATCH** /domains/{domain}/nameservers | Change domain nameservers |
| [**closeDomain**](DomainApi.md#closeDomain) | **DELETE** /domains/{domain} | Close external customer domain product |
| [**getDomainInfo**](DomainApi.md#getDomainInfo) | **GET** /domains/{domain} | Get domain information and availability |
| [**listDomains**](DomainApi.md#listDomains) | **GET** /domains | List customer domains |
| [**registerDomain**](DomainApi.md#registerDomain) | **POST** /domains/{domain}/register | Register domain |
| [**renewDomain**](DomainApi.md#renewDomain) | **POST** /domains/{domain}/renew | Renew domain |
| [**whoisDomain**](DomainApi.md#whoisDomain) | **GET** /domains/{domain}/whois | Check domain WHOIS availability and prices |


<a id="changeDomainNameservers"></a>
# **changeDomainNameservers**
> CreateDnsRecord200Response changeDomainNameservers(domain, changeDomainNameserversRequest)

Change domain nameservers

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DomainApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val changeDomainNameserversRequest : ChangeDomainNameserversRequest =  // ChangeDomainNameserversRequest | Nameserver payload
try {
    val result : CreateDnsRecord200Response = apiInstance.changeDomainNameservers(domain, changeDomainNameserversRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#changeDomainNameservers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#changeDomainNameservers")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **changeDomainNameserversRequest** | [**ChangeDomainNameserversRequest**](ChangeDomainNameserversRequest.md)| Nameserver payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="closeDomain"></a>
# **closeDomain**
> CreateDnsRecord200Response closeDomain(domain, cname)

Close external customer domain product

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DomainApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val cname : kotlin.String = cname_example // kotlin.String | Customer name
try {
    val result : CreateDnsRecord200Response = apiInstance.closeDomain(domain, cname)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#closeDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#closeDomain")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cname** | **kotlin.String**| Customer name | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getDomainInfo"></a>
# **getDomainInfo**
> CreateDnsRecord200Response getDomainInfo(domain, cname)

Get domain information and availability

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DomainApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val cname : kotlin.String = cname_example // kotlin.String | Customer name for product context
try {
    val result : CreateDnsRecord200Response = apiInstance.getDomainInfo(domain, cname)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#getDomainInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#getDomainInfo")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cname** | **kotlin.String**| Customer name for product context | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listDomains"></a>
# **listDomains**
> ListDomains200Response listDomains(cname)

List customer domains

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DomainApi()
val cname : kotlin.String = cname_example // kotlin.String | Customer name
try {
    val result : ListDomains200Response = apiInstance.listDomains(cname)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#listDomains")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#listDomains")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cname** | **kotlin.String**| Customer name | |

### Return type

[**ListDomains200Response**](ListDomains200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="registerDomain"></a>
# **registerDomain**
> CreateDnsRecord200Response registerDomain(domain, registerDomainRequest)

Register domain

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DomainApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val registerDomainRequest : RegisterDomainRequest =  // RegisterDomainRequest | Domain registration payload
try {
    val result : CreateDnsRecord200Response = apiInstance.registerDomain(domain, registerDomainRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#registerDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#registerDomain")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **registerDomainRequest** | [**RegisterDomainRequest**](RegisterDomainRequest.md)| Domain registration payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="renewDomain"></a>
# **renewDomain**
> CreateDnsRecord200Response renewDomain(domain, renewDomainRequest)

Renew domain

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DomainApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val renewDomainRequest : RenewDomainRequest =  // RenewDomainRequest | Domain renewal payload
try {
    val result : CreateDnsRecord200Response = apiInstance.renewDomain(domain, renewDomainRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#renewDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#renewDomain")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **renewDomainRequest** | [**RenewDomainRequest**](RenewDomainRequest.md)| Domain renewal payload | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="whoisDomain"></a>
# **whoisDomain**
> WhoisDomain200Response whoisDomain(domain, cname, currencyId)

Check domain WHOIS availability and prices

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DomainApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val cname : kotlin.String = cname_example // kotlin.String | Customer name for price context
val currencyId : kotlin.String = currencyId_example // kotlin.String | Currency ID
try {
    val result : WhoisDomain200Response = apiInstance.whoisDomain(domain, cname, currencyId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainApi#whoisDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainApi#whoisDomain")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| **cname** | **kotlin.String**| Customer name for price context | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **currencyId** | **kotlin.String**| Currency ID | [optional] |

### Return type

[**WhoisDomain200Response**](WhoisDomain200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


# DNSApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createDnsRecord**](DNSApi.md#createDnsRecord) | **POST** /dns/{domain}/records | Create DNS record |
| [**deleteDnsRecord**](DNSApi.md#deleteDnsRecord) | **DELETE** /dns/{domain}/records/{recordId} | Delete DNS record |
| [**getDnsRecords**](DNSApi.md#getDnsRecords) | **GET** /dns/{domain}/records | Get DNS records by domain |
| [**updateDnsRecord**](DNSApi.md#updateDnsRecord) | **PATCH** /dns/{domain}/records/{recordId} | Update DNS record |


<a id="createDnsRecord"></a>
# **createDnsRecord**
> CreateDnsRecord200Response createDnsRecord(domain, createDnsRecordRequest)

Create DNS record

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DNSApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val createDnsRecordRequest : CreateDnsRecordRequest =  // CreateDnsRecordRequest | DNS record payload
try {
    val result : CreateDnsRecord200Response = apiInstance.createDnsRecord(domain, createDnsRecordRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DNSApi#createDnsRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DNSApi#createDnsRecord")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createDnsRecordRequest** | [**CreateDnsRecordRequest**](CreateDnsRecordRequest.md)| DNS record payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteDnsRecord"></a>
# **deleteDnsRecord**
> CreateDnsRecord200Response deleteDnsRecord(domain, recordId)

Delete DNS record

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DNSApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val recordId : kotlin.Int = 56 // kotlin.Int | Record ID
try {
    val result : CreateDnsRecord200Response = apiInstance.deleteDnsRecord(domain, recordId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DNSApi#deleteDnsRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DNSApi#deleteDnsRecord")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **recordId** | **kotlin.Int**| Record ID | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getDnsRecords"></a>
# **getDnsRecords**
> GetDnsRecords200Response getDnsRecords(domain, type)

Get DNS records by domain

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DNSApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val type : kotlin.String = type_example // kotlin.String | Filter records by type
try {
    val result : GetDnsRecords200Response = apiInstance.getDnsRecords(domain, type)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DNSApi#getDnsRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DNSApi#getDnsRecords")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **type** | **kotlin.String**| Filter records by type | [optional] |

### Return type

[**GetDnsRecords200Response**](GetDnsRecords200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateDnsRecord"></a>
# **updateDnsRecord**
> CreateDnsRecord200Response updateDnsRecord(domain, recordId, updateDnsRecordRequest)

Update DNS record

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = DNSApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val recordId : kotlin.Int = 56 // kotlin.Int | Record ID
val updateDnsRecordRequest : UpdateDnsRecordRequest =  // UpdateDnsRecordRequest | Partial DNS record payload
try {
    val result : CreateDnsRecord200Response = apiInstance.updateDnsRecord(domain, recordId, updateDnsRecordRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DNSApi#updateDnsRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DNSApi#updateDnsRecord")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| **recordId** | **kotlin.Int**| Record ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateDnsRecordRequest** | [**UpdateDnsRecordRequest**](UpdateDnsRecordRequest.md)| Partial DNS record payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


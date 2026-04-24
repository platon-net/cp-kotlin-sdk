# EmailApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**changeMailboxPassword**](EmailApi.md#changeMailboxPassword) | **PATCH** /email/{domain}/mailboxes/{username}/password | Change mailbox password |
| [**createMailbox**](EmailApi.md#createMailbox) | **POST** /email/{domain}/mailboxes | Create mailbox |


<a id="changeMailboxPassword"></a>
# **changeMailboxPassword**
> CreateDnsRecord200Response changeMailboxPassword(domain, username, changeMailboxPasswordRequest)

Change mailbox password

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = EmailApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val username : kotlin.String = username_example // kotlin.String | Mailbox username
val changeMailboxPasswordRequest : ChangeMailboxPasswordRequest =  // ChangeMailboxPasswordRequest | Mailbox password payload
try {
    val result : CreateDnsRecord200Response = apiInstance.changeMailboxPassword(domain, username, changeMailboxPasswordRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmailApi#changeMailboxPassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmailApi#changeMailboxPassword")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| **username** | **kotlin.String**| Mailbox username | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **changeMailboxPasswordRequest** | [**ChangeMailboxPasswordRequest**](ChangeMailboxPasswordRequest.md)| Mailbox password payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="createMailbox"></a>
# **createMailbox**
> CreateDnsRecord200Response createMailbox(domain, createMailboxRequest)

Create mailbox

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = EmailApi()
val domain : kotlin.String = domain_example // kotlin.String | Domain name
val createMailboxRequest : CreateMailboxRequest =  // CreateMailboxRequest | Mailbox payload
try {
    val result : CreateDnsRecord200Response = apiInstance.createMailbox(domain, createMailboxRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmailApi#createMailbox")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmailApi#createMailbox")
    e.printStackTrace()
}
```

### Parameters
| **domain** | **kotlin.String**| Domain name | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createMailboxRequest** | [**CreateMailboxRequest**](CreateMailboxRequest.md)| Mailbox payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


# OAuthApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createOauthRequest**](OAuthApi.md#createOauthRequest) | **POST** /oauth/requests | Create OAuth request |
| [**deleteOauthToken**](OAuthApi.md#deleteOauthToken) | **DELETE** /oauth/tokens | Delete OAuth token |
| [**getOauthScopes**](OAuthApi.md#getOauthScopes) | **GET** /oauth/scopes | List available OAuth scopes |
| [**refreshOauthToken**](OAuthApi.md#refreshOauthToken) | **POST** /oauth/tokens/refresh | Refresh OAuth token |
| [**verifyOauthRequest**](OAuthApi.md#verifyOauthRequest) | **GET** /oauth/requests/verify | Verify OAuth request |


<a id="createOauthRequest"></a>
# **createOauthRequest**
> CreateOauthRequest200Response createOauthRequest(createOauthRequestRequest)

Create OAuth request

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = OAuthApi()
val createOauthRequestRequest : CreateOauthRequestRequest =  // CreateOauthRequestRequest | OAuth create payload
try {
    val result : CreateOauthRequest200Response = apiInstance.createOauthRequest(createOauthRequestRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#createOauthRequest")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#createOauthRequest")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createOauthRequestRequest** | [**CreateOauthRequestRequest**](CreateOauthRequestRequest.md)| OAuth create payload | [optional] |

### Return type

[**CreateOauthRequest200Response**](CreateOauthRequest200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteOauthToken"></a>
# **deleteOauthToken**
> DeleteOauthToken200Response deleteOauthToken(token)

Delete OAuth token

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = OAuthApi()
val token : kotlin.String = token_example // kotlin.String | OAuth token
try {
    val result : DeleteOauthToken200Response = apiInstance.deleteOauthToken(token)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#deleteOauthToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#deleteOauthToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **token** | **kotlin.String**| OAuth token | |

### Return type

[**DeleteOauthToken200Response**](DeleteOauthToken200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getOauthScopes"></a>
# **getOauthScopes**
> GetOauthScopes200Response getOauthScopes()

List available OAuth scopes

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = OAuthApi()
try {
    val result : GetOauthScopes200Response = apiInstance.getOauthScopes()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#getOauthScopes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#getOauthScopes")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GetOauthScopes200Response**](GetOauthScopes200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="refreshOauthToken"></a>
# **refreshOauthToken**
> VerifyOauthRequest200Response refreshOauthToken(refreshOauthTokenRequest)

Refresh OAuth token

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = OAuthApi()
val refreshOauthTokenRequest : RefreshOauthTokenRequest =  // RefreshOauthTokenRequest | OAuth refresh payload
try {
    val result : VerifyOauthRequest200Response = apiInstance.refreshOauthToken(refreshOauthTokenRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#refreshOauthToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#refreshOauthToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **refreshOauthTokenRequest** | [**RefreshOauthTokenRequest**](RefreshOauthTokenRequest.md)| OAuth refresh payload | |

### Return type

[**VerifyOauthRequest200Response**](VerifyOauthRequest200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="verifyOauthRequest"></a>
# **verifyOauthRequest**
> VerifyOauthRequest200Response verifyOauthRequest(verifyToken)

Verify OAuth request

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = OAuthApi()
val verifyToken : kotlin.String = verifyToken_example // kotlin.String | Verify token from OAuth create response
try {
    val result : VerifyOauthRequest200Response = apiInstance.verifyOauthRequest(verifyToken)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OAuthApi#verifyOauthRequest")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OAuthApi#verifyOauthRequest")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **verifyToken** | **kotlin.String**| Verify token from OAuth create response | |

### Return type

[**VerifyOauthRequest200Response**](VerifyOauthRequest200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


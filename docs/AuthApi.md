# AuthApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createAuthToken**](AuthApi.md#createAuthToken) | **POST** /auth/token | Create anonymous auth token |


<a id="createAuthToken"></a>
# **createAuthToken**
> CreateAuthToken200Response createAuthToken()

Create anonymous auth token

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = AuthApi()
try {
    val result : CreateAuthToken200Response = apiInstance.createAuthToken()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#createAuthToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#createAuthToken")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CreateAuthToken200Response**](CreateAuthToken200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


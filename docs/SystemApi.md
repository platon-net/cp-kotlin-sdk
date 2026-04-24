# SystemApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**hello**](SystemApi.md#hello) | **GET** /system/hello | Returns greeting message |
| [**revision**](SystemApi.md#revision) | **GET** /system/revision | Returns revision number of system |
| [**time**](SystemApi.md#time) | **GET** /system/time | Returns current date and time of system |


<a id="hello"></a>
# **hello**
> Hello200Response hello()

Returns greeting message

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : Hello200Response = apiInstance.hello()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#hello")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#hello")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Hello200Response**](Hello200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="revision"></a>
# **revision**
> Revision200Response revision()

Returns revision number of system

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : Revision200Response = apiInstance.revision()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#revision")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#revision")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Revision200Response**](Revision200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="time"></a>
# **time**
> Time200Response time()

Returns current date and time of system

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : Time200Response = apiInstance.time()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#time")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#time")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Time200Response**](Time200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


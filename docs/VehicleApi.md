# VehicleApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createVehicleEvent**](VehicleApi.md#createVehicleEvent) | **POST** /vehicle/events | Create vehicle event without receipt image |
| [**deleteVehicleEvent**](VehicleApi.md#deleteVehicleEvent) | **DELETE** /vehicle/events/{eventId} | Delete vehicle event |
| [**finalizeVehicleEvent**](VehicleApi.md#finalizeVehicleEvent) | **POST** /vehicle/events/{eventId}/finalize | Finalize vehicle event draft |
| [**getVehicleEvent**](VehicleApi.md#getVehicleEvent) | **GET** /vehicle/events/{eventId} | Get vehicle event detail |
| [**getVehicleEventImage**](VehicleApi.md#getVehicleEventImage) | **GET** /vehicle/events/{eventId}/image | Get event image or thumbnail |
| [**listVehicleCurrencies**](VehicleApi.md#listVehicleCurrencies) | **GET** /vehicle/currencies | List currencies for vehicle events |
| [**listVehicleEvents**](VehicleApi.md#listVehicleEvents) | **GET** /vehicle/events | List vehicle events for the authenticated driver |
| [**listVehicleVehicles**](VehicleApi.md#listVehicleVehicles) | **GET** /vehicle/vehicles | List vehicles available to the authenticated driver |
| [**rescanVehicleEventImage**](VehicleApi.md#rescanVehicleEventImage) | **POST** /vehicle/events/{eventId}/image | Replace event image and rescan event data |
| [**setPreferredVehicle**](VehicleApi.md#setPreferredVehicle) | **PATCH** /vehicle/preferred-vehicle | Set or clear preferred vehicle |
| [**uploadVehicleReceiptImage**](VehicleApi.md#uploadVehicleReceiptImage) | **POST** /vehicle/events/receipt-image | Upload receipt image and create processing event draft |


<a id="createVehicleEvent"></a>
# **createVehicleEvent**
> CreateDnsRecord200Response createVehicleEvent(createVehicleEventRequest)

Create vehicle event without receipt image

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
val createVehicleEventRequest : CreateVehicleEventRequest =  // CreateVehicleEventRequest | Vehicle event create payload
try {
    val result : CreateDnsRecord200Response = apiInstance.createVehicleEvent(createVehicleEventRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#createVehicleEvent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#createVehicleEvent")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createVehicleEventRequest** | [**CreateVehicleEventRequest**](CreateVehicleEventRequest.md)| Vehicle event create payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteVehicleEvent"></a>
# **deleteVehicleEvent**
> CreateDnsRecord200Response deleteVehicleEvent(eventId)

Delete vehicle event

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
val eventId : kotlin.Int = 56 // kotlin.Int | Vehicle event ID
try {
    val result : CreateDnsRecord200Response = apiInstance.deleteVehicleEvent(eventId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#deleteVehicleEvent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#deleteVehicleEvent")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **eventId** | **kotlin.Int**| Vehicle event ID | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="finalizeVehicleEvent"></a>
# **finalizeVehicleEvent**
> CreateDnsRecord200Response finalizeVehicleEvent(eventId, finalizeVehicleEventRequest)

Finalize vehicle event draft

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
val eventId : kotlin.Int = 56 // kotlin.Int | Vehicle event ID
val finalizeVehicleEventRequest : FinalizeVehicleEventRequest =  // FinalizeVehicleEventRequest | Vehicle event finalize payload
try {
    val result : CreateDnsRecord200Response = apiInstance.finalizeVehicleEvent(eventId, finalizeVehicleEventRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#finalizeVehicleEvent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#finalizeVehicleEvent")
    e.printStackTrace()
}
```

### Parameters
| **eventId** | **kotlin.Int**| Vehicle event ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **finalizeVehicleEventRequest** | [**FinalizeVehicleEventRequest**](FinalizeVehicleEventRequest.md)| Vehicle event finalize payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="getVehicleEvent"></a>
# **getVehicleEvent**
> CreateDnsRecord200Response getVehicleEvent(eventId)

Get vehicle event detail

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
val eventId : kotlin.Int = 56 // kotlin.Int | Vehicle event ID
try {
    val result : CreateDnsRecord200Response = apiInstance.getVehicleEvent(eventId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#getVehicleEvent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#getVehicleEvent")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **eventId** | **kotlin.Int**| Vehicle event ID | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getVehicleEventImage"></a>
# **getVehicleEventImage**
> java.io.File getVehicleEventImage(eventId, size)

Get event image or thumbnail

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
val eventId : kotlin.Int = 56 // kotlin.Int | Vehicle event ID
val size : kotlin.String = size_example // kotlin.String | Image size variant: thumb, thumbnail or small for thumbnail response
try {
    val result : java.io.File = apiInstance.getVehicleEventImage(eventId, size)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#getVehicleEventImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#getVehicleEventImage")
    e.printStackTrace()
}
```

### Parameters
| **eventId** | **kotlin.Int**| Vehicle event ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **size** | **kotlin.String**| Image size variant: thumb, thumbnail or small for thumbnail response | [optional] |

### Return type

[**java.io.File**](java.io.File.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="listVehicleCurrencies"></a>
# **listVehicleCurrencies**
> CreateDnsRecord200Response listVehicleCurrencies()

List currencies for vehicle events

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
try {
    val result : CreateDnsRecord200Response = apiInstance.listVehicleCurrencies()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#listVehicleCurrencies")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#listVehicleCurrencies")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listVehicleEvents"></a>
# **listVehicleEvents**
> CreateDnsRecord200Response listVehicleEvents(since)

List vehicle events for the authenticated driver

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
val since : kotlin.String = since_example // kotlin.String | Return events with event datetime greater than or equal to the provided local datetime
try {
    val result : CreateDnsRecord200Response = apiInstance.listVehicleEvents(since)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#listVehicleEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#listVehicleEvents")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **since** | **kotlin.String**| Return events with event datetime greater than or equal to the provided local datetime | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listVehicleVehicles"></a>
# **listVehicleVehicles**
> CreateDnsRecord200Response listVehicleVehicles()

List vehicles available to the authenticated driver

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
try {
    val result : CreateDnsRecord200Response = apiInstance.listVehicleVehicles()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#listVehicleVehicles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#listVehicleVehicles")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="rescanVehicleEventImage"></a>
# **rescanVehicleEventImage**
> CreateDnsRecord200Response rescanVehicleEventImage(eventId, image, timezone, eventType)

Replace event image and rescan event data

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
val eventId : kotlin.Int = 56 // kotlin.Int | Vehicle event ID
val image : java.io.File = BINARY_DATA_HERE // java.io.File | 
val timezone : kotlin.String = timezone_example // kotlin.String | 
val eventType : kotlin.String = eventType_example // kotlin.String | 
try {
    val result : CreateDnsRecord200Response = apiInstance.rescanVehicleEventImage(eventId, image, timezone, eventType)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#rescanVehicleEventImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#rescanVehicleEventImage")
    e.printStackTrace()
}
```

### Parameters
| **eventId** | **kotlin.Int**| Vehicle event ID | |
| **image** | **java.io.File**|  | |
| **timezone** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **eventType** | **kotlin.String**|  | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

<a id="setPreferredVehicle"></a>
# **setPreferredVehicle**
> CreateDnsRecord200Response setPreferredVehicle(setPreferredVehicleRequest)

Set or clear preferred vehicle

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
val setPreferredVehicleRequest : SetPreferredVehicleRequest =  // SetPreferredVehicleRequest | Preferred vehicle payload
try {
    val result : CreateDnsRecord200Response = apiInstance.setPreferredVehicle(setPreferredVehicleRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#setPreferredVehicle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#setPreferredVehicle")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **setPreferredVehicleRequest** | [**SetPreferredVehicleRequest**](SetPreferredVehicleRequest.md)| Preferred vehicle payload | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="uploadVehicleReceiptImage"></a>
# **uploadVehicleReceiptImage**
> CreateDnsRecord200Response uploadVehicleReceiptImage(image, timezone, eventType)

Upload receipt image and create processing event draft

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = VehicleApi()
val image : java.io.File = BINARY_DATA_HERE // java.io.File | 
val timezone : kotlin.String = timezone_example // kotlin.String | 
val eventType : kotlin.String = eventType_example // kotlin.String | 
try {
    val result : CreateDnsRecord200Response = apiInstance.uploadVehicleReceiptImage(image, timezone, eventType)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VehicleApi#uploadVehicleReceiptImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VehicleApi#uploadVehicleReceiptImage")
    e.printStackTrace()
}
```

### Parameters
| **image** | **java.io.File**|  | |
| **timezone** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **eventType** | **kotlin.String**|  | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


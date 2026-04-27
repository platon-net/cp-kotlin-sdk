# CartApi

All URIs are relative to *https://setup.platon.sk/api*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**checkCartCoupon**](CartApi.md#checkCartCoupon) | **POST** /cart/coupons/check | Check and apply cart coupon |
| [**createCartItem**](CartApi.md#createCartItem) | **POST** /cart/items | Add item to cart |
| [**deleteCartItem**](CartApi.md#deleteCartItem) | **DELETE** /cart/items/{cartItemId} | Remove item from cart |
| [**getCartBillingAddress**](CartApi.md#getCartBillingAddress) | **GET** /cart/billing-address | Get cart billing address |
| [**getCartCoupon**](CartApi.md#getCartCoupon) | **GET** /cart/coupons/current | Get current cart coupon |
| [**getCartTotal**](CartApi.md#getCartTotal) | **GET** /cart/total | Get cart total |
| [**listCartItems**](CartApi.md#listCartItems) | **GET** /cart/items | List cart items |
| [**updateCartItem**](CartApi.md#updateCartItem) | **PATCH** /cart/items/{cartItemId} | Update cart item data |
| [**updateCartItemCount**](CartApi.md#updateCartItemCount) | **PATCH** /cart/items/by-product/count | Update cart item count by product and domain |


<a id="checkCartCoupon"></a>
# **checkCartCoupon**
> CreateDnsRecord200Response checkCartCoupon(checkCartCouponRequest)

Check and apply cart coupon

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = CartApi()
val checkCartCouponRequest : CheckCartCouponRequest =  // CheckCartCouponRequest | Cart coupon check payload
try {
    val result : CreateDnsRecord200Response = apiInstance.checkCartCoupon(checkCartCouponRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#checkCartCoupon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#checkCartCoupon")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **checkCartCouponRequest** | [**CheckCartCouponRequest**](CheckCartCouponRequest.md)| Cart coupon check payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="createCartItem"></a>
# **createCartItem**
> CreateDnsRecord200Response createCartItem(createCartItemRequest)

Add item to cart

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = CartApi()
val createCartItemRequest : CreateCartItemRequest =  // CreateCartItemRequest | Cart item add payload
try {
    val result : CreateDnsRecord200Response = apiInstance.createCartItem(createCartItemRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#createCartItem")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#createCartItem")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createCartItemRequest** | [**CreateCartItemRequest**](CreateCartItemRequest.md)| Cart item add payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteCartItem"></a>
# **deleteCartItem**
> CreateDnsRecord200Response deleteCartItem(cartItemId, cname)

Remove item from cart

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = CartApi()
val cartItemId : kotlin.Int = 56 // kotlin.Int | Cart item ID
val cname : kotlin.String = cname_example // kotlin.String | Customer name
try {
    val result : CreateDnsRecord200Response = apiInstance.deleteCartItem(cartItemId, cname)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#deleteCartItem")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#deleteCartItem")
    e.printStackTrace()
}
```

### Parameters
| **cartItemId** | **kotlin.Int**| Cart item ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cname** | **kotlin.String**| Customer name | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getCartBillingAddress"></a>
# **getCartBillingAddress**
> CreateDnsRecord200Response getCartBillingAddress(cname)

Get cart billing address

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = CartApi()
val cname : kotlin.String = cname_example // kotlin.String | Customer name
try {
    val result : CreateDnsRecord200Response = apiInstance.getCartBillingAddress(cname)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#getCartBillingAddress")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#getCartBillingAddress")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cname** | **kotlin.String**| Customer name | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getCartCoupon"></a>
# **getCartCoupon**
> CreateDnsRecord200Response getCartCoupon(cname)

Get current cart coupon

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = CartApi()
val cname : kotlin.String = cname_example // kotlin.String | Customer name
try {
    val result : CreateDnsRecord200Response = apiInstance.getCartCoupon(cname)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#getCartCoupon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#getCartCoupon")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cname** | **kotlin.String**| Customer name | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getCartTotal"></a>
# **getCartTotal**
> CreateDnsRecord200Response getCartTotal(cname)

Get cart total

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = CartApi()
val cname : kotlin.String = cname_example // kotlin.String | Customer name
try {
    val result : CreateDnsRecord200Response = apiInstance.getCartTotal(cname)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#getCartTotal")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#getCartTotal")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cname** | **kotlin.String**| Customer name | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listCartItems"></a>
# **listCartItems**
> CreateDnsRecord200Response listCartItems(cname, lang)

List cart items

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = CartApi()
val cname : kotlin.String = cname_example // kotlin.String | Customer name
val lang : kotlin.String = lang_example // kotlin.String | Response language
try {
    val result : CreateDnsRecord200Response = apiInstance.listCartItems(cname, lang)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#listCartItems")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#listCartItems")
    e.printStackTrace()
}
```

### Parameters
| **cname** | **kotlin.String**| Customer name | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **lang** | **kotlin.String**| Response language | [optional] |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateCartItem"></a>
# **updateCartItem**
> CreateDnsRecord200Response updateCartItem(cartItemId, updateCartItemRequest)

Update cart item data

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = CartApi()
val cartItemId : kotlin.Int = 56 // kotlin.Int | Cart item ID
val updateCartItemRequest : UpdateCartItemRequest =  // UpdateCartItemRequest | Cart item update payload
try {
    val result : CreateDnsRecord200Response = apiInstance.updateCartItem(cartItemId, updateCartItemRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#updateCartItem")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#updateCartItem")
    e.printStackTrace()
}
```

### Parameters
| **cartItemId** | **kotlin.Int**| Cart item ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateCartItemRequest** | [**UpdateCartItemRequest**](UpdateCartItemRequest.md)| Cart item update payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="updateCartItemCount"></a>
# **updateCartItemCount**
> CreateDnsRecord200Response updateCartItemCount(updateCartItemCountRequest)

Update cart item count by product and domain

### Example
```kotlin
// Import classes:
//import sk.platon.controlpanel.sdk.infrastructure.*
//import sk.platon.controlpanel.sdk.models.*

val apiInstance = CartApi()
val updateCartItemCountRequest : UpdateCartItemCountRequest =  // UpdateCartItemCountRequest | Cart item count update payload
try {
    val result : CreateDnsRecord200Response = apiInstance.updateCartItemCount(updateCartItemCountRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#updateCartItemCount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#updateCartItemCount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateCartItemCountRequest** | [**UpdateCartItemCountRequest**](UpdateCartItemCountRequest.md)| Cart item count update payload | |

### Return type

[**CreateDnsRecord200Response**](CreateDnsRecord200Response.md)

### Authorization


Configure bearerAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


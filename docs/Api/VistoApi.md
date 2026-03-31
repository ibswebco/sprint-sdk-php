# OpenAPI\Client\VistoApi



All URIs are relative to https://api.sprintco.it/v2, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**v2vistiDestroy()**](VistoApi.md#v2vistiDestroy) | **DELETE** /visti/{visto} | Remove the specified resource from storage |
| [**v2vistiIndex()**](VistoApi.md#v2vistiIndex) | **GET** /visti | Display a listing of the resource |
| [**v2vistiShow()**](VistoApi.md#v2vistiShow) | **GET** /visti/{visto} | Display the specified resource |
| [**v2vistiStore()**](VistoApi.md#v2vistiStore) | **POST** /visti | Store a newly created resource in storage |
| [**v2vistiUpdate()**](VistoApi.md#v2vistiUpdate) | **PUT** /visti/{visto} | Update the specified resource in storage |


## `v2vistiDestroy()`

```php
v2vistiDestroy($visto)
```

Remove the specified resource from storage

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$visto = 'visto_example'; // string | The visto cod

try {
    $apiInstance->v2vistiDestroy($visto);
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiDestroy: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **visto** | **string**| The visto cod | |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `v2vistiIndex()`

```php
v2vistiIndex(): object
```

Display a listing of the resource

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->v2vistiIndex();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiIndex: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[http](../../README.md#http)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `v2vistiShow()`

```php
v2vistiShow($visto): object
```

Display the specified resource

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$visto = 'visto_example'; // string | The visto cod

try {
    $result = $apiInstance->v2vistiShow($visto);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiShow: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **visto** | **string**| The visto cod | |

### Return type

**object**

### Authorization

[http](../../README.md#http)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `v2vistiStore()`

```php
v2vistiStore($v2visti_store_request): object
```

Store a newly created resource in storage

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$v2visti_store_request = new \OpenAPI\Client\Model\V2vistiStoreRequest(); // \OpenAPI\Client\Model\V2vistiStoreRequest

try {
    $result = $apiInstance->v2vistiStore($v2visti_store_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiStore: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **v2visti_store_request** | [**\OpenAPI\Client\Model\V2vistiStoreRequest**](../Model/V2vistiStoreRequest.md)|  | |

### Return type

**object**

### Authorization

[http](../../README.md#http)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `v2vistiUpdate()`

```php
v2vistiUpdate($visto, $v2visti_update_request): object
```

Update the specified resource in storage

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$visto = 'visto_example'; // string | The visto cod
$v2visti_update_request = new \OpenAPI\Client\Model\V2vistiUpdateRequest(); // \OpenAPI\Client\Model\V2vistiUpdateRequest

try {
    $result = $apiInstance->v2vistiUpdate($visto, $v2visti_update_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiUpdate: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **visto** | **string**| The visto cod | |
| **v2visti_update_request** | [**\OpenAPI\Client\Model\V2vistiUpdateRequest**](../Model/V2vistiUpdateRequest.md)|  | |

### Return type

**object**

### Authorization

[http](../../README.md#http)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

# OpenAPI\Client\ModelloApi



All URIs are relative to https://api.sprintco.it/v2, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**v2modelliDestroy()**](ModelloApi.md#v2modelliDestroy) | **DELETE** /modelli/{modello} | Remove the specified resource from storage |
| [**v2modelliIndex()**](ModelloApi.md#v2modelliIndex) | **GET** /modelli | Display a listing of the resource |
| [**v2modelliShow()**](ModelloApi.md#v2modelliShow) | **GET** /modelli/{modello} | Display the specified resource |
| [**v2modelliStore()**](ModelloApi.md#v2modelliStore) | **POST** /modelli | Store a newly created resource in storage |
| [**v2modelliUpdate()**](ModelloApi.md#v2modelliUpdate) | **PUT** /modelli/{modello} | Update the specified resource in storage |


## `v2modelliDestroy()`

```php
v2modelliDestroy($modello)
```

Remove the specified resource from storage

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$modello = 56; // int | The modello idm1

try {
    $apiInstance->v2modelliDestroy($modello);
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliDestroy: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **modello** | **int**| The modello idm1 | |

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

## `v2modelliIndex()`

```php
v2modelliIndex(): object
```

Display a listing of the resource

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->v2modelliIndex();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliIndex: ', $e->getMessage(), PHP_EOL;
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

## `v2modelliShow()`

```php
v2modelliShow($modello): object
```

Display the specified resource

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$modello = 56; // int | The modello idm1

try {
    $result = $apiInstance->v2modelliShow($modello);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliShow: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **modello** | **int**| The modello idm1 | |

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

## `v2modelliStore()`

```php
v2modelliStore($v2modelli_store_request): object
```

Store a newly created resource in storage

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$v2modelli_store_request = new \OpenAPI\Client\Model\V2modelliStoreRequest(); // \OpenAPI\Client\Model\V2modelliStoreRequest

try {
    $result = $apiInstance->v2modelliStore($v2modelli_store_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliStore: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **v2modelli_store_request** | [**\OpenAPI\Client\Model\V2modelliStoreRequest**](../Model/V2modelliStoreRequest.md)|  | |

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

## `v2modelliUpdate()`

```php
v2modelliUpdate($modello, $v2modelli_update_request): object
```

Update the specified resource in storage

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$modello = 56; // int | The modello idm1
$v2modelli_update_request = new \OpenAPI\Client\Model\V2modelliUpdateRequest(); // \OpenAPI\Client\Model\V2modelliUpdateRequest

try {
    $result = $apiInstance->v2modelliUpdate($modello, $v2modelli_update_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliUpdate: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **modello** | **int**| The modello idm1 | |
| **v2modelli_update_request** | [**\OpenAPI\Client\Model\V2modelliUpdateRequest**](../Model/V2modelliUpdateRequest.md)|  | |

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

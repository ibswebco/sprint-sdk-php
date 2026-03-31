# OpenAPI\Client\RichiestaApi



All URIs are relative to https://api.sprintco.it/v2, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**v2richiesteDestroy()**](RichiestaApi.md#v2richiesteDestroy) | **DELETE** /richieste/{richiesta} | Remove the specified resource from storage |
| [**v2richiesteIndex()**](RichiestaApi.md#v2richiesteIndex) | **GET** /richieste | Display a listing of the resource |
| [**v2richiesteShow()**](RichiestaApi.md#v2richiesteShow) | **GET** /richieste/{richiesta} | Display the specified resource |
| [**v2richiesteStore()**](RichiestaApi.md#v2richiesteStore) | **POST** /richieste | Store a newly created resource in storage |
| [**v2richiesteUpdate()**](RichiestaApi.md#v2richiesteUpdate) | **PUT** /richieste/{richiesta} | Update the specified resource in storage |


## `v2richiesteDestroy()`

```php
v2richiesteDestroy($richiesta): object
```

Remove the specified resource from storage

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$richiesta = 'richiesta_example'; // string | The richiesta r1 codric

try {
    $result = $apiInstance->v2richiesteDestroy($richiesta);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteDestroy: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **richiesta** | **string**| The richiesta r1 codric | |

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

## `v2richiesteIndex()`

```php
v2richiesteIndex(): object
```

Display a listing of the resource

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->v2richiesteIndex();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteIndex: ', $e->getMessage(), PHP_EOL;
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

## `v2richiesteShow()`

```php
v2richiesteShow($richiesta): object
```

Display the specified resource

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$richiesta = 'richiesta_example'; // string | The richiesta r1 codric

try {
    $result = $apiInstance->v2richiesteShow($richiesta);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteShow: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **richiesta** | **string**| The richiesta r1 codric | |

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

## `v2richiesteStore()`

```php
v2richiesteStore($v2richieste_store_request): object
```

Store a newly created resource in storage

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$v2richieste_store_request = new \OpenAPI\Client\Model\V2richiesteStoreRequest(); // \OpenAPI\Client\Model\V2richiesteStoreRequest

try {
    $result = $apiInstance->v2richiesteStore($v2richieste_store_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteStore: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **v2richieste_store_request** | [**\OpenAPI\Client\Model\V2richiesteStoreRequest**](../Model/V2richiesteStoreRequest.md)|  | |

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

## `v2richiesteUpdate()`

```php
v2richiesteUpdate($richiesta, $v2richieste_update_request): object
```

Update the specified resource in storage

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: http
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$richiesta = 'richiesta_example'; // string | The richiesta r1 codric
$v2richieste_update_request = new \OpenAPI\Client\Model\V2richiesteUpdateRequest(); // \OpenAPI\Client\Model\V2richiesteUpdateRequest

try {
    $result = $apiInstance->v2richiesteUpdate($richiesta, $v2richieste_update_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteUpdate: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **richiesta** | **string**| The richiesta r1 codric | |
| **v2richieste_update_request** | [**\OpenAPI\Client\Model\V2richiesteUpdateRequest**](../Model/V2richiesteUpdateRequest.md)|  | |

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

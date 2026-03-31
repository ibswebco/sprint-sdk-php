# Swagger\Client\ModelloApi

All URIs are relative to *https://api.sprintco.it/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**v2modelliDestroy**](ModelloApi.md#v2modellidestroy) | **DELETE** /modelli/{modello} | Remove the specified resource from storage
[**v2modelliIndex**](ModelloApi.md#v2modelliindex) | **GET** /modelli | Display a listing of the resource
[**v2modelliShow**](ModelloApi.md#v2modellishow) | **GET** /modelli/{modello} | Display the specified resource
[**v2modelliStore**](ModelloApi.md#v2modellistore) | **POST** /modelli | Store a newly created resource in storage
[**v2modelliUpdate**](ModelloApi.md#v2modelliupdate) | **PUT** /modelli/{modello} | Update the specified resource in storage

# **v2modelliDestroy**
> v2modelliDestroy($modello)

Remove the specified resource from storage

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$modello = new \Swagger\Client\Model\null(); //  | The modello idm1

try {
    $apiInstance->v2modelliDestroy($modello);
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliDestroy: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **modello** | [****](../Model/.md)| The modello idm1 |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2modelliIndex**
> v2modelliIndex()

Display a listing of the resource

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $apiInstance->v2modelliIndex();
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliIndex: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2modelliShow**
> v2modelliShow($modello)

Display the specified resource

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$modello = new \Swagger\Client\Model\null(); //  | The modello idm1

try {
    $apiInstance->v2modelliShow($modello);
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliShow: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **modello** | [****](../Model/.md)| The modello idm1 |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2modelliStore**
> v2modelliStore($body)

Store a newly created resource in storage

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ModelliBody(); // \Swagger\Client\Model\ModelliBody | 

try {
    $apiInstance->v2modelliStore($body);
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliStore: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ModelliBody**](../Model/ModelliBody.md)|  |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2modelliUpdate**
> v2modelliUpdate($body, $modello)

Update the specified resource in storage

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\ModelloApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ModelliModelloBody(); // \Swagger\Client\Model\ModelliModelloBody | 
$modello = new \Swagger\Client\Model\null(); //  | The modello idm1

try {
    $apiInstance->v2modelliUpdate($body, $modello);
} catch (Exception $e) {
    echo 'Exception when calling ModelloApi->v2modelliUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ModelliModelloBody**](../Model/ModelliModelloBody.md)|  |
 **modello** | [****](../Model/.md)| The modello idm1 |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


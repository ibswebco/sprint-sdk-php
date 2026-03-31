# Swagger\Client\VistoApi

All URIs are relative to *https://api.sprintco.it/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**v2vistiDestroy**](VistoApi.md#v2vistidestroy) | **DELETE** /visti/{visto} | Remove the specified resource from storage
[**v2vistiIndex**](VistoApi.md#v2vistiindex) | **GET** /visti | Display a listing of the resource
[**v2vistiShow**](VistoApi.md#v2vistishow) | **GET** /visti/{visto} | Display the specified resource
[**v2vistiStore**](VistoApi.md#v2vististore) | **POST** /visti | Store a newly created resource in storage
[**v2vistiUpdate**](VistoApi.md#v2vistiupdate) | **PUT** /visti/{visto} | Update the specified resource in storage

# **v2vistiDestroy**
> v2vistiDestroy($visto)

Remove the specified resource from storage

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$visto = new \Swagger\Client\Model\null(); //  | The visto cod

try {
    $apiInstance->v2vistiDestroy($visto);
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiDestroy: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **visto** | [****](../Model/.md)| The visto cod |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2vistiIndex**
> v2vistiIndex()

Display a listing of the resource

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $apiInstance->v2vistiIndex();
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiIndex: ', $e->getMessage(), PHP_EOL;
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

# **v2vistiShow**
> v2vistiShow($visto)

Display the specified resource

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$visto = new \Swagger\Client\Model\null(); //  | The visto cod

try {
    $apiInstance->v2vistiShow($visto);
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiShow: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **visto** | [****](../Model/.md)| The visto cod |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2vistiStore**
> v2vistiStore($body)

Store a newly created resource in storage

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\VistiBody(); // \Swagger\Client\Model\VistiBody | 

try {
    $apiInstance->v2vistiStore($body);
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiStore: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\VistiBody**](../Model/VistiBody.md)|  |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2vistiUpdate**
> v2vistiUpdate($body, $visto)

Update the specified resource in storage

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\VistoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\VistiVistoBody(); // \Swagger\Client\Model\VistiVistoBody | 
$visto = new \Swagger\Client\Model\null(); //  | The visto cod

try {
    $apiInstance->v2vistiUpdate($body, $visto);
} catch (Exception $e) {
    echo 'Exception when calling VistoApi->v2vistiUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\VistiVistoBody**](../Model/VistiVistoBody.md)|  |
 **visto** | [****](../Model/.md)| The visto cod |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


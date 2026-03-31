# Swagger\Client\RichiestaApi

All URIs are relative to *https://api.sprintco.it/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**v2richiesteDestroy**](RichiestaApi.md#v2richiestedestroy) | **DELETE** /richieste/{richiesta} | Remove the specified resource from storage
[**v2richiesteIndex**](RichiestaApi.md#v2richiesteindex) | **GET** /richieste | Display a listing of the resource
[**v2richiesteShow**](RichiestaApi.md#v2richiesteshow) | **GET** /richieste/{richiesta} | Display the specified resource
[**v2richiesteStore**](RichiestaApi.md#v2richiestestore) | **POST** /richieste | Store a newly created resource in storage
[**v2richiesteUpdate**](RichiestaApi.md#v2richiesteupdate) | **PUT** /richieste/{richiesta} | Update the specified resource in storage

# **v2richiesteDestroy**
> v2richiesteDestroy($richiesta)

Remove the specified resource from storage

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$richiesta = new \Swagger\Client\Model\null(); //  | The richiesta r1 codric

try {
    $apiInstance->v2richiesteDestroy($richiesta);
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteDestroy: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **richiesta** | [****](../Model/.md)| The richiesta r1 codric |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2richiesteIndex**
> v2richiesteIndex()

Display a listing of the resource

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $apiInstance->v2richiesteIndex();
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteIndex: ', $e->getMessage(), PHP_EOL;
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

# **v2richiesteShow**
> v2richiesteShow($richiesta)

Display the specified resource

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$richiesta = new \Swagger\Client\Model\null(); //  | The richiesta r1 codric

try {
    $apiInstance->v2richiesteShow($richiesta);
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteShow: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **richiesta** | [****](../Model/.md)| The richiesta r1 codric |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2richiesteStore**
> v2richiesteStore($body)

Store a newly created resource in storage

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\RichiesteBody(); // \Swagger\Client\Model\RichiesteBody | 

try {
    $apiInstance->v2richiesteStore($body);
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteStore: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\RichiesteBody**](../Model/RichiesteBody.md)|  |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **v2richiesteUpdate**
> v2richiesteUpdate($body, $richiesta)

Update the specified resource in storage

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: http
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\Api\RichiestaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\RichiesteRichiestaBody(); // \Swagger\Client\Model\RichiesteRichiestaBody | 
$richiesta = new \Swagger\Client\Model\null(); //  | The richiesta r1 codric

try {
    $apiInstance->v2richiesteUpdate($body, $richiesta);
} catch (Exception $e) {
    echo 'Exception when calling RichiestaApi->v2richiesteUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\RichiesteRichiestaBody**](../Model/RichiesteRichiestaBody.md)|  |
 **richiesta** | [****](../Model/.md)| The richiesta r1 codric |

### Return type

void (empty response body)

### Authorization

[http](../../README.md#http)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


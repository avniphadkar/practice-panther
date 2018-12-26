# Swagger\Client\TimeEntriesApi

All URIs are relative to *https://app.practicepanther.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**timeEntriesDelete**](TimeEntriesApi.md#timeEntriesDelete) | **DELETE** /api/v2/timeentries | 
[**timeEntriesGetTimeEntry**](TimeEntriesApi.md#timeEntriesGetTimeEntry) | **GET** /api/v2/timeentries/{id} | 
[**timeEntriesGetTimeEntrys**](TimeEntriesApi.md#timeEntriesGetTimeEntrys) | **GET** /api/v2/timeentries | 
[**timeEntriesPostAccount**](TimeEntriesApi.md#timeEntriesPostAccount) | **POST** /api/v2/timeentries | 
[**timeEntriesPutAccount**](TimeEntriesApi.md#timeEntriesPutAccount) | **PUT** /api/v2/timeentries | 


# **timeEntriesDelete**
> \Swagger\Client\Model\TimeEntry timeEntriesDelete($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TimeEntriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->timeEntriesDelete($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TimeEntriesApi->timeEntriesDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\TimeEntry**](../Model/TimeEntry.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **timeEntriesGetTimeEntry**
> \Swagger\Client\Model\TimeEntry timeEntriesGetTimeEntry($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TimeEntriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->timeEntriesGetTimeEntry($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TimeEntriesApi->timeEntriesGetTimeEntry: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\TimeEntry**](../Model/TimeEntry.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **timeEntriesGetTimeEntrys**
> \Swagger\Client\Model\TimeEntry timeEntriesGetTimeEntrys($account_id, $matter_id, $user_id, $item_id, $created_since, $updated_since, $date_from, $date_to)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TimeEntriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$account_id = "account_id_example"; // string | 
$matter_id = "matter_id_example"; // string | 
$user_id = "user_id_example"; // string | 
$item_id = "item_id_example"; // string | 
$created_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$updated_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$date_from = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$date_to = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 

try {
    $result = $apiInstance->timeEntriesGetTimeEntrys($account_id, $matter_id, $user_id, $item_id, $created_since, $updated_since, $date_from, $date_to);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TimeEntriesApi->timeEntriesGetTimeEntrys: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **string**|  | [optional]
 **matter_id** | **string**|  | [optional]
 **user_id** | **string**|  | [optional]
 **item_id** | **string**|  | [optional]
 **created_since** | **\DateTime**|  | [optional]
 **updated_since** | **\DateTime**|  | [optional]
 **date_from** | **\DateTime**|  | [optional]
 **date_to** | **\DateTime**|  | [optional]

### Return type

[**\Swagger\Client\Model\TimeEntry**](../Model/TimeEntry.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **timeEntriesPostAccount**
> \Swagger\Client\Model\TimeEntry timeEntriesPostAccount($value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TimeEntriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\TimeEntry(); // \Swagger\Client\Model\TimeEntry | 

try {
    $result = $apiInstance->timeEntriesPostAccount($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TimeEntriesApi->timeEntriesPostAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\TimeEntry**](../Model/TimeEntry.md)|  |

### Return type

[**\Swagger\Client\Model\TimeEntry**](../Model/TimeEntry.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **timeEntriesPutAccount**
> \Swagger\Client\Model\TimeEntry timeEntriesPutAccount($id, $value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TimeEntriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 
$value = new \Swagger\Client\Model\TimeEntry(); // \Swagger\Client\Model\TimeEntry | 

try {
    $result = $apiInstance->timeEntriesPutAccount($id, $value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TimeEntriesApi->timeEntriesPutAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **value** | [**\Swagger\Client\Model\TimeEntry**](../Model/TimeEntry.md)|  |

### Return type

[**\Swagger\Client\Model\TimeEntry**](../Model/TimeEntry.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


# Swagger\Client\EventsApi

All URIs are relative to *https://app.practicepanther.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**eventsDelete**](EventsApi.md#eventsDelete) | **DELETE** /api/v2/events | 
[**eventsGetEvent**](EventsApi.md#eventsGetEvent) | **GET** /api/v2/events/{id} | 
[**eventsGetEvents**](EventsApi.md#eventsGetEvents) | **GET** /api/v2/events | 
[**eventsPostAccount**](EventsApi.md#eventsPostAccount) | **POST** /api/v2/events | 
[**eventsPutAccount**](EventsApi.md#eventsPutAccount) | **PUT** /api/v2/events | 


# **eventsDelete**
> \Swagger\Client\Model\Event eventsDelete($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EventsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->eventsDelete($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventsApi->eventsDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Event**](../Model/Event.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **eventsGetEvent**
> \Swagger\Client\Model\Event eventsGetEvent($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EventsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->eventsGetEvent($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventsApi->eventsGetEvent: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Event**](../Model/Event.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **eventsGetEvents**
> \Swagger\Client\Model\Event eventsGetEvents($assigned_to_user_id, $account_id, $matter_id, $created_since, $updated_since, $date_from, $date_to, $activity_tag)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EventsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$assigned_to_user_id = "assigned_to_user_id_example"; // string | 
$account_id = "account_id_example"; // string | 
$matter_id = "matter_id_example"; // string | 
$created_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$updated_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$date_from = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$date_to = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$activity_tag = "activity_tag_example"; // string | 

try {
    $result = $apiInstance->eventsGetEvents($assigned_to_user_id, $account_id, $matter_id, $created_since, $updated_since, $date_from, $date_to, $activity_tag);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventsApi->eventsGetEvents: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assigned_to_user_id** | **string**|  | [optional]
 **account_id** | **string**|  | [optional]
 **matter_id** | **string**|  | [optional]
 **created_since** | **\DateTime**|  | [optional]
 **updated_since** | **\DateTime**|  | [optional]
 **date_from** | **\DateTime**|  | [optional]
 **date_to** | **\DateTime**|  | [optional]
 **activity_tag** | **string**|  | [optional]

### Return type

[**\Swagger\Client\Model\Event**](../Model/Event.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **eventsPostAccount**
> \Swagger\Client\Model\Event eventsPostAccount($value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EventsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\Event(); // \Swagger\Client\Model\Event | 

try {
    $result = $apiInstance->eventsPostAccount($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventsApi->eventsPostAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\Event**](../Model/Event.md)|  |

### Return type

[**\Swagger\Client\Model\Event**](../Model/Event.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **eventsPutAccount**
> \Swagger\Client\Model\Event eventsPutAccount($id, $value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EventsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 
$value = new \Swagger\Client\Model\Event(); // \Swagger\Client\Model\Event | 

try {
    $result = $apiInstance->eventsPutAccount($id, $value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventsApi->eventsPutAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **value** | [**\Swagger\Client\Model\Event**](../Model/Event.md)|  |

### Return type

[**\Swagger\Client\Model\Event**](../Model/Event.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


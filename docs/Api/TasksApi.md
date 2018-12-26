# Swagger\Client\TasksApi

All URIs are relative to *https://app.practicepanther.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**tasksDelete**](TasksApi.md#tasksDelete) | **DELETE** /api/v2/tasks | 
[**tasksGetTask**](TasksApi.md#tasksGetTask) | **GET** /api/v2/tasks/{id} | 
[**tasksGetTasks**](TasksApi.md#tasksGetTasks) | **GET** /api/v2/tasks | 
[**tasksPostAccount**](TasksApi.md#tasksPostAccount) | **POST** /api/v2/tasks | 
[**tasksPutAccount**](TasksApi.md#tasksPutAccount) | **PUT** /api/v2/tasks | 


# **tasksDelete**
> \Swagger\Client\Model\Task tasksDelete($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TasksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->tasksDelete($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TasksApi->tasksDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Task**](../Model/Task.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **tasksGetTask**
> \Swagger\Client\Model\Task tasksGetTask($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TasksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->tasksGetTask($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TasksApi->tasksGetTask: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Task**](../Model/Task.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **tasksGetTasks**
> \Swagger\Client\Model\Task tasksGetTasks($assigned_to_user_id, $account_id, $matter_id, $created_since, $updated_since, $status, $due_date_from, $due_date_to, $activity_tag)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TasksApi(
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
$status = "status_example"; // string | 
$due_date_from = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$due_date_to = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$activity_tag = "activity_tag_example"; // string | 

try {
    $result = $apiInstance->tasksGetTasks($assigned_to_user_id, $account_id, $matter_id, $created_since, $updated_since, $status, $due_date_from, $due_date_to, $activity_tag);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TasksApi->tasksGetTasks: ', $e->getMessage(), PHP_EOL;
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
 **status** | **string**|  | [optional]
 **due_date_from** | **\DateTime**|  | [optional]
 **due_date_to** | **\DateTime**|  | [optional]
 **activity_tag** | **string**|  | [optional]

### Return type

[**\Swagger\Client\Model\Task**](../Model/Task.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **tasksPostAccount**
> \Swagger\Client\Model\Task tasksPostAccount($value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TasksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\Task(); // \Swagger\Client\Model\Task | 

try {
    $result = $apiInstance->tasksPostAccount($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TasksApi->tasksPostAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\Task**](../Model/Task.md)|  |

### Return type

[**\Swagger\Client\Model\Task**](../Model/Task.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **tasksPutAccount**
> \Swagger\Client\Model\Task tasksPutAccount($id, $value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TasksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 
$value = new \Swagger\Client\Model\Task(); // \Swagger\Client\Model\Task | 

try {
    $result = $apiInstance->tasksPutAccount($id, $value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TasksApi->tasksPutAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **value** | [**\Swagger\Client\Model\Task**](../Model/Task.md)|  |

### Return type

[**\Swagger\Client\Model\Task**](../Model/Task.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


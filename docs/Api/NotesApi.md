# Swagger\Client\NotesApi

All URIs are relative to *https://app.practicepanther.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**notesDelete**](NotesApi.md#notesDelete) | **DELETE** /api/v2/notes | 
[**notesGetNote**](NotesApi.md#notesGetNote) | **GET** /api/v2/notes/{id} | 
[**notesGetNotes**](NotesApi.md#notesGetNotes) | **GET** /api/v2/notes | 
[**notesPostNote**](NotesApi.md#notesPostNote) | **POST** /api/v2/notes | 
[**notesPutNote**](NotesApi.md#notesPutNote) | **PUT** /api/v2/notes | 


# **notesDelete**
> \Swagger\Client\Model\Note notesDelete($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\NotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->notesDelete($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NotesApi->notesDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Note**](../Model/Note.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **notesGetNote**
> \Swagger\Client\Model\Note notesGetNote($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\NotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->notesGetNote($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NotesApi->notesGetNote: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Note**](../Model/Note.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **notesGetNotes**
> \Swagger\Client\Model\Note notesGetNotes($assigned_to_user_id, $account_id, $matter_id, $created_since, $updated_since, $date_from, $date_to, $activity_tag)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\NotesApi(
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
    $result = $apiInstance->notesGetNotes($assigned_to_user_id, $account_id, $matter_id, $created_since, $updated_since, $date_from, $date_to, $activity_tag);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NotesApi->notesGetNotes: ', $e->getMessage(), PHP_EOL;
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

[**\Swagger\Client\Model\Note**](../Model/Note.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **notesPostNote**
> \Swagger\Client\Model\Note notesPostNote($value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\NotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\Note(); // \Swagger\Client\Model\Note | 

try {
    $result = $apiInstance->notesPostNote($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NotesApi->notesPostNote: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\Note**](../Model/Note.md)|  |

### Return type

[**\Swagger\Client\Model\Note**](../Model/Note.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **notesPutNote**
> \Swagger\Client\Model\Note notesPutNote($id, $value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\NotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 
$value = new \Swagger\Client\Model\Note(); // \Swagger\Client\Model\Note | 

try {
    $result = $apiInstance->notesPutNote($id, $value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NotesApi->notesPutNote: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **value** | [**\Swagger\Client\Model\Note**](../Model/Note.md)|  |

### Return type

[**\Swagger\Client\Model\Note**](../Model/Note.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


# Swagger\Client\EmailsApi

All URIs are relative to *https://app.practicepanther.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**emailsDelete**](EmailsApi.md#emailsDelete) | **DELETE** /api/v2/emails | 
[**emailsGetEmail**](EmailsApi.md#emailsGetEmail) | **GET** /api/v2/emails/{id} | 
[**emailsGetEmails**](EmailsApi.md#emailsGetEmails) | **GET** /api/v2/emails | 
[**emailsPostEmail**](EmailsApi.md#emailsPostEmail) | **POST** /api/v2/emails | 
[**emailsPutAccount**](EmailsApi.md#emailsPutAccount) | **PUT** /api/v2/emails | 


# **emailsDelete**
> \Swagger\Client\Model\Email emailsDelete($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EmailsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->emailsDelete($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EmailsApi->emailsDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Email**](../Model/Email.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **emailsGetEmail**
> \Swagger\Client\Model\Email emailsGetEmail($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EmailsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->emailsGetEmail($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EmailsApi->emailsGetEmail: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Email**](../Model/Email.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **emailsGetEmails**
> \Swagger\Client\Model\Email emailsGetEmails($assigned_to_user_id, $account_id, $matter_id, $created_since, $updated_since, $activity_tag)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EmailsApi(
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
$activity_tag = "activity_tag_example"; // string | 

try {
    $result = $apiInstance->emailsGetEmails($assigned_to_user_id, $account_id, $matter_id, $created_since, $updated_since, $activity_tag);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EmailsApi->emailsGetEmails: ', $e->getMessage(), PHP_EOL;
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
 **activity_tag** | **string**|  | [optional]

### Return type

[**\Swagger\Client\Model\Email**](../Model/Email.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **emailsPostEmail**
> \Swagger\Client\Model\Email emailsPostEmail($value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EmailsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\Email(); // \Swagger\Client\Model\Email | 

try {
    $result = $apiInstance->emailsPostEmail($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EmailsApi->emailsPostEmail: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\Email**](../Model/Email.md)|  |

### Return type

[**\Swagger\Client\Model\Email**](../Model/Email.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **emailsPutAccount**
> \Swagger\Client\Model\Email emailsPutAccount($id, $value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\EmailsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 
$value = new \Swagger\Client\Model\Email(); // \Swagger\Client\Model\Email | 

try {
    $result = $apiInstance->emailsPutAccount($id, $value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EmailsApi->emailsPutAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **value** | [**\Swagger\Client\Model\Email**](../Model/Email.md)|  |

### Return type

[**\Swagger\Client\Model\Email**](../Model/Email.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


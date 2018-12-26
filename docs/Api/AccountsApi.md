# Swagger\Client\AccountsApi

All URIs are relative to *https://app.practicepanther.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**accountsDelete**](AccountsApi.md#accountsDelete) | **DELETE** /api/v2/accounts | 
[**accountsGetAccount**](AccountsApi.md#accountsGetAccount) | **GET** /api/v2/accounts/{id} | 
[**accountsGetAccounts**](AccountsApi.md#accountsGetAccounts) | **GET** /api/v2/accounts | 
[**accountsPostAccount**](AccountsApi.md#accountsPostAccount) | **POST** /api/v2/accounts | 
[**accountsPutAccount**](AccountsApi.md#accountsPutAccount) | **PUT** /api/v2/accounts | 


# **accountsDelete**
> \Swagger\Client\Model\Account accountsDelete($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\AccountsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->accountsDelete($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountsApi->accountsDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Account**](../Model/Account.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **accountsGetAccount**
> \Swagger\Client\Model\Account accountsGetAccount($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\AccountsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->accountsGetAccount($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountsApi->accountsGetAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Account**](../Model/Account.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **accountsGetAccounts**
> \Swagger\Client\Model\Account accountsGetAccounts($assigned_to_user_id, $created_since, $updated_since, $search_text, $account_tag)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\AccountsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$assigned_to_user_id = "assigned_to_user_id_example"; // string | 
$created_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$updated_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$search_text = "search_text_example"; // string | 
$account_tag = "account_tag_example"; // string | 

try {
    $result = $apiInstance->accountsGetAccounts($assigned_to_user_id, $created_since, $updated_since, $search_text, $account_tag);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountsApi->accountsGetAccounts: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assigned_to_user_id** | **string**|  | [optional]
 **created_since** | **\DateTime**|  | [optional]
 **updated_since** | **\DateTime**|  | [optional]
 **search_text** | **string**|  | [optional]
 **account_tag** | **string**|  | [optional]

### Return type

[**\Swagger\Client\Model\Account**](../Model/Account.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **accountsPostAccount**
> \Swagger\Client\Model\Account accountsPostAccount($value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\AccountsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\Account(); // \Swagger\Client\Model\Account | 

try {
    $result = $apiInstance->accountsPostAccount($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountsApi->accountsPostAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\Account**](../Model/Account.md)|  |

### Return type

[**\Swagger\Client\Model\Account**](../Model/Account.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **accountsPutAccount**
> \Swagger\Client\Model\Account accountsPutAccount($id, $value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\AccountsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 
$value = new \Swagger\Client\Model\Account(); // \Swagger\Client\Model\Account | 

try {
    $result = $apiInstance->accountsPutAccount($id, $value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountsApi->accountsPutAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **value** | [**\Swagger\Client\Model\Account**](../Model/Account.md)|  |

### Return type

[**\Swagger\Client\Model\Account**](../Model/Account.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


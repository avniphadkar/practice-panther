# Swagger\Client\ExpenseCategoriesApi

All URIs are relative to *https://app.practicepanther.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**expenseCategoriesDelete**](ExpenseCategoriesApi.md#expenseCategoriesDelete) | **DELETE** /api/v2/ExpenseCategories | 
[**expenseCategoriesGetExpenseCategories**](ExpenseCategoriesApi.md#expenseCategoriesGetExpenseCategories) | **GET** /api/v2/ExpenseCategories | 
[**expenseCategoriesGetExpenseCategory**](ExpenseCategoriesApi.md#expenseCategoriesGetExpenseCategory) | **GET** /api/v2/ExpenseCategories/{id} | 
[**expenseCategoriesPostExpenseCategory**](ExpenseCategoriesApi.md#expenseCategoriesPostExpenseCategory) | **POST** /api/v2/ExpenseCategories | 
[**expenseCategoriesPutExpenseCategory**](ExpenseCategoriesApi.md#expenseCategoriesPutExpenseCategory) | **PUT** /api/v2/ExpenseCategories | 


# **expenseCategoriesDelete**
> \Swagger\Client\Model\ExpenseCategory expenseCategoriesDelete($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\ExpenseCategoriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->expenseCategoriesDelete($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ExpenseCategoriesApi->expenseCategoriesDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\ExpenseCategory**](../Model/ExpenseCategory.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **expenseCategoriesGetExpenseCategories**
> \Swagger\Client\Model\ExpenseCategory expenseCategoriesGetExpenseCategories($created_since, $updated_since)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\ExpenseCategoriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$created_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$updated_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 

try {
    $result = $apiInstance->expenseCategoriesGetExpenseCategories($created_since, $updated_since);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ExpenseCategoriesApi->expenseCategoriesGetExpenseCategories: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **created_since** | **\DateTime**|  | [optional]
 **updated_since** | **\DateTime**|  | [optional]

### Return type

[**\Swagger\Client\Model\ExpenseCategory**](../Model/ExpenseCategory.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **expenseCategoriesGetExpenseCategory**
> \Swagger\Client\Model\ExpenseCategory expenseCategoriesGetExpenseCategory($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\ExpenseCategoriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->expenseCategoriesGetExpenseCategory($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ExpenseCategoriesApi->expenseCategoriesGetExpenseCategory: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\ExpenseCategory**](../Model/ExpenseCategory.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **expenseCategoriesPostExpenseCategory**
> \Swagger\Client\Model\ExpenseCategory expenseCategoriesPostExpenseCategory($value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\ExpenseCategoriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\ExpenseCategory(); // \Swagger\Client\Model\ExpenseCategory | 

try {
    $result = $apiInstance->expenseCategoriesPostExpenseCategory($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ExpenseCategoriesApi->expenseCategoriesPostExpenseCategory: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\ExpenseCategory**](../Model/ExpenseCategory.md)|  |

### Return type

[**\Swagger\Client\Model\ExpenseCategory**](../Model/ExpenseCategory.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **expenseCategoriesPutExpenseCategory**
> \Swagger\Client\Model\ExpenseCategory expenseCategoriesPutExpenseCategory($id, $value)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\ExpenseCategoriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 
$value = new \Swagger\Client\Model\ExpenseCategory(); // \Swagger\Client\Model\ExpenseCategory | 

try {
    $result = $apiInstance->expenseCategoriesPutExpenseCategory($id, $value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ExpenseCategoriesApi->expenseCategoriesPutExpenseCategory: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **value** | [**\Swagger\Client\Model\ExpenseCategory**](../Model/ExpenseCategory.md)|  |

### Return type

[**\Swagger\Client\Model\ExpenseCategory**](../Model/ExpenseCategory.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


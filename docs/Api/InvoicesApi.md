# Swagger\Client\InvoicesApi

All URIs are relative to *https://app.practicepanther.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**invoicesDelete**](InvoicesApi.md#invoicesDelete) | **DELETE** /api/v2/invoices | 
[**invoicesGetInvoice**](InvoicesApi.md#invoicesGetInvoice) | **GET** /api/v2/invoices/{id} | 
[**invoicesGetInvoices**](InvoicesApi.md#invoicesGetInvoices) | **GET** /api/v2/invoices | 


# **invoicesDelete**
> \Swagger\Client\Model\Invoice invoicesDelete($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\InvoicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->invoicesDelete($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicesApi->invoicesDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **invoicesGetInvoice**
> \Swagger\Client\Model\Invoice invoicesGetInvoice($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\InvoicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->invoicesGetInvoice($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicesApi->invoicesGetInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **invoicesGetInvoices**
> \Swagger\Client\Model\Invoice invoicesGetInvoices($account_id, $matter_id, $created_since, $updated_since, $date_from, $date_to)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\InvoicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$account_id = "account_id_example"; // string | 
$matter_id = "matter_id_example"; // string | 
$created_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$updated_since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$date_from = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 
$date_to = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | 

try {
    $result = $apiInstance->invoicesGetInvoices($account_id, $matter_id, $created_since, $updated_since, $date_from, $date_to);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicesApi->invoicesGetInvoices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **string**|  | [optional]
 **matter_id** | **string**|  | [optional]
 **created_since** | **\DateTime**|  | [optional]
 **updated_since** | **\DateTime**|  | [optional]
 **date_from** | **\DateTime**|  | [optional]
 **date_to** | **\DateTime**|  | [optional]

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


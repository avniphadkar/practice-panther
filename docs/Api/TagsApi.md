# Swagger\Client\TagsApi

All URIs are relative to *https://app.practicepanther.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**tagsGetTagsForAccounts**](TagsApi.md#tagsGetTagsForAccounts) | **GET** /api/v2/tags/account | Returns a list of all tags currently being used for accounts.
[**tagsGetTagsForActivities**](TagsApi.md#tagsGetTagsForActivities) | **GET** /api/v2/tags/activity | Returns a list of all tags currently being used for activites such as tasks, event, call logs, emails and notes.
[**tagsGetTagsForProjects**](TagsApi.md#tagsGetTagsForProjects) | **GET** /api/v2/tags/matter | Returns a list of all tags currently being used for matters.


# **tagsGetTagsForAccounts**
> \Swagger\Client\Model\Tag[] tagsGetTagsForAccounts()

Returns a list of all tags currently being used for accounts.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TagsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->tagsGetTagsForAccounts();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TagsApi->tagsGetTagsForAccounts: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\Tag[]**](../Model/Tag.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **tagsGetTagsForActivities**
> \Swagger\Client\Model\Tag[] tagsGetTagsForActivities()

Returns a list of all tags currently being used for activites such as tasks, event, call logs, emails and notes.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TagsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->tagsGetTagsForActivities();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TagsApi->tagsGetTagsForActivities: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\Tag[]**](../Model/Tag.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **tagsGetTagsForProjects**
> \Swagger\Client\Model\Tag[] tagsGetTagsForProjects()

Returns a list of all tags currently being used for matters.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure OAuth2 access token for authorization: oauth2
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

$apiInstance = new Swagger\Client\Api\TagsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->tagsGetTagsForProjects();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TagsApi->tagsGetTagsForProjects: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\Tag[]**](../Model/Tag.md)

### Authorization

[oauth2](../../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


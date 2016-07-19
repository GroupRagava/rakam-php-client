# Rakam\RetentionApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**analyzeRetention**](RetentionApi.md#analyzeRetention) | **POST** /retention/analyze | Execute query


# **analyzeRetention**
> \client.model\QueryResult analyzeRetention($retention_query)

Execute query



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\RetentionApi();
$retention_query = new \client.model\RetentionQuery(); // \client.model\RetentionQuery | 

try {
    $result = $api_instance->analyzeRetention($retention_query);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RetentionApi->analyzeRetention: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **retention_query** | [**\client.model\RetentionQuery**](../Model/\client.model\RetentionQuery.md)|  |

### Return type

[**\client.model\QueryResult**](../Model/QueryResult.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


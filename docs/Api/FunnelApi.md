# Rakam\FunnelApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**analyzeFunnel**](FunnelApi.md#analyzeFunnel) | **POST** /funnel/analyze | Execute query


# **analyzeFunnel**
> \client.model\QueryResult analyzeFunnel($funnel_query)

Execute query



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\FunnelApi();
$funnel_query = new \client.model\FunnelQuery(); // \client.model\FunnelQuery | 

try {
    $result = $api_instance->analyzeFunnel($funnel_query);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling FunnelApi->analyzeFunnel: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **funnel_query** | [**\client.model\FunnelQuery**](../Model/\client.model\FunnelQuery.md)|  |

### Return type

[**\client.model\QueryResult**](../Model/QueryResult.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


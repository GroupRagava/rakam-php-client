# Rakam\QueryApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**execute**](QueryApi.md#execute) | **POST** /query/execute | Execute query on event data-set
[**explain**](QueryApi.md#explain) | **POST** /query/explain | Explain query
[**metadata**](QueryApi.md#metadata) | **POST** /query/metadata | Test query


# **execute**
> \client.model\QueryResult execute($execute)

Execute query on event data-set



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\QueryApi();
$execute = new \client.model\Execute(); // \client.model\Execute | 

try {
    $result = $api_instance->execute($execute);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QueryApi->execute: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **execute** | [**\client.model\Execute**](../Model/\client.model\Execute.md)|  |

### Return type

[**\client.model\QueryResult**](../Model/QueryResult.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **explain**
> \client.model\ResponseQuery explain($explain)

Explain query



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\QueryApi();
$explain = new \client.model\Explain(); // \client.model\Explain | 

try {
    $result = $api_instance->explain($explain);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QueryApi->explain: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **explain** | [**\client.model\Explain**](../Model/\client.model\Explain.md)|  |

### Return type

[**\client.model\ResponseQuery**](../Model/ResponseQuery.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **metadata**
> \client.model\SchemaField[] metadata($query_metadata)

Test query



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\QueryApi();
$query_metadata = new \client.model\QueryMetadata(); // \client.model\QueryMetadata | 

try {
    $result = $api_instance->metadata($query_metadata);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QueryApi->metadata: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query_metadata** | [**\client.model\QueryMetadata**](../Model/\client.model\QueryMetadata.md)|  |

### Return type

[**\client.model\SchemaField[]**](../Model/SchemaField.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


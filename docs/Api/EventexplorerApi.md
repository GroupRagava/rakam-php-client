# Rakam\EventexplorerApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**analyzeEvents**](EventexplorerApi.md#analyzeEvents) | **POST** /event-explorer/analyze | Perform simple query on event data
[**createPrecomputedTable**](EventexplorerApi.md#createPrecomputedTable) | **POST** /event-explorer/pre_calculate | Create Pre-computed table
[**getEventStatistics**](EventexplorerApi.md#getEventStatistics) | **POST** /event-explorer/statistics | Event statistics
[**getExtraDimensions**](EventexplorerApi.md#getExtraDimensions) | **GET** /event-explorer/extra_dimensions | Event statistics


# **analyzeEvents**
> \client.model\QueryResult analyzeEvents($analyze_request)

Perform simple query on event data



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\EventexplorerApi();
$analyze_request = new \client.model\AnalyzeRequest(); // \client.model\AnalyzeRequest | 

try {
    $result = $api_instance->analyzeEvents($analyze_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventexplorerApi->analyzeEvents: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **analyze_request** | [**\client.model\AnalyzeRequest**](../Model/\client.model\AnalyzeRequest.md)|  |

### Return type

[**\client.model\QueryResult**](../Model/QueryResult.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createPrecomputedTable**
> \client.model\PrecalculatedTable createPrecomputedTable($create_precomputed_table)

Create Pre-computed table



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\EventexplorerApi();
$create_precomputed_table = new \client.model\CreatePrecomputedTable(); // \client.model\CreatePrecomputedTable | 

try {
    $result = $api_instance->createPrecomputedTable($create_precomputed_table);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventexplorerApi->createPrecomputedTable: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_precomputed_table** | [**\client.model\CreatePrecomputedTable**](../Model/\client.model\CreatePrecomputedTable.md)|  |

### Return type

[**\client.model\PrecalculatedTable**](../Model/PrecalculatedTable.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getEventStatistics**
> \client.model\QueryResult getEventStatistics($event_explorer_get_event_statistics)

Event statistics



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\EventexplorerApi();
$event_explorer_get_event_statistics = new \client.model\EventExplorerGetEventStatistics(); // \client.model\EventExplorerGetEventStatistics | 

try {
    $result = $api_instance->getEventStatistics($event_explorer_get_event_statistics);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventexplorerApi->getEventStatistics: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **event_explorer_get_event_statistics** | [**\client.model\EventExplorerGetEventStatistics**](../Model/\client.model\EventExplorerGetEventStatistics.md)|  |

### Return type

[**\client.model\QueryResult**](../Model/QueryResult.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getExtraDimensions**
> map[string,string[]] getExtraDimensions()

Event statistics



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\EventexplorerApi();

try {
    $result = $api_instance->getExtraDimensions();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventexplorerApi->getExtraDimensions: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**map[string,string[]]**](../Model/array.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


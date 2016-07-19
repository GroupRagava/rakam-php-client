# Rakam\RealtimeApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createTable**](RealtimeApi.md#createTable) | **POST** /realtime/create | Create report
[**deleteTable**](RealtimeApi.md#deleteTable) | **POST** /realtime/delete | Delete report
[**listTables**](RealtimeApi.md#listTables) | **POST** /realtime/list | List queries
[**queryTable**](RealtimeApi.md#queryTable) | **POST** /realtime/get | Get report


# **createTable**
> \client.model\SuccessMessage createTable($real_time_report)

Create report



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\RealtimeApi();
$real_time_report = new \client.model\RealTimeReport(); // \client.model\RealTimeReport | 

try {
    $result = $api_instance->createTable($real_time_report);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RealtimeApi->createTable: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **real_time_report** | [**\client.model\RealTimeReport**](../Model/\client.model\RealTimeReport.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteTable**
> \client.model\SuccessMessage deleteTable($realtime_delete_table)

Delete report



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\RealtimeApi();
$realtime_delete_table = new \client.model\RealtimeDeleteTable(); // \client.model\RealtimeDeleteTable | 

try {
    $result = $api_instance->deleteTable($realtime_delete_table);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RealtimeApi->deleteTable: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **realtime_delete_table** | [**\client.model\RealtimeDeleteTable**](../Model/\client.model\RealtimeDeleteTable.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listTables**
> \client.model\ContinuousQuery[] listTables()

List queries



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\RealtimeApi();

try {
    $result = $api_instance->listTables();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RealtimeApi->listTables: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\client.model\ContinuousQuery[]**](../Model/ContinuousQuery.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **queryTable**
> \client.model\RealTimeQueryResult queryTable($realtime_query_table)

Get report



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\RealtimeApi();
$realtime_query_table = new \client.model\RealtimeQueryTable(); // \client.model\RealtimeQueryTable | 

try {
    $result = $api_instance->queryTable($realtime_query_table);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RealtimeApi->queryTable: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **realtime_query_table** | [**\client.model\RealtimeQueryTable**](../Model/\client.model\RealtimeQueryTable.md)|  |

### Return type

[**\client.model\RealTimeQueryResult**](../Model/RealTimeQueryResult.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


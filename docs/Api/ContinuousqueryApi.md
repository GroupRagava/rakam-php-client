# Rakam\ContinuousqueryApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createQuery**](ContinuousqueryApi.md#createQuery) | **POST** /continuous-query/create | Create stream
[**deleteQuery**](ContinuousqueryApi.md#deleteQuery) | **POST** /continuous-query/delete | Delete stream
[**getQuery**](ContinuousqueryApi.md#getQuery) | **POST** /continuous-query/get | Get continuous query
[**getSchemaOfQuery**](ContinuousqueryApi.md#getSchemaOfQuery) | **POST** /continuous-query/schema | Get query schema
[**listQueries**](ContinuousqueryApi.md#listQueries) | **POST** /continuous-query/list | List queries
[**testQuery**](ContinuousqueryApi.md#testQuery) | **POST** /continuous-query/test | Test continuous query


# **createQuery**
> \client.model\SuccessMessage createQuery($continuous_query)

Create stream

Creates a new continuous query for specified SQL query. Rakam will process data in batches keep the result of query in-memory all the time. Compared to reports, continuous queries continuously aggregate the data on the fly and the result is always available either in-memory or disk.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\ContinuousqueryApi();
$continuous_query = new \client.model\ContinuousQuery(); // \client.model\ContinuousQuery | 

try {
    $result = $api_instance->createQuery($continuous_query);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContinuousqueryApi->createQuery: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **continuous_query** | [**\client.model\ContinuousQuery**](../Model/\client.model\ContinuousQuery.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteQuery**
> \client.model\SuccessMessage deleteQuery($continuous_query_delete_query)

Delete stream



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\ContinuousqueryApi();
$continuous_query_delete_query = new \client.model\ContinuousQueryDeleteQuery(); // \client.model\ContinuousQueryDeleteQuery | 

try {
    $result = $api_instance->deleteQuery($continuous_query_delete_query);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContinuousqueryApi->deleteQuery: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **continuous_query_delete_query** | [**\client.model\ContinuousQueryDeleteQuery**](../Model/\client.model\ContinuousQueryDeleteQuery.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getQuery**
> \client.model\ContinuousQuery getQuery($continuous_query_get_query)

Get continuous query



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\ContinuousqueryApi();
$continuous_query_get_query = new \client.model\ContinuousQueryGetQuery(); // \client.model\ContinuousQueryGetQuery | 

try {
    $result = $api_instance->getQuery($continuous_query_get_query);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContinuousqueryApi->getQuery: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **continuous_query_get_query** | [**\client.model\ContinuousQueryGetQuery**](../Model/\client.model\ContinuousQueryGetQuery.md)|  |

### Return type

[**\client.model\ContinuousQuery**](../Model/ContinuousQuery.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSchemaOfQuery**
> \client.model\Collection[] getSchemaOfQuery($continuous_query_get_schema_of_query)

Get query schema



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\ContinuousqueryApi();
$continuous_query_get_schema_of_query = new \client.model\ContinuousQueryGetSchemaOfQuery(); // \client.model\ContinuousQueryGetSchemaOfQuery | 

try {
    $result = $api_instance->getSchemaOfQuery($continuous_query_get_schema_of_query);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContinuousqueryApi->getSchemaOfQuery: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **continuous_query_get_schema_of_query** | [**\client.model\ContinuousQueryGetSchemaOfQuery**](../Model/\client.model\ContinuousQueryGetSchemaOfQuery.md)|  |

### Return type

[**\client.model\Collection[]**](../Model/Collection.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listQueries**
> \client.model\ContinuousQuery[] listQueries()

List queries



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\ContinuousqueryApi();

try {
    $result = $api_instance->listQueries();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContinuousqueryApi->listQueries: ', $e->getMessage(), PHP_EOL;
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

# **testQuery**
> bool testQuery($continuous_query_test_query)

Test continuous query



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\ContinuousqueryApi();
$continuous_query_test_query = new \client.model\ContinuousQueryTestQuery(); // \client.model\ContinuousQueryTestQuery | 

try {
    $result = $api_instance->testQuery($continuous_query_test_query);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContinuousqueryApi->testQuery: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **continuous_query_test_query** | [**\client.model\ContinuousQueryTestQuery**](../Model/\client.model\ContinuousQueryTestQuery.md)|  |

### Return type

**bool**

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


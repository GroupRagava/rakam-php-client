# Rakam\MaterializedviewApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createView**](MaterializedviewApi.md#createView) | **POST** /materialized-view/create | Create view
[**deleteView**](MaterializedviewApi.md#deleteView) | **POST** /materialized-view/delete | Delete materialized view
[**getSchemaOfView**](MaterializedviewApi.md#getSchemaOfView) | **POST** /materialized-view/schema | Get schemas
[**getView**](MaterializedviewApi.md#getView) | **POST** /materialized-view/get | Get view
[**listViews**](MaterializedviewApi.md#listViews) | **POST** /materialized-view/list | List views


# **createView**
> \client.model\SuccessMessage createView($materialized_view)

Create view



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\MaterializedviewApi();
$materialized_view = new \client.model\MaterializedView(); // \client.model\MaterializedView | 

try {
    $result = $api_instance->createView($materialized_view);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MaterializedviewApi->createView: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **materialized_view** | [**\client.model\MaterializedView**](../Model/\client.model\MaterializedView.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteView**
> \client.model\SuccessMessage deleteView($materialized_view_delete_view)

Delete materialized view



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\MaterializedviewApi();
$materialized_view_delete_view = new \client.model\MaterializedViewDeleteView(); // \client.model\MaterializedViewDeleteView | 

try {
    $result = $api_instance->deleteView($materialized_view_delete_view);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MaterializedviewApi->deleteView: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **materialized_view_delete_view** | [**\client.model\MaterializedViewDeleteView**](../Model/\client.model\MaterializedViewDeleteView.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSchemaOfView**
> \client.model\MaterializedViewSchema[] getSchemaOfView($materialized_view_get_schema_of_view)

Get schemas



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\MaterializedviewApi();
$materialized_view_get_schema_of_view = new \client.model\MaterializedViewGetSchemaOfView(); // \client.model\MaterializedViewGetSchemaOfView | 

try {
    $result = $api_instance->getSchemaOfView($materialized_view_get_schema_of_view);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MaterializedviewApi->getSchemaOfView: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **materialized_view_get_schema_of_view** | [**\client.model\MaterializedViewGetSchemaOfView**](../Model/\client.model\MaterializedViewGetSchemaOfView.md)|  |

### Return type

[**\client.model\MaterializedViewSchema[]**](../Model/MaterializedViewSchema.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getView**
> \client.model\MaterializedView getView($materialized_view_get_view)

Get view



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\MaterializedviewApi();
$materialized_view_get_view = new \client.model\MaterializedViewGetView(); // \client.model\MaterializedViewGetView | 

try {
    $result = $api_instance->getView($materialized_view_get_view);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MaterializedviewApi->getView: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **materialized_view_get_view** | [**\client.model\MaterializedViewGetView**](../Model/\client.model\MaterializedViewGetView.md)|  |

### Return type

[**\client.model\MaterializedView**](../Model/MaterializedView.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listViews**
> \client.model\MaterializedView[] listViews()

List views



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\MaterializedviewApi();

try {
    $result = $api_instance->listViews();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MaterializedviewApi->listViews: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\client.model\MaterializedView[]**](../Model/MaterializedView.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


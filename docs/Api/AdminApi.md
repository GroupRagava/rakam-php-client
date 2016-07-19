# Rakam\AdminApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addCustomFieldsToSchema**](AdminApi.md#addCustomFieldsToSchema) | **POST** /project/schema/add/custom | Add fields to collections by transforming other schemas
[**addFieldsToSchema**](AdminApi.md#addFieldsToSchema) | **POST** /project/schema/add | Add fields to collections
[**checkApiKeys**](AdminApi.md#checkApiKeys) | **POST** /project/check-api-keys | Create API Keys
[**checkLockKey**](AdminApi.md#checkLockKey) | **POST** /admin/lock_key | Check lock key
[**collections**](AdminApi.md#collections) | **POST** /project/collection | Get collection names
[**createApiKeys**](AdminApi.md#createApiKeys) | **POST** /project/create-api-keys | Create API Keys
[**createProject**](AdminApi.md#createProject) | **POST** /project/create | Create project
[**deleteProject**](AdminApi.md#deleteProject) | **DELETE** /project/delete | Delete project
[**getConfigurations**](AdminApi.md#getConfigurations) | **GET** /admin/configurations | List installed modules
[**getProjects**](AdminApi.md#getProjects) | **GET** /project/list | List created projects
[**getStats**](AdminApi.md#getStats) | **POST** /project/stats | Get project stats
[**getTypes**](AdminApi.md#getTypes) | **GET** /admin/types | Get types
[**revokeApiKeys**](AdminApi.md#revokeApiKeys) | **DELETE** /project/revoke-api-keys | Revoke API Keys
[**schema**](AdminApi.md#schema) | **POST** /project/schema | Get collection schema


# **addCustomFieldsToSchema**
> \client.model\SchemaField[] addCustomFieldsToSchema($project_add_custom_fields_to_schema)

Add fields to collections by transforming other schemas



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();
$project_add_custom_fields_to_schema = new \client.model\ProjectAddCustomFieldsToSchema(); // \client.model\ProjectAddCustomFieldsToSchema | 

try {
    $result = $api_instance->addCustomFieldsToSchema($project_add_custom_fields_to_schema);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->addCustomFieldsToSchema: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_add_custom_fields_to_schema** | [**\client.model\ProjectAddCustomFieldsToSchema**](../Model/\client.model\ProjectAddCustomFieldsToSchema.md)|  |

### Return type

[**\client.model\SchemaField[]**](../Model/SchemaField.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **addFieldsToSchema**
> \client.model\SchemaField[] addFieldsToSchema($project_add_fields_to_schema)

Add fields to collections



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();
$project_add_fields_to_schema = new \client.model\ProjectAddFieldsToSchema(); // \client.model\ProjectAddFieldsToSchema | 

try {
    $result = $api_instance->addFieldsToSchema($project_add_fields_to_schema);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->addFieldsToSchema: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_add_fields_to_schema** | [**\client.model\ProjectAddFieldsToSchema**](../Model/\client.model\ProjectAddFieldsToSchema.md)|  |

### Return type

[**\client.model\SchemaField[]**](../Model/SchemaField.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **checkApiKeys**
> bool[] checkApiKeys($project_check_api_keys)

Create API Keys



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\AdminApi();
$project_check_api_keys = new \client.model\ProjectCheckApiKeys(); // \client.model\ProjectCheckApiKeys | 

try {
    $result = $api_instance->checkApiKeys($project_check_api_keys);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->checkApiKeys: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_check_api_keys** | [**\client.model\ProjectCheckApiKeys**](../Model/\client.model\ProjectCheckApiKeys.md)|  |

### Return type

**bool[]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **checkLockKey**
> bool checkLockKey($check_lock_key)

Check lock key



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();
$check_lock_key = new \client.model\CheckLockKey(); // \client.model\CheckLockKey | 

try {
    $result = $api_instance->checkLockKey($check_lock_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->checkLockKey: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **check_lock_key** | [**\client.model\CheckLockKey**](../Model/\client.model\CheckLockKey.md)|  |

### Return type

**bool**

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **collections**
> string[] collections()

Get collection names



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();

try {
    $result = $api_instance->collections();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->collections: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

**string[]**

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createApiKeys**
> \client.model\ProjectApiKeys createApiKeys()

Create API Keys



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();

try {
    $result = $api_instance->createApiKeys();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->createApiKeys: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\client.model\ProjectApiKeys**](../Model/ProjectApiKeys.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createProject**
> \client.model\ProjectApiKeys createProject($create_project)

Create project



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\AdminApi();
$create_project = new \client.model\CreateProject(); // \client.model\CreateProject | 

try {
    $result = $api_instance->createProject($create_project);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->createProject: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_project** | [**\client.model\CreateProject**](../Model/\client.model\CreateProject.md)|  |

### Return type

[**\client.model\ProjectApiKeys**](../Model/ProjectApiKeys.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteProject**
> \client.model\SuccessMessage deleteProject()

Delete project



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();

try {
    $result = $api_instance->deleteProject();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->deleteProject: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getConfigurations**
> \client.model\ModuleDescriptor[] getConfigurations()

List installed modules



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();

try {
    $result = $api_instance->getConfigurations();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->getConfigurations: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\client.model\ModuleDescriptor[]**](../Model/ModuleDescriptor.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getProjects**
> string[] getProjects()

List created projects



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();

try {
    $result = $api_instance->getProjects();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->getProjects: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

**string[]**

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getStats**
> map[string,\client.model\Stats] getStats($project_get_stats)

Get project stats



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\AdminApi();
$project_get_stats = new \client.model\ProjectGetStats(); // \client.model\ProjectGetStats | 

try {
    $result = $api_instance->getStats($project_get_stats);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->getStats: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_get_stats** | [**\client.model\ProjectGetStats**](../Model/\client.model\ProjectGetStats.md)|  |

### Return type

[**map[string,\client.model\Stats]**](../Model/Stats.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getTypes**
> map[string,string] getTypes()

Get types



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();

try {
    $result = $api_instance->getTypes();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->getTypes: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**map[string,string]**](../Model/map.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **revokeApiKeys**
> \client.model\SuccessMessage revokeApiKeys($master_key)

Revoke API Keys



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();
$master_key = "master_key_example"; // string | 

try {
    $result = $api_instance->revokeApiKeys($master_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->revokeApiKeys: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **master_key** | **string**|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **schema**
> \client.model\Collection[] schema($project_schema)

Get collection schema



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\AdminApi();
$project_schema = new \client.model\ProjectSchema(); // \client.model\ProjectSchema | 

try {
    $result = $api_instance->schema($project_schema);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AdminApi->schema: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_schema** | [**\client.model\ProjectSchema**](../Model/\client.model\ProjectSchema.md)|  |

### Return type

[**\client.model\Collection[]**](../Model/Collection.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


# Rakam\UseractionApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**batch**](UseractionApi.md#batch) | **POST** /user/action/email/batch | Apply batch operation
[**send**](UseractionApi.md#send) | **POST** /user/action/email/single | Perform action for single user


# **batch**
> int batch($user_email_action_batch)

Apply batch operation



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\UseractionApi();
$user_email_action_batch = new \client.model\UserEmailActionBatch(); // \client.model\UserEmailActionBatch | 

try {
    $result = $api_instance->batch($user_email_action_batch);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UseractionApi->batch: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_email_action_batch** | [**\client.model\UserEmailActionBatch**](../Model/\client.model\UserEmailActionBatch.md)|  |

### Return type

**int**

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **send**
> bool send($user_email_action_send)

Perform action for single user



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\UseractionApi();
$user_email_action_send = new \client.model\UserEmailActionSend(); // \client.model\UserEmailActionSend | 

try {
    $result = $api_instance->send($user_email_action_send);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UseractionApi->send: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_email_action_send** | [**\client.model\UserEmailActionSend**](../Model/\client.model\UserEmailActionSend.md)|  |

### Return type

**bool**

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


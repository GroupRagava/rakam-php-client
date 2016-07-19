# Rakam\RecipeApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**exportRecipe**](RecipeApi.md#exportRecipe) | **GET** /recipe/export | Export recipe
[**installRecipe**](RecipeApi.md#installRecipe) | **POST** /recipe/install | Install recipe


# **exportRecipe**
> \client.model\Recipe exportRecipe($accept)

Export recipe



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\RecipeApi();
$accept = "accept_example"; // string | 

try {
    $result = $api_instance->exportRecipe($accept);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RecipeApi->exportRecipe: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **string**|  |

### Return type

[**\client.model\Recipe**](../Model/Recipe.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **installRecipe**
> \client.model\SuccessMessage installRecipe()

Install recipe



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\RecipeApi();

try {
    $result = $api_instance->installRecipe();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RecipeApi->installRecipe: ', $e->getMessage(), PHP_EOL;
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


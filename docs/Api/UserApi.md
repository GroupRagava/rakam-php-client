# Rakam\UserApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSegment**](UserApi.md#createSegment) | **POST** /user/create_segment | Get events of the user
[**createUser**](UserApi.md#createUser) | **POST** /user/create | Create new user
[**createUsers**](UserApi.md#createUsers) | **POST** /user/batch/create | Create multiple new users
[**getEvents**](UserApi.md#getEvents) | **POST** /user/get_events | Get events of the user
[**getMetadata**](UserApi.md#getMetadata) | **GET** /user/metadata | Get user storage metadata
[**getUser**](UserApi.md#getUser) | **POST** /user/get | Get user
[**incrementProperty**](UserApi.md#incrementProperty) | **POST** /user/increment_property | Set user property
[**searchUsers**](UserApi.md#searchUsers) | **POST** /user/search | Search users
[**setProperties**](UserApi.md#setProperties) | **POST** /user/set_properties | Set user properties
[**setPropertiesOnce**](UserApi.md#setPropertiesOnce) | **POST** /user/set_properties_once | Set user properties once
[**unsetProperty**](UserApi.md#unsetProperty) | **POST** /user/unset_properties | Unset user property


# **createSegment**
> \client.model\SuccessMessage createSegment($user_create_segment)

Get events of the user



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\UserApi();
$user_create_segment = new \client.model\UserCreateSegment(); // \client.model\UserCreateSegment | 

try {
    $result = $api_instance->createSegment($user_create_segment);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createSegment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_create_segment** | [**\client.model\UserCreateSegment**](../Model/\client.model\UserCreateSegment.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUser**
> int createUser($user)

Create new user



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\UserApi();
$user = new \client.model\User(); // \client.model\User | 

try {
    $result = $api_instance->createUser($user);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | [**\client.model\User**](../Model/\client.model\User.md)|  |

### Return type

**int**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUsers**
> object[] createUsers($user_create_users)

Create multiple new users

Returns user ids. User id may be string or numeric.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: write_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('write_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('write_key', 'Bearer');

$api_instance = new Rakam\Api\UserApi();
$user_create_users = new \client.model\UserCreateUsers(); // \client.model\UserCreateUsers | 

try {
    $result = $api_instance->createUsers($user_create_users);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createUsers: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_create_users** | [**\client.model\UserCreateUsers**](../Model/\client.model\UserCreateUsers.md)|  |

### Return type

**object[]**

### Authorization

[write_key](../../README.md#write_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getEvents**
> \client.model\CollectionEvent[] getEvents($user_get_events)

Get events of the user



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\UserApi();
$user_get_events = new \client.model\UserGetEvents(); // \client.model\UserGetEvents | 

try {
    $result = $api_instance->getEvents($user_get_events);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->getEvents: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_get_events** | [**\client.model\UserGetEvents**](../Model/\client.model\UserGetEvents.md)|  |

### Return type

[**\client.model\CollectionEvent[]**](../Model/CollectionEvent.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getMetadata**
> \client.model\MetadataResponse getMetadata()

Get user storage metadata



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\UserApi();

try {
    $result = $api_instance->getMetadata();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->getMetadata: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\client.model\MetadataResponse**](../Model/MetadataResponse.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getUser**
> \client.model\User getUser($user_get_user)

Get user



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\UserApi();
$user_get_user = new \client.model\UserGetUser(); // \client.model\UserGetUser | 

try {
    $result = $api_instance->getUser($user_get_user);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->getUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_get_user** | [**\client.model\UserGetUser**](../Model/\client.model\UserGetUser.md)|  |

### Return type

[**\client.model\User**](../Model/User.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **incrementProperty**
> \client.model\SuccessMessage incrementProperty($user_increment_property)

Set user property



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\UserApi();
$user_increment_property = new \client.model\UserIncrementProperty(); // \client.model\UserIncrementProperty | 

try {
    $result = $api_instance->incrementProperty($user_increment_property);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->incrementProperty: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_increment_property** | [**\client.model\UserIncrementProperty**](../Model/\client.model\UserIncrementProperty.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchUsers**
> \client.model\QueryResult searchUsers($user_search_users)

Search users



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: read_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('read_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('read_key', 'Bearer');

$api_instance = new Rakam\Api\UserApi();
$user_search_users = new \client.model\UserSearchUsers(); // \client.model\UserSearchUsers | 

try {
    $result = $api_instance->searchUsers($user_search_users);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->searchUsers: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_search_users** | [**\client.model\UserSearchUsers**](../Model/\client.model\UserSearchUsers.md)|  |

### Return type

[**\client.model\QueryResult**](../Model/QueryResult.md)

### Authorization

[read_key](../../README.md#read_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **setProperties**
> int setProperties($user)

Set user properties



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\UserApi();
$user = new \client.model\User(); // \client.model\User | 

try {
    $result = $api_instance->setProperties($user);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->setProperties: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | [**\client.model\User**](../Model/\client.model\User.md)|  |

### Return type

**int**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **setPropertiesOnce**
> int setPropertiesOnce($user)

Set user properties once



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\UserApi();
$user = new \client.model\User(); // \client.model\User | 

try {
    $result = $api_instance->setPropertiesOnce($user);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->setPropertiesOnce: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | [**\client.model\User**](../Model/\client.model\User.md)|  |

### Return type

**int**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **unsetProperty**
> \client.model\SuccessMessage unsetProperty($user_unset_property)

Unset user property



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\UserApi();
$user_unset_property = new \client.model\UserUnsetProperty(); // \client.model\UserUnsetProperty | 

try {
    $result = $api_instance->unsetProperty($user_unset_property);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->unsetProperty: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_unset_property** | [**\client.model\UserUnsetProperty**](../Model/\client.model\UserUnsetProperty.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


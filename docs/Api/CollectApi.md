# Rakam\CollectApi

All URIs are relative to *https://app.rakam.io/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**batchEvents**](CollectApi.md#batchEvents) | **POST** /event/batch | Collect multiple events
[**bulkEvents**](CollectApi.md#bulkEvents) | **POST** /event/bulk | Collect Bulk events
[**bulkEventsRemote**](CollectApi.md#bulkEventsRemote) | **POST** /event/bulk/remote | Collect bulk events from remote
[**collectEvent**](CollectApi.md#collectEvent) | **POST** /event/collect | Collect event
[**commitBulkEvents**](CollectApi.md#commitBulkEvents) | **POST** /event/bulk/commit | Commit Bulk events


# **batchEvents**
> int batchEvents($event_list)

Collect multiple events

Returns 1 if the events are collected.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\CollectApi();
$event_list = new \client.model\EventList(); // \client.model\EventList | 

try {
    $result = $api_instance->batchEvents($event_list);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectApi->batchEvents: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **event_list** | [**\client.model\EventList**](../Model/\client.model\EventList.md)|  |

### Return type

**int**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **bulkEvents**
> \client.model\SuccessMessage bulkEvents($event_list)

Collect Bulk events

Bulk API requires master_key as api key and designed to handle large value of data. The endpoint also accepts application/avro and text/csv formats. You need need to set 'collection' and 'master_key' query parameters if the content-type is not application/json.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\CollectApi();
$event_list = new \client.model\EventList(); // \client.model\EventList | 

try {
    $result = $api_instance->bulkEvents($event_list);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectApi->bulkEvents: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **event_list** | [**\client.model\EventList**](../Model/\client.model\EventList.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **bulkEventsRemote**
> int bulkEventsRemote($bulk_event_remote)

Collect bulk events from remote



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\CollectApi();
$bulk_event_remote = new \client.model\BulkEventRemote(); // \client.model\BulkEventRemote | 

try {
    $result = $api_instance->bulkEventsRemote($bulk_event_remote);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectApi->bulkEventsRemote: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulk_event_remote** | [**\client.model\BulkEventRemote**](../Model/\client.model\BulkEventRemote.md)|  |

### Return type

**int**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **collectEvent**
> int collectEvent($event)

Collect event



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Rakam\Api\CollectApi();
$event = new \client.model\Event(); // \client.model\Event | 

try {
    $result = $api_instance->collectEvent($event);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectApi->collectEvent: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **event** | [**\client.model\Event**](../Model/\client.model\Event.md)|  |

### Return type

**int**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **commitBulkEvents**
> \client.model\SuccessMessage commitBulkEvents($commit_bulk_events)

Commit Bulk events



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: master_key
Rakam\Configuration::getDefaultConfiguration()->setApiKey('master_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Rakam\Configuration::getDefaultConfiguration()->setApiKeyPrefix('master_key', 'Bearer');

$api_instance = new Rakam\Api\CollectApi();
$commit_bulk_events = new \client.model\CommitBulkEvents(); // \client.model\CommitBulkEvents | 

try {
    $result = $api_instance->commitBulkEvents($commit_bulk_events);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectApi->commitBulkEvents: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **commit_bulk_events** | [**\client.model\CommitBulkEvents**](../Model/\client.model\CommitBulkEvents.md)|  |

### Return type

[**\client.model\SuccessMessage**](../Model/SuccessMessage.md)

### Authorization

[master_key](../../README.md#master_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


# valstorm_api.NotificationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**mark_notification_as_read_v1_notifications_mark_read_post**](NotificationsApi.md#mark_notification_as_read_v1_notifications_mark_read_post) | **POST** /v1/notifications/mark-read | Mark Notification As Read
[**mark_notification_data_as_read_v1_notifications_mark_read_by_key_value_post**](NotificationsApi.md#mark_notification_data_as_read_v1_notifications_mark_read_by_key_value_post) | **POST** /v1/notifications/mark-read-by-key-value | Mark Notification Data As Read
[**send_dynamic_notification_route_v1_notifications_dynamic_post**](NotificationsApi.md#send_dynamic_notification_route_v1_notifications_dynamic_post) | **POST** /v1/notifications/dynamic | Send Dynamic Notification Route
[**send_notification_route_v1_notifications_post**](NotificationsApi.md#send_notification_route_v1_notifications_post) | **POST** /v1/notifications | Send Notification Route
[**send_notification_v1_notifications_send_post**](NotificationsApi.md#send_notification_v1_notifications_send_post) | **POST** /v1/notifications/send | Send Notification
[**set_notification_token_v1_notifications_set_token_post**](NotificationsApi.md#set_notification_token_v1_notifications_set_token_post) | **POST** /v1/notifications/set-token | Set Notification Token


# **mark_notification_as_read_v1_notifications_mark_read_post**
> MarketAsReadResponse mark_notification_as_read_v1_notifications_mark_read_post(request_body)

Mark Notification As Read

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.market_as_read_response import MarketAsReadResponse
from valstorm_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = valstorm_api.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with valstorm_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = valstorm_api.NotificationsApi(api_client)
    request_body = ['request_body_example'] # List[str] | 

    try:
        # Mark Notification As Read
        api_response = api_instance.mark_notification_as_read_v1_notifications_mark_read_post(request_body)
        print("The response of NotificationsApi->mark_notification_as_read_v1_notifications_mark_read_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->mark_notification_as_read_v1_notifications_mark_read_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request_body** | [**List[str]**](str.md)|  | 

### Return type

[**MarketAsReadResponse**](MarketAsReadResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **mark_notification_data_as_read_v1_notifications_mark_read_by_key_value_post**
> object mark_notification_data_as_read_v1_notifications_mark_read_by_key_value_post(data)

Mark Notification Data As Read

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.data import Data
from valstorm_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = valstorm_api.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with valstorm_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = valstorm_api.NotificationsApi(api_client)
    data = valstorm_api.Data() # Data | 

    try:
        # Mark Notification Data As Read
        api_response = api_instance.mark_notification_data_as_read_v1_notifications_mark_read_by_key_value_post(data)
        print("The response of NotificationsApi->mark_notification_data_as_read_v1_notifications_mark_read_by_key_value_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->mark_notification_data_as_read_v1_notifications_mark_read_by_key_value_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Data**](Data.md)|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_dynamic_notification_route_v1_notifications_dynamic_post**
> object send_dynamic_notification_route_v1_notifications_dynamic_post(requests)

Send Dynamic Notification Route

Summary: Send a dynamic notification without needing a predefined setting.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.requests import Requests
from valstorm_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = valstorm_api.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with valstorm_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = valstorm_api.NotificationsApi(api_client)
    requests = valstorm_api.Requests() # Requests | 

    try:
        # Send Dynamic Notification Route
        api_response = api_instance.send_dynamic_notification_route_v1_notifications_dynamic_post(requests)
        print("The response of NotificationsApi->send_dynamic_notification_route_v1_notifications_dynamic_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->send_dynamic_notification_route_v1_notifications_dynamic_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **requests** | [**Requests**](Requests.md)|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_notification_route_v1_notifications_post**
> object send_notification_route_v1_notifications_post(send_notification_setting)

Send Notification Route

Summary: Send a notification to a user.
Parameters:
    - notification: The notification to send.
    - current_user: The current user.
    - background_tasks: The background tasks.
Returns:
    - A JSON response with the status of the notification.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.send_notification_setting import SendNotificationSetting
from valstorm_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = valstorm_api.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with valstorm_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = valstorm_api.NotificationsApi(api_client)
    send_notification_setting = [valstorm_api.SendNotificationSetting()] # List[SendNotificationSetting] | 

    try:
        # Send Notification Route
        api_response = api_instance.send_notification_route_v1_notifications_post(send_notification_setting)
        print("The response of NotificationsApi->send_notification_route_v1_notifications_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->send_notification_route_v1_notifications_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_notification_setting** | [**List[SendNotificationSetting]**](SendNotificationSetting.md)|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_notification_v1_notifications_send_post**
> object send_notification_v1_notifications_send_post(web_notification)

Send Notification

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.web_notification import WebNotification
from valstorm_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = valstorm_api.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with valstorm_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = valstorm_api.NotificationsApi(api_client)
    web_notification = valstorm_api.WebNotification() # WebNotification | 

    try:
        # Send Notification
        api_response = api_instance.send_notification_v1_notifications_send_post(web_notification)
        print("The response of NotificationsApi->send_notification_v1_notifications_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->send_notification_v1_notifications_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **web_notification** | [**WebNotification**](WebNotification.md)|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_notification_token_v1_notifications_set_token_post**
> object set_notification_token_v1_notifications_set_token_post(request_body)

Set Notification Token

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = valstorm_api.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with valstorm_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = valstorm_api.NotificationsApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Set Notification Token
        api_response = api_instance.set_notification_token_v1_notifications_set_token_post(request_body)
        print("The response of NotificationsApi->set_notification_token_v1_notifications_set_token_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->set_notification_token_v1_notifications_set_token_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request_body** | [**Dict[str, object]**](object.md)|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


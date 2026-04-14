# valstorm_api.MicrosoftApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**callback_microsoft_v1_microsoft_auth_callback_get**](MicrosoftApi.md#callback_microsoft_v1_microsoft_auth_callback_get) | **GET** /v1/microsoft/auth/callback | Callback Microsoft
[**create_microsoft_subscription_v1_microsoft_subscriptions_post**](MicrosoftApi.md#create_microsoft_subscription_v1_microsoft_subscriptions_post) | **POST** /v1/microsoft/subscriptions | Create Microsoft Subscription
[**delete_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_delete**](MicrosoftApi.md#delete_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_delete) | **DELETE** /v1/microsoft/subscriptions/{subscription_id} | Delete Microsoft Subscription
[**get_microsoft_calendar_v1_microsoft_calendar_get**](MicrosoftApi.md#get_microsoft_calendar_v1_microsoft_calendar_get) | **GET** /v1/microsoft/calendar | Get Microsoft Calendar
[**get_microsoft_profile_v1_microsoft_me_get**](MicrosoftApi.md#get_microsoft_profile_v1_microsoft_me_get) | **GET** /v1/microsoft/me | Get Microsoft Profile
[**get_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_get**](MicrosoftApi.md#get_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_get) | **GET** /v1/microsoft/subscriptions/{subscription_id} | Get Microsoft Subscription
[**list_microsoft_calendars_v1_microsoft_calendars_get**](MicrosoftApi.md#list_microsoft_calendars_v1_microsoft_calendars_get) | **GET** /v1/microsoft/calendars | List Microsoft Calendars
[**list_microsoft_events_v1_microsoft_calendar_events_get**](MicrosoftApi.md#list_microsoft_events_v1_microsoft_calendar_events_get) | **GET** /v1/microsoft/calendar/events | List Microsoft Events
[**list_microsoft_inbox_v1_microsoft_list_inbox_get**](MicrosoftApi.md#list_microsoft_inbox_v1_microsoft_list_inbox_get) | **GET** /v1/microsoft/list-inbox | List Microsoft Inbox
[**list_microsoft_subscriptions_v1_microsoft_subscriptions_get**](MicrosoftApi.md#list_microsoft_subscriptions_v1_microsoft_subscriptions_get) | **GET** /v1/microsoft/subscriptions | List Microsoft Subscriptions
[**login_microsoft_v1_microsoft_auth_login_get**](MicrosoftApi.md#login_microsoft_v1_microsoft_auth_login_get) | **GET** /v1/microsoft/auth/login | Login Microsoft
[**microsoft_calendar_webhook_v1_microsoft_webhook_calendar_notifications_org_id_user_id_calendar_id_post**](MicrosoftApi.md#microsoft_calendar_webhook_v1_microsoft_webhook_calendar_notifications_org_id_user_id_calendar_id_post) | **POST** /v1/microsoft/webhook/calendar/notifications/{org_id}/{user_id}/{calendar_id} | Microsoft Calendar Webhook
[**microsoft_webhook_v1_microsoft_webhook_notifications_org_id_user_id_post**](MicrosoftApi.md#microsoft_webhook_v1_microsoft_webhook_notifications_org_id_user_id_post) | **POST** /v1/microsoft/webhook/notifications/{org_id}/{user_id} | Microsoft Webhook
[**sync_microsoft_calendar_v1_microsoft_calendar_calendar_id_sync_post**](MicrosoftApi.md#sync_microsoft_calendar_v1_microsoft_calendar_calendar_id_sync_post) | **POST** /v1/microsoft/calendar/{calendar_id}/sync | Sync Microsoft Calendar
[**sync_microsoft_inbox_v1_microsoft_email_sync_post**](MicrosoftApi.md#sync_microsoft_inbox_v1_microsoft_email_sync_post) | **POST** /v1/microsoft/email/sync | Sync Microsoft Inbox
[**update_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_patch**](MicrosoftApi.md#update_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_patch) | **PATCH** /v1/microsoft/subscriptions/{subscription_id} | Update Microsoft Subscription
[**watch_microsoft_calendar_v1_microsoft_calendar_calendar_id_watch_post**](MicrosoftApi.md#watch_microsoft_calendar_v1_microsoft_calendar_calendar_id_watch_post) | **POST** /v1/microsoft/calendar/{calendar_id}/watch | Watch Microsoft Calendar
[**watch_microsoft_inbox_v1_microsoft_email_watch_post**](MicrosoftApi.md#watch_microsoft_inbox_v1_microsoft_email_watch_post) | **POST** /v1/microsoft/email/watch | Watch Microsoft Inbox


# **callback_microsoft_v1_microsoft_auth_callback_get**
> object callback_microsoft_v1_microsoft_auth_callback_get(code=code, state=state, error=error, error_description=error_description)

Callback Microsoft

Handles the callback from Microsoft.
Exchanges code for token and associates it with the correct user.

### Example


```python
import valstorm_api
from valstorm_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = valstorm_api.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with valstorm_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = valstorm_api.MicrosoftApi(api_client)
    code = 'code_example' # str |  (optional)
    state = 'state_example' # str |  (optional)
    error = 'error_example' # str |  (optional)
    error_description = 'error_description_example' # str |  (optional)

    try:
        # Callback Microsoft
        api_response = api_instance.callback_microsoft_v1_microsoft_auth_callback_get(code=code, state=state, error=error, error_description=error_description)
        print("The response of MicrosoftApi->callback_microsoft_v1_microsoft_auth_callback_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->callback_microsoft_v1_microsoft_auth_callback_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **str**|  | [optional] 
 **state** | **str**|  | [optional] 
 **error** | **str**|  | [optional] 
 **error_description** | **str**|  | [optional] 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_microsoft_subscription_v1_microsoft_subscriptions_post**
> object create_microsoft_subscription_v1_microsoft_subscriptions_post(create_subscription_request)

Create Microsoft Subscription

Creates a new Microsoft Graph subscription.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.create_subscription_request import CreateSubscriptionRequest
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
    api_instance = valstorm_api.MicrosoftApi(api_client)
    create_subscription_request = valstorm_api.CreateSubscriptionRequest() # CreateSubscriptionRequest | 

    try:
        # Create Microsoft Subscription
        api_response = api_instance.create_microsoft_subscription_v1_microsoft_subscriptions_post(create_subscription_request)
        print("The response of MicrosoftApi->create_microsoft_subscription_v1_microsoft_subscriptions_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->create_microsoft_subscription_v1_microsoft_subscriptions_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_subscription_request** | [**CreateSubscriptionRequest**](CreateSubscriptionRequest.md)|  | 

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
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_delete**
> object delete_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_delete(subscription_id)

Delete Microsoft Subscription

Deletes a specific Microsoft Graph subscription.

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
    api_instance = valstorm_api.MicrosoftApi(api_client)
    subscription_id = 'subscription_id_example' # str | 

    try:
        # Delete Microsoft Subscription
        api_response = api_instance.delete_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_delete(subscription_id)
        print("The response of MicrosoftApi->delete_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->delete_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_id** | **str**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_microsoft_calendar_v1_microsoft_calendar_get**
> object get_microsoft_calendar_v1_microsoft_calendar_get()

Get Microsoft Calendar

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
    api_instance = valstorm_api.MicrosoftApi(api_client)

    try:
        # Get Microsoft Calendar
        api_response = api_instance.get_microsoft_calendar_v1_microsoft_calendar_get()
        print("The response of MicrosoftApi->get_microsoft_calendar_v1_microsoft_calendar_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->get_microsoft_calendar_v1_microsoft_calendar_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_microsoft_profile_v1_microsoft_me_get**
> object get_microsoft_profile_v1_microsoft_me_get()

Get Microsoft Profile

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
    api_instance = valstorm_api.MicrosoftApi(api_client)

    try:
        # Get Microsoft Profile
        api_response = api_instance.get_microsoft_profile_v1_microsoft_me_get()
        print("The response of MicrosoftApi->get_microsoft_profile_v1_microsoft_me_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->get_microsoft_profile_v1_microsoft_me_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_get**
> object get_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_get(subscription_id)

Get Microsoft Subscription

Retrieves a specific Microsoft Graph subscription.

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
    api_instance = valstorm_api.MicrosoftApi(api_client)
    subscription_id = 'subscription_id_example' # str | 

    try:
        # Get Microsoft Subscription
        api_response = api_instance.get_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_get(subscription_id)
        print("The response of MicrosoftApi->get_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->get_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_id** | **str**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_microsoft_calendars_v1_microsoft_calendars_get**
> object list_microsoft_calendars_v1_microsoft_calendars_get()

List Microsoft Calendars

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
    api_instance = valstorm_api.MicrosoftApi(api_client)

    try:
        # List Microsoft Calendars
        api_response = api_instance.list_microsoft_calendars_v1_microsoft_calendars_get()
        print("The response of MicrosoftApi->list_microsoft_calendars_v1_microsoft_calendars_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->list_microsoft_calendars_v1_microsoft_calendars_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_microsoft_events_v1_microsoft_calendar_events_get**
> object list_microsoft_events_v1_microsoft_calendar_events_get(calendar_id=calendar_id)

List Microsoft Events

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
    api_instance = valstorm_api.MicrosoftApi(api_client)
    calendar_id = 'calendar_id_example' # str |  (optional)

    try:
        # List Microsoft Events
        api_response = api_instance.list_microsoft_events_v1_microsoft_calendar_events_get(calendar_id=calendar_id)
        print("The response of MicrosoftApi->list_microsoft_events_v1_microsoft_calendar_events_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->list_microsoft_events_v1_microsoft_calendar_events_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **calendar_id** | **str**|  | [optional] 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_microsoft_inbox_v1_microsoft_list_inbox_get**
> object list_microsoft_inbox_v1_microsoft_list_inbox_get()

List Microsoft Inbox

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
    api_instance = valstorm_api.MicrosoftApi(api_client)

    try:
        # List Microsoft Inbox
        api_response = api_instance.list_microsoft_inbox_v1_microsoft_list_inbox_get()
        print("The response of MicrosoftApi->list_microsoft_inbox_v1_microsoft_list_inbox_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->list_microsoft_inbox_v1_microsoft_list_inbox_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_microsoft_subscriptions_v1_microsoft_subscriptions_get**
> object list_microsoft_subscriptions_v1_microsoft_subscriptions_get()

List Microsoft Subscriptions

Lists all Microsoft Graph subscriptions for the user.

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
    api_instance = valstorm_api.MicrosoftApi(api_client)

    try:
        # List Microsoft Subscriptions
        api_response = api_instance.list_microsoft_subscriptions_v1_microsoft_subscriptions_get()
        print("The response of MicrosoftApi->list_microsoft_subscriptions_v1_microsoft_subscriptions_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->list_microsoft_subscriptions_v1_microsoft_subscriptions_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **login_microsoft_v1_microsoft_auth_login_get**
> object login_microsoft_v1_microsoft_auth_login_get()

Login Microsoft

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
    api_instance = valstorm_api.MicrosoftApi(api_client)

    try:
        # Login Microsoft
        api_response = api_instance.login_microsoft_v1_microsoft_auth_login_get()
        print("The response of MicrosoftApi->login_microsoft_v1_microsoft_auth_login_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->login_microsoft_v1_microsoft_auth_login_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **microsoft_calendar_webhook_v1_microsoft_webhook_calendar_notifications_org_id_user_id_calendar_id_post**
> object microsoft_calendar_webhook_v1_microsoft_webhook_calendar_notifications_org_id_user_id_calendar_id_post(org_id, user_id, calendar_id, validation_token=validation_token)

Microsoft Calendar Webhook

Public endpoint to receive Microsoft Graph webhook notifications for calendar events.

### Example


```python
import valstorm_api
from valstorm_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = valstorm_api.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with valstorm_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = valstorm_api.MicrosoftApi(api_client)
    org_id = 'org_id_example' # str | 
    user_id = 'user_id_example' # str | 
    calendar_id = 'calendar_id_example' # str | 
    validation_token = 'validation_token_example' # str |  (optional)

    try:
        # Microsoft Calendar Webhook
        api_response = api_instance.microsoft_calendar_webhook_v1_microsoft_webhook_calendar_notifications_org_id_user_id_calendar_id_post(org_id, user_id, calendar_id, validation_token=validation_token)
        print("The response of MicrosoftApi->microsoft_calendar_webhook_v1_microsoft_webhook_calendar_notifications_org_id_user_id_calendar_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->microsoft_calendar_webhook_v1_microsoft_webhook_calendar_notifications_org_id_user_id_calendar_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 
 **user_id** | **str**|  | 
 **calendar_id** | **str**|  | 
 **validation_token** | **str**|  | [optional] 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **microsoft_webhook_v1_microsoft_webhook_notifications_org_id_user_id_post**
> object microsoft_webhook_v1_microsoft_webhook_notifications_org_id_user_id_post(org_id, user_id, validation_token=validation_token)

Microsoft Webhook

Public endpoint to receive Microsoft Graph webhook notifications.

### Example


```python
import valstorm_api
from valstorm_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = valstorm_api.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with valstorm_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = valstorm_api.MicrosoftApi(api_client)
    org_id = 'org_id_example' # str | 
    user_id = 'user_id_example' # str | 
    validation_token = 'validation_token_example' # str |  (optional)

    try:
        # Microsoft Webhook
        api_response = api_instance.microsoft_webhook_v1_microsoft_webhook_notifications_org_id_user_id_post(org_id, user_id, validation_token=validation_token)
        print("The response of MicrosoftApi->microsoft_webhook_v1_microsoft_webhook_notifications_org_id_user_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->microsoft_webhook_v1_microsoft_webhook_notifications_org_id_user_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 
 **user_id** | **str**|  | 
 **validation_token** | **str**|  | [optional] 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sync_microsoft_calendar_v1_microsoft_calendar_calendar_id_sync_post**
> object sync_microsoft_calendar_v1_microsoft_calendar_calendar_id_sync_post(calendar_id)

Sync Microsoft Calendar

Triggers an initial full sync or a delta sync of the user's Outlook calendar.

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
    api_instance = valstorm_api.MicrosoftApi(api_client)
    calendar_id = 'calendar_id_example' # str | 

    try:
        # Sync Microsoft Calendar
        api_response = api_instance.sync_microsoft_calendar_v1_microsoft_calendar_calendar_id_sync_post(calendar_id)
        print("The response of MicrosoftApi->sync_microsoft_calendar_v1_microsoft_calendar_calendar_id_sync_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->sync_microsoft_calendar_v1_microsoft_calendar_calendar_id_sync_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **calendar_id** | **str**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sync_microsoft_inbox_v1_microsoft_email_sync_post**
> object sync_microsoft_inbox_v1_microsoft_email_sync_post()

Sync Microsoft Inbox

Triggers a sync of the user's Outlook inbox.
Performs a delta sync if a previous sync has been completed,
otherwise performs an initial full sync.

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
    api_instance = valstorm_api.MicrosoftApi(api_client)

    try:
        # Sync Microsoft Inbox
        api_response = api_instance.sync_microsoft_inbox_v1_microsoft_email_sync_post()
        print("The response of MicrosoftApi->sync_microsoft_inbox_v1_microsoft_email_sync_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->sync_microsoft_inbox_v1_microsoft_email_sync_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_patch**
> object update_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_patch(subscription_id, expiration_date_time)

Update Microsoft Subscription

Updates a specific Microsoft Graph subscription.

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
    api_instance = valstorm_api.MicrosoftApi(api_client)
    subscription_id = 'subscription_id_example' # str | 
    expiration_date_time = 'expiration_date_time_example' # str | 

    try:
        # Update Microsoft Subscription
        api_response = api_instance.update_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_patch(subscription_id, expiration_date_time)
        print("The response of MicrosoftApi->update_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->update_microsoft_subscription_v1_microsoft_subscriptions_subscription_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_id** | **str**|  | 
 **expiration_date_time** | **str**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **watch_microsoft_calendar_v1_microsoft_calendar_calendar_id_watch_post**
> object watch_microsoft_calendar_v1_microsoft_calendar_calendar_id_watch_post(calendar_id)

Watch Microsoft Calendar

Sets up a Microsoft Graph subscription (webhook) for real-time calendar notifications.

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
    api_instance = valstorm_api.MicrosoftApi(api_client)
    calendar_id = 'calendar_id_example' # str | 

    try:
        # Watch Microsoft Calendar
        api_response = api_instance.watch_microsoft_calendar_v1_microsoft_calendar_calendar_id_watch_post(calendar_id)
        print("The response of MicrosoftApi->watch_microsoft_calendar_v1_microsoft_calendar_calendar_id_watch_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->watch_microsoft_calendar_v1_microsoft_calendar_calendar_id_watch_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **calendar_id** | **str**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **watch_microsoft_inbox_v1_microsoft_email_watch_post**
> object watch_microsoft_inbox_v1_microsoft_email_watch_post()

Watch Microsoft Inbox

Sets up a Microsoft Graph subscription (webhook) for real-time email notifications.
https://learn.microsoft.com/en-us/graph/api/resources/subscription?view=graph-rest-1.0

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
    api_instance = valstorm_api.MicrosoftApi(api_client)

    try:
        # Watch Microsoft Inbox
        api_response = api_instance.watch_microsoft_inbox_v1_microsoft_email_watch_post()
        print("The response of MicrosoftApi->watch_microsoft_inbox_v1_microsoft_email_watch_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MicrosoftApi->watch_microsoft_inbox_v1_microsoft_email_watch_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


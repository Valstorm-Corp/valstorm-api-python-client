# valstorm_api.ServicesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_email_list_route_v1_email_provider_list_get**](ServicesApi.md#get_email_list_route_v1_email_provider_list_get) | **GET** /v1/email/{provider}/list | Get Email List Route
[**get_email_route_v1_email_provider_email_id_get**](ServicesApi.md#get_email_route_v1_email_provider_email_id_get) | **GET** /v1/email/{provider}/{email_id} | Get Email Route
[**get_hooks_v1_hooks_post**](ServicesApi.md#get_hooks_v1_hooks_post) | **POST** /v1/hooks | Get Hooks
[**initial_load_v1_load_get**](ServicesApi.md#initial_load_v1_load_get) | **GET** /v1/load | Initial Load
[**send_email_message_v1_email_google_provider_post**](ServicesApi.md#send_email_message_v1_email_google_provider_post) | **POST** /v1/email/google/{provider} | Send Email Message
[**send_email_route_v1_email_provider_post**](ServicesApi.md#send_email_route_v1_email_provider_post) | **POST** /v1/email/{provider} | Send Email Route
[**send_request_v1_request_post**](ServicesApi.md#send_request_v1_request_post) | **POST** /v1/request | Send Request


# **get_email_list_route_v1_email_provider_list_get**
> object get_email_list_route_v1_email_provider_list_get(provider)

Get Email List Route

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
    api_instance = valstorm_api.ServicesApi(api_client)
    provider = 'provider_example' # str | 

    try:
        # Get Email List Route
        api_response = api_instance.get_email_list_route_v1_email_provider_list_get(provider)
        print("The response of ServicesApi->get_email_list_route_v1_email_provider_list_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicesApi->get_email_list_route_v1_email_provider_list_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **provider** | **str**|  | 

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
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_email_route_v1_email_provider_email_id_get**
> object get_email_route_v1_email_provider_email_id_get(email_id, provider)

Get Email Route

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
    api_instance = valstorm_api.ServicesApi(api_client)
    email_id = 'email_id_example' # str | 
    provider = 'provider_example' # str | 

    try:
        # Get Email Route
        api_response = api_instance.get_email_route_v1_email_provider_email_id_get(email_id, provider)
        print("The response of ServicesApi->get_email_route_v1_email_provider_email_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicesApi->get_email_route_v1_email_provider_email_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_id** | **str**|  | 
 **provider** | **str**|  | 

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
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_hooks_v1_hooks_post**
> object get_hooks_v1_hooks_post()

Get Hooks

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
    api_instance = valstorm_api.ServicesApi(api_client)

    try:
        # Get Hooks
        api_response = api_instance.get_hooks_v1_hooks_post()
        print("The response of ServicesApi->get_hooks_v1_hooks_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicesApi->get_hooks_v1_hooks_post: %s\n" % e)
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
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **initial_load_v1_load_get**
> object initial_load_v1_load_get()

Initial Load

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
    api_instance = valstorm_api.ServicesApi(api_client)

    try:
        # Initial Load
        api_response = api_instance.initial_load_v1_load_get()
        print("The response of ServicesApi->initial_load_v1_load_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicesApi->initial_load_v1_load_get: %s\n" % e)
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
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_email_message_v1_email_google_provider_post**
> object send_email_message_v1_email_google_provider_post(provider, email_message)

Send Email Message

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.email_message import EmailMessage
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
    api_instance = valstorm_api.ServicesApi(api_client)
    provider = 'provider_example' # str | 
    email_message = valstorm_api.EmailMessage() # EmailMessage | 

    try:
        # Send Email Message
        api_response = api_instance.send_email_message_v1_email_google_provider_post(provider, email_message)
        print("The response of ServicesApi->send_email_message_v1_email_google_provider_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicesApi->send_email_message_v1_email_google_provider_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **provider** | **str**|  | 
 **email_message** | [**EmailMessage**](EmailMessage.md)|  | 

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

# **send_email_route_v1_email_provider_post**
> object send_email_route_v1_email_provider_post(provider, email_template)

Send Email Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.email_template import EmailTemplate
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
    api_instance = valstorm_api.ServicesApi(api_client)
    provider = 'provider_example' # str | 
    email_template = valstorm_api.EmailTemplate() # EmailTemplate | 

    try:
        # Send Email Route
        api_response = api_instance.send_email_route_v1_email_provider_post(provider, email_template)
        print("The response of ServicesApi->send_email_route_v1_email_provider_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicesApi->send_email_route_v1_email_provider_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **provider** | **str**|  | 
 **email_template** | [**EmailTemplate**](EmailTemplate.md)|  | 

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

# **send_request_v1_request_post**
> object send_request_v1_request_post(request_body)

Send Request

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
    api_instance = valstorm_api.ServicesApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Send Request
        api_response = api_instance.send_request_v1_request_post(request_body)
        print("The response of ServicesApi->send_request_v1_request_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicesApi->send_request_v1_request_post: %s\n" % e)
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


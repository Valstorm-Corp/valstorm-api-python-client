# valstorm_api.AiApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**chat_with_data_route_v1_ai_agent_chat_post**](AiApi.md#chat_with_data_route_v1_ai_agent_chat_post) | **POST** /v1/ai/agent/chat | Chat With Data Route
[**confirm_agent_tool_route_v1_ai_agent_confirm_post**](AiApi.md#confirm_agent_tool_route_v1_ai_agent_confirm_post) | **POST** /v1/ai/agent/confirm | Confirm Agent Tool Route
[**get_agent_tools_route_v1_ai_agent_agent_id_tools_get**](AiApi.md#get_agent_tools_route_v1_ai_agent_agent_id_tools_get) | **GET** /v1/ai/agent/{agent_id}/tools | Get Agent Tools Route
[**get_ai_tools_v1_ai_tools_get**](AiApi.md#get_ai_tools_v1_ai_tools_get) | **GET** /v1/ai/tools | Get Ai Tools


# **chat_with_data_route_v1_ai_agent_chat_post**
> object chat_with_data_route_v1_ai_agent_chat_post(chat_request)

Chat With Data Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.chat_request import ChatRequest
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
    api_instance = valstorm_api.AiApi(api_client)
    chat_request = valstorm_api.ChatRequest() # ChatRequest | 

    try:
        # Chat With Data Route
        api_response = api_instance.chat_with_data_route_v1_ai_agent_chat_post(chat_request)
        print("The response of AiApi->chat_with_data_route_v1_ai_agent_chat_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AiApi->chat_with_data_route_v1_ai_agent_chat_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **chat_request** | [**ChatRequest**](ChatRequest.md)|  | 

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

# **confirm_agent_tool_route_v1_ai_agent_confirm_post**
> object confirm_agent_tool_route_v1_ai_agent_confirm_post(confirm_tool_request)

Confirm Agent Tool Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.confirm_tool_request import ConfirmToolRequest
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
    api_instance = valstorm_api.AiApi(api_client)
    confirm_tool_request = valstorm_api.ConfirmToolRequest() # ConfirmToolRequest | 

    try:
        # Confirm Agent Tool Route
        api_response = api_instance.confirm_agent_tool_route_v1_ai_agent_confirm_post(confirm_tool_request)
        print("The response of AiApi->confirm_agent_tool_route_v1_ai_agent_confirm_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AiApi->confirm_agent_tool_route_v1_ai_agent_confirm_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **confirm_tool_request** | [**ConfirmToolRequest**](ConfirmToolRequest.md)|  | 

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

# **get_agent_tools_route_v1_ai_agent_agent_id_tools_get**
> object get_agent_tools_route_v1_ai_agent_agent_id_tools_get(agent_id)

Get Agent Tools Route

Returns the list of tools configured for a specific agent.

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
    api_instance = valstorm_api.AiApi(api_client)
    agent_id = 'agent_id_example' # str | 

    try:
        # Get Agent Tools Route
        api_response = api_instance.get_agent_tools_route_v1_ai_agent_agent_id_tools_get(agent_id)
        print("The response of AiApi->get_agent_tools_route_v1_ai_agent_agent_id_tools_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AiApi->get_agent_tools_route_v1_ai_agent_agent_id_tools_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **agent_id** | **str**|  | 

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

# **get_ai_tools_v1_ai_tools_get**
> object get_ai_tools_v1_ai_tools_get()

Get Ai Tools

Returns the list of all available platform tools that the AI can use.

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
    api_instance = valstorm_api.AiApi(api_client)

    try:
        # Get Ai Tools
        api_response = api_instance.get_ai_tools_v1_ai_tools_get()
        print("The response of AiApi->get_ai_tools_v1_ai_tools_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AiApi->get_ai_tools_v1_ai_tools_get: %s\n" % e)
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


# valstorm_api.TwilioMessageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_message_v1_twilio_message_post**](TwilioMessageApi.md#create_message_v1_twilio_message_post) | **POST** /v1/twilio/message | Create Message
[**get_message_v1_twilio_message_service_sid_conversation_sid_message_sid_get**](TwilioMessageApi.md#get_message_v1_twilio_message_service_sid_conversation_sid_message_sid_get) | **GET** /v1/twilio/message/{service_sid}/{conversation_sid}/{message_sid} | Get Message
[**get_messages_v1_twilio_message_service_sid_conversation_sid_get**](TwilioMessageApi.md#get_messages_v1_twilio_message_service_sid_conversation_sid_get) | **GET** /v1/twilio/message/{service_sid}/{conversation_sid} | Get Messages


# **create_message_v1_twilio_message_post**
> object create_message_v1_twilio_message_post(message)

Create Message

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.message import Message
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
    api_instance = valstorm_api.TwilioMessageApi(api_client)
    message = valstorm_api.Message() # Message | 

    try:
        # Create Message
        api_response = api_instance.create_message_v1_twilio_message_post(message)
        print("The response of TwilioMessageApi->create_message_v1_twilio_message_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioMessageApi->create_message_v1_twilio_message_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message** | [**Message**](Message.md)|  | 

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

# **get_message_v1_twilio_message_service_sid_conversation_sid_message_sid_get**
> object get_message_v1_twilio_message_service_sid_conversation_sid_message_sid_get(service_sid, conversation_sid, message_sid)

Get Message

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
    api_instance = valstorm_api.TwilioMessageApi(api_client)
    service_sid = 'service_sid_example' # str | 
    conversation_sid = 'conversation_sid_example' # str | 
    message_sid = 'message_sid_example' # str | 

    try:
        # Get Message
        api_response = api_instance.get_message_v1_twilio_message_service_sid_conversation_sid_message_sid_get(service_sid, conversation_sid, message_sid)
        print("The response of TwilioMessageApi->get_message_v1_twilio_message_service_sid_conversation_sid_message_sid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioMessageApi->get_message_v1_twilio_message_service_sid_conversation_sid_message_sid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_sid** | **str**|  | 
 **conversation_sid** | **str**|  | 
 **message_sid** | **str**|  | 

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

# **get_messages_v1_twilio_message_service_sid_conversation_sid_get**
> object get_messages_v1_twilio_message_service_sid_conversation_sid_get(service_sid, conversation_sid)

Get Messages

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
    api_instance = valstorm_api.TwilioMessageApi(api_client)
    service_sid = 'service_sid_example' # str | 
    conversation_sid = 'conversation_sid_example' # str | 

    try:
        # Get Messages
        api_response = api_instance.get_messages_v1_twilio_message_service_sid_conversation_sid_get(service_sid, conversation_sid)
        print("The response of TwilioMessageApi->get_messages_v1_twilio_message_service_sid_conversation_sid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioMessageApi->get_messages_v1_twilio_message_service_sid_conversation_sid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_sid** | **str**|  | 
 **conversation_sid** | **str**|  | 

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


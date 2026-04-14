# valstorm_api.TwilioConversationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_conversational_intelligence_service_resource_v1_twilio_conversational_intelligence_post**](TwilioConversationApi.md#create_conversational_intelligence_service_resource_v1_twilio_conversational_intelligence_post) | **POST** /v1/twilio/conversational-intelligence | Create Conversational Intelligence Service Resource
[**create_route_v1_twilio_conversation_post**](TwilioConversationApi.md#create_route_v1_twilio_conversation_post) | **POST** /v1/twilio/conversation | Create Route
[**create_route_v1_twilio_conversation_with_participants_post**](TwilioConversationApi.md#create_route_v1_twilio_conversation_with_participants_post) | **POST** /v1/twilio/conversation/with-participants | Create Route
[**create_transcription_v1_twilio_conversational_intelligence_transcribe_post**](TwilioConversationApi.md#create_transcription_v1_twilio_conversational_intelligence_transcribe_post) | **POST** /v1/twilio/conversational-intelligence/transcribe | Create Transcription
[**delete_conversation_route_v1_twilio_conversation_conversation_id_delete**](TwilioConversationApi.md#delete_conversation_route_v1_twilio_conversation_conversation_id_delete) | **DELETE** /v1/twilio/conversation/{conversation_id} | Delete Conversation Route
[**delete_service_conversation_route_v1_twilio_conversation_service_id_conversation_id_delete**](TwilioConversationApi.md#delete_service_conversation_route_v1_twilio_conversation_service_id_conversation_id_delete) | **DELETE** /v1/twilio/conversation/{service_id}/{conversation_id} | Delete Service Conversation Route
[**get_conversation_count_v1_twilio_conversation_count_get**](TwilioConversationApi.md#get_conversation_count_v1_twilio_conversation_count_get) | **GET** /v1/twilio/conversation/count | Get Conversation Count
[**get_conversation_page_v1_twilio_conversation_page_get**](TwilioConversationApi.md#get_conversation_page_v1_twilio_conversation_page_get) | **GET** /v1/twilio/conversation/page | Get Conversation Page
[**get_route_by_service_and_conversation_v1_twilio_conversation_service_id_conversation_id_get**](TwilioConversationApi.md#get_route_by_service_and_conversation_v1_twilio_conversation_service_id_conversation_id_get) | **GET** /v1/twilio/conversation/{service_id}/{conversation_id} | Get Route By Service And Conversation
[**get_route_v1_twilio_conversation_get**](TwilioConversationApi.md#get_route_v1_twilio_conversation_get) | **GET** /v1/twilio/conversation | Get Route
[**get_route_v1_twilio_conversation_service_id_get**](TwilioConversationApi.md#get_route_v1_twilio_conversation_service_id_get) | **GET** /v1/twilio/conversation/{service_id} | Get Route
[**get_transcription_sentences_v1_twilio_conversational_intelligence_transcription_sid_sentences_get**](TwilioConversationApi.md#get_transcription_sentences_v1_twilio_conversational_intelligence_transcription_sid_sentences_get) | **GET** /v1/twilio/conversational-intelligence/transcription/{sid}/sentences | Get Transcription Sentences
[**get_transcription_v1_twilio_conversational_intelligence_transcription_sid_get**](TwilioConversationApi.md#get_transcription_v1_twilio_conversational_intelligence_transcription_sid_get) | **GET** /v1/twilio/conversational-intelligence/transcription/{sid} | Get Transcription
[**token_route_v1_twilio_conversation_token_get**](TwilioConversationApi.md#token_route_v1_twilio_conversation_token_get) | **GET** /v1/twilio/conversation/token | Token Route
[**twilio_conversational_intelligence_webhook_v1_twilio_conversational_intelligence_webhook_organization_id_post**](TwilioConversationApi.md#twilio_conversational_intelligence_webhook_v1_twilio_conversational_intelligence_webhook_organization_id_post) | **POST** /v1/twilio/conversational-intelligence/webhook/{organization_id} | Twilio Conversational Intelligence Webhook
[**update_route_v1_twilio_conversation_service_id_conversation_id_put**](TwilioConversationApi.md#update_route_v1_twilio_conversation_service_id_conversation_id_put) | **PUT** /v1/twilio/conversation/{service_id}/{conversation_id} | Update Route


# **create_conversational_intelligence_service_resource_v1_twilio_conversational_intelligence_post**
> object create_conversational_intelligence_service_resource_v1_twilio_conversational_intelligence_post(create_service_request)

Create Conversational Intelligence Service Resource

Creates a new Twilio Conversational Intelligence Service.
https://www.twilio.com/docs/conversational-intelligence/api/service-resource

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.create_service_request import CreateServiceRequest
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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    create_service_request = valstorm_api.CreateServiceRequest() # CreateServiceRequest | 

    try:
        # Create Conversational Intelligence Service Resource
        api_response = api_instance.create_conversational_intelligence_service_resource_v1_twilio_conversational_intelligence_post(create_service_request)
        print("The response of TwilioConversationApi->create_conversational_intelligence_service_resource_v1_twilio_conversational_intelligence_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->create_conversational_intelligence_service_resource_v1_twilio_conversational_intelligence_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_service_request** | [**CreateServiceRequest**](CreateServiceRequest.md)|  | 

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

# **create_route_v1_twilio_conversation_post**
> object create_route_v1_twilio_conversation_post(conversation)

Create Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.conversation import Conversation
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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    conversation = valstorm_api.Conversation() # Conversation | 

    try:
        # Create Route
        api_response = api_instance.create_route_v1_twilio_conversation_post(conversation)
        print("The response of TwilioConversationApi->create_route_v1_twilio_conversation_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->create_route_v1_twilio_conversation_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversation** | [**Conversation**](Conversation.md)|  | 

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

# **create_route_v1_twilio_conversation_with_participants_post**
> object create_route_v1_twilio_conversation_with_participants_post(mms_conversation)

Create Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.mms_conversation import MmsConversation
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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    mms_conversation = valstorm_api.MmsConversation() # MmsConversation | 

    try:
        # Create Route
        api_response = api_instance.create_route_v1_twilio_conversation_with_participants_post(mms_conversation)
        print("The response of TwilioConversationApi->create_route_v1_twilio_conversation_with_participants_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->create_route_v1_twilio_conversation_with_participants_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mms_conversation** | [**MmsConversation**](MmsConversation.md)|  | 

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

# **create_transcription_v1_twilio_conversational_intelligence_transcribe_post**
> object create_transcription_v1_twilio_conversational_intelligence_transcribe_post(create_twilio_recording_transcription_request)

Create Transcription

Creates a new transcription for a given Twilio recording.
https://www.twilio.com/docs/conversational-intelligence/api/transcription-resource#create-a-transcription

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.create_twilio_recording_transcription_request import CreateTwilioRecordingTranscriptionRequest
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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    create_twilio_recording_transcription_request = valstorm_api.CreateTwilioRecordingTranscriptionRequest() # CreateTwilioRecordingTranscriptionRequest | 

    try:
        # Create Transcription
        api_response = api_instance.create_transcription_v1_twilio_conversational_intelligence_transcribe_post(create_twilio_recording_transcription_request)
        print("The response of TwilioConversationApi->create_transcription_v1_twilio_conversational_intelligence_transcribe_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->create_transcription_v1_twilio_conversational_intelligence_transcribe_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_twilio_recording_transcription_request** | [**CreateTwilioRecordingTranscriptionRequest**](CreateTwilioRecordingTranscriptionRequest.md)|  | 

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

# **delete_conversation_route_v1_twilio_conversation_conversation_id_delete**
> object delete_conversation_route_v1_twilio_conversation_conversation_id_delete(conversation_id)

Delete Conversation Route

Delete a conversation

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    conversation_id = 'conversation_id_example' # str | 

    try:
        # Delete Conversation Route
        api_response = api_instance.delete_conversation_route_v1_twilio_conversation_conversation_id_delete(conversation_id)
        print("The response of TwilioConversationApi->delete_conversation_route_v1_twilio_conversation_conversation_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->delete_conversation_route_v1_twilio_conversation_conversation_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversation_id** | **str**|  | 

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

# **delete_service_conversation_route_v1_twilio_conversation_service_id_conversation_id_delete**
> object delete_service_conversation_route_v1_twilio_conversation_service_id_conversation_id_delete(service_id, conversation_id)

Delete Service Conversation Route

Delete a conversation from a service

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    service_id = 'service_id_example' # str | 
    conversation_id = 'conversation_id_example' # str | 

    try:
        # Delete Service Conversation Route
        api_response = api_instance.delete_service_conversation_route_v1_twilio_conversation_service_id_conversation_id_delete(service_id, conversation_id)
        print("The response of TwilioConversationApi->delete_service_conversation_route_v1_twilio_conversation_service_id_conversation_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->delete_service_conversation_route_v1_twilio_conversation_service_id_conversation_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_id** | **str**|  | 
 **conversation_id** | **str**|  | 

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

# **get_conversation_count_v1_twilio_conversation_count_get**
> object get_conversation_count_v1_twilio_conversation_count_get(service_id)

Get Conversation Count

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    service_id = 'service_id_example' # str | 

    try:
        # Get Conversation Count
        api_response = api_instance.get_conversation_count_v1_twilio_conversation_count_get(service_id)
        print("The response of TwilioConversationApi->get_conversation_count_v1_twilio_conversation_count_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->get_conversation_count_v1_twilio_conversation_count_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_id** | **str**|  | 

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

# **get_conversation_page_v1_twilio_conversation_page_get**
> object get_conversation_page_v1_twilio_conversation_page_get(service_id, page_size=page_size, page_token=page_token)

Get Conversation Page

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    service_id = 'service_id_example' # str | 
    page_size = 50 # int |  (optional) (default to 50)
    page_token = 'page_token_example' # str |  (optional)

    try:
        # Get Conversation Page
        api_response = api_instance.get_conversation_page_v1_twilio_conversation_page_get(service_id, page_size=page_size, page_token=page_token)
        print("The response of TwilioConversationApi->get_conversation_page_v1_twilio_conversation_page_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->get_conversation_page_v1_twilio_conversation_page_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_id** | **str**|  | 
 **page_size** | **int**|  | [optional] [default to 50]
 **page_token** | **str**|  | [optional] 

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

# **get_route_by_service_and_conversation_v1_twilio_conversation_service_id_conversation_id_get**
> object get_route_by_service_and_conversation_v1_twilio_conversation_service_id_conversation_id_get(service_id, conversation_id)

Get Route By Service And Conversation

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    service_id = 'service_id_example' # str | 
    conversation_id = 'conversation_id_example' # str | 

    try:
        # Get Route By Service And Conversation
        api_response = api_instance.get_route_by_service_and_conversation_v1_twilio_conversation_service_id_conversation_id_get(service_id, conversation_id)
        print("The response of TwilioConversationApi->get_route_by_service_and_conversation_v1_twilio_conversation_service_id_conversation_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->get_route_by_service_and_conversation_v1_twilio_conversation_service_id_conversation_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_id** | **str**|  | 
 **conversation_id** | **str**|  | 

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

# **get_route_v1_twilio_conversation_get**
> object get_route_v1_twilio_conversation_get()

Get Route

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)

    try:
        # Get Route
        api_response = api_instance.get_route_v1_twilio_conversation_get()
        print("The response of TwilioConversationApi->get_route_v1_twilio_conversation_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->get_route_v1_twilio_conversation_get: %s\n" % e)
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

# **get_route_v1_twilio_conversation_service_id_get**
> object get_route_v1_twilio_conversation_service_id_get(service_id)

Get Route

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    service_id = 'service_id_example' # str | 

    try:
        # Get Route
        api_response = api_instance.get_route_v1_twilio_conversation_service_id_get(service_id)
        print("The response of TwilioConversationApi->get_route_v1_twilio_conversation_service_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->get_route_v1_twilio_conversation_service_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_id** | **str**|  | 

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

# **get_transcription_sentences_v1_twilio_conversational_intelligence_transcription_sid_sentences_get**
> object get_transcription_sentences_v1_twilio_conversational_intelligence_transcription_sid_sentences_get(sid)

Get Transcription Sentences

Retrieves a transcription by its SID.
https://www.twilio.com/docs/conversational-intelligence/api/transcription-resource#retrieve-a-transcription

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Get Transcription Sentences
        api_response = api_instance.get_transcription_sentences_v1_twilio_conversational_intelligence_transcription_sid_sentences_get(sid)
        print("The response of TwilioConversationApi->get_transcription_sentences_v1_twilio_conversational_intelligence_transcription_sid_sentences_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->get_transcription_sentences_v1_twilio_conversational_intelligence_transcription_sid_sentences_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **get_transcription_v1_twilio_conversational_intelligence_transcription_sid_get**
> object get_transcription_v1_twilio_conversational_intelligence_transcription_sid_get(sid)

Get Transcription

Retrieves a transcription by its SID.
https://www.twilio.com/docs/conversational-intelligence/api/transcription-resource#retrieve-a-transcription

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Get Transcription
        api_response = api_instance.get_transcription_v1_twilio_conversational_intelligence_transcription_sid_get(sid)
        print("The response of TwilioConversationApi->get_transcription_v1_twilio_conversational_intelligence_transcription_sid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->get_transcription_v1_twilio_conversational_intelligence_transcription_sid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **token_route_v1_twilio_conversation_token_get**
> object token_route_v1_twilio_conversation_token_get()

Token Route

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)

    try:
        # Token Route
        api_response = api_instance.token_route_v1_twilio_conversation_token_get()
        print("The response of TwilioConversationApi->token_route_v1_twilio_conversation_token_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->token_route_v1_twilio_conversation_token_get: %s\n" % e)
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

# **twilio_conversational_intelligence_webhook_v1_twilio_conversational_intelligence_webhook_organization_id_post**
> object twilio_conversational_intelligence_webhook_v1_twilio_conversational_intelligence_webhook_organization_id_post(organization_id)

Twilio Conversational Intelligence Webhook

Webhook endpoint to receive events from Twilio Conversational Intelligence.

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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    organization_id = 'organization_id_example' # str | 

    try:
        # Twilio Conversational Intelligence Webhook
        api_response = api_instance.twilio_conversational_intelligence_webhook_v1_twilio_conversational_intelligence_webhook_organization_id_post(organization_id)
        print("The response of TwilioConversationApi->twilio_conversational_intelligence_webhook_v1_twilio_conversational_intelligence_webhook_organization_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->twilio_conversational_intelligence_webhook_v1_twilio_conversational_intelligence_webhook_organization_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organization_id** | **str**|  | 

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
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_route_v1_twilio_conversation_service_id_conversation_id_put**
> object update_route_v1_twilio_conversation_service_id_conversation_id_put(service_id, conversation_id, conversate_state_change)

Update Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.conversate_state_change import ConversateStateChange
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
    api_instance = valstorm_api.TwilioConversationApi(api_client)
    service_id = 'service_id_example' # str | 
    conversation_id = 'conversation_id_example' # str | 
    conversate_state_change = valstorm_api.ConversateStateChange() # ConversateStateChange | 

    try:
        # Update Route
        api_response = api_instance.update_route_v1_twilio_conversation_service_id_conversation_id_put(service_id, conversation_id, conversate_state_change)
        print("The response of TwilioConversationApi->update_route_v1_twilio_conversation_service_id_conversation_id_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationApi->update_route_v1_twilio_conversation_service_id_conversation_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_id** | **str**|  | 
 **conversation_id** | **str**|  | 
 **conversate_state_change** | [**ConversateStateChange**](ConversateStateChange.md)|  | 

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


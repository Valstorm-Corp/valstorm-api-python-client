# valstorm_api.TwilioParticipantApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_route_v1_twilio_participant_post**](TwilioParticipantApi.md#create_route_v1_twilio_participant_post) | **POST** /v1/twilio/participant | Create Route
[**delete_route_v1_twilio_participant_conversation_id_participant_id_delete**](TwilioParticipantApi.md#delete_route_v1_twilio_participant_conversation_id_participant_id_delete) | **DELETE** /v1/twilio/participant/{conversation_id}/{participant_id} | Delete Route
[**get_participants_v1_twilio_participant_service_sid_conversation_id_get**](TwilioParticipantApi.md#get_participants_v1_twilio_participant_service_sid_conversation_id_get) | **GET** /v1/twilio/participant/{service_sid}/{conversation_id} | Get Participants
[**get_route_v1_twilio_participant_service_sid_conversation_id_participant_id_get**](TwilioParticipantApi.md#get_route_v1_twilio_participant_service_sid_conversation_id_participant_id_get) | **GET** /v1/twilio/participant/{service_sid}/{conversation_id}/{participant_id} | Get Route
[**service_delete_route_v1_twilio_participant_service_id_conversation_id_participant_id_delete**](TwilioParticipantApi.md#service_delete_route_v1_twilio_participant_service_id_conversation_id_participant_id_delete) | **DELETE** /v1/twilio/participant/{service_id}/{conversation_id}/{participant_id} | Service Delete Route


# **create_route_v1_twilio_participant_post**
> object create_route_v1_twilio_participant_post(create_participant)

Create Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.create_participant import CreateParticipant
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
    api_instance = valstorm_api.TwilioParticipantApi(api_client)
    create_participant = valstorm_api.CreateParticipant() # CreateParticipant | 

    try:
        # Create Route
        api_response = api_instance.create_route_v1_twilio_participant_post(create_participant)
        print("The response of TwilioParticipantApi->create_route_v1_twilio_participant_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioParticipantApi->create_route_v1_twilio_participant_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_participant** | [**CreateParticipant**](CreateParticipant.md)|  | 

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

# **delete_route_v1_twilio_participant_conversation_id_participant_id_delete**
> object delete_route_v1_twilio_participant_conversation_id_participant_id_delete(conversation_id, participant_id)

Delete Route

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
    api_instance = valstorm_api.TwilioParticipantApi(api_client)
    conversation_id = 'conversation_id_example' # str | 
    participant_id = 'participant_id_example' # str | 

    try:
        # Delete Route
        api_response = api_instance.delete_route_v1_twilio_participant_conversation_id_participant_id_delete(conversation_id, participant_id)
        print("The response of TwilioParticipantApi->delete_route_v1_twilio_participant_conversation_id_participant_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioParticipantApi->delete_route_v1_twilio_participant_conversation_id_participant_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversation_id** | **str**|  | 
 **participant_id** | **str**|  | 

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

# **get_participants_v1_twilio_participant_service_sid_conversation_id_get**
> object get_participants_v1_twilio_participant_service_sid_conversation_id_get(service_sid, conversation_id)

Get Participants

Description: Get all Twilio participants by conversation id
Args:
    service_sid (str): Twilio service id
    conversation_id (str): Twilio conversation id
    current_user (User, optional): Current user. Defaults to Depends(get_current_user).
Returns:
    JSONResponse: Twilio participants

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
    api_instance = valstorm_api.TwilioParticipantApi(api_client)
    service_sid = 'service_sid_example' # str | 
    conversation_id = 'conversation_id_example' # str | 

    try:
        # Get Participants
        api_response = api_instance.get_participants_v1_twilio_participant_service_sid_conversation_id_get(service_sid, conversation_id)
        print("The response of TwilioParticipantApi->get_participants_v1_twilio_participant_service_sid_conversation_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioParticipantApi->get_participants_v1_twilio_participant_service_sid_conversation_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_sid** | **str**|  | 
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

# **get_route_v1_twilio_participant_service_sid_conversation_id_participant_id_get**
> object get_route_v1_twilio_participant_service_sid_conversation_id_participant_id_get(service_sid, conversation_id, participant_id)

Get Route

Description: Get a Twilio participant by conversation id and participant id
Creates a new participant record if it does not exist in the database
Args:
    service_sid (str): Twilio service id
    conversation_id (str): Twilio conversation id
    participant_id (str): Twilio participant id
    background_task (BackgroundTasks): FastAPI background task
    current_user (User, optional): Current user. Defaults to Depends(get_current_user).
Returns:
    JSONResponse: Twilio participant record

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
    api_instance = valstorm_api.TwilioParticipantApi(api_client)
    service_sid = 'service_sid_example' # str | 
    conversation_id = 'conversation_id_example' # str | 
    participant_id = 'participant_id_example' # str | 

    try:
        # Get Route
        api_response = api_instance.get_route_v1_twilio_participant_service_sid_conversation_id_participant_id_get(service_sid, conversation_id, participant_id)
        print("The response of TwilioParticipantApi->get_route_v1_twilio_participant_service_sid_conversation_id_participant_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioParticipantApi->get_route_v1_twilio_participant_service_sid_conversation_id_participant_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_sid** | **str**|  | 
 **conversation_id** | **str**|  | 
 **participant_id** | **str**|  | 

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

# **service_delete_route_v1_twilio_participant_service_id_conversation_id_participant_id_delete**
> object service_delete_route_v1_twilio_participant_service_id_conversation_id_participant_id_delete(service_id, conversation_id, participant_id)

Service Delete Route

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
    api_instance = valstorm_api.TwilioParticipantApi(api_client)
    service_id = 'service_id_example' # str | 
    conversation_id = 'conversation_id_example' # str | 
    participant_id = 'participant_id_example' # str | 

    try:
        # Service Delete Route
        api_response = api_instance.service_delete_route_v1_twilio_participant_service_id_conversation_id_participant_id_delete(service_id, conversation_id, participant_id)
        print("The response of TwilioParticipantApi->service_delete_route_v1_twilio_participant_service_id_conversation_id_participant_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioParticipantApi->service_delete_route_v1_twilio_participant_service_id_conversation_id_participant_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_id** | **str**|  | 
 **conversation_id** | **str**|  | 
 **participant_id** | **str**|  | 

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


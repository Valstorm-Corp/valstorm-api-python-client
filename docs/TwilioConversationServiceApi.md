# valstorm_api.TwilioConversationServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_route_v1_twilio_service_get**](TwilioConversationServiceApi.md#get_route_v1_twilio_service_get) | **GET** /v1/twilio/service | Get Route
[**post_push_credential_v1_twilio_service_push_credential_post**](TwilioConversationServiceApi.md#post_push_credential_v1_twilio_service_push_credential_post) | **POST** /v1/twilio/service/push-credential | Post Push Credential
[**post_route_v1_twilio_service_post**](TwilioConversationServiceApi.md#post_route_v1_twilio_service_post) | **POST** /v1/twilio/service | Post Route


# **get_route_v1_twilio_service_get**
> object get_route_v1_twilio_service_get()

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
    api_instance = valstorm_api.TwilioConversationServiceApi(api_client)

    try:
        # Get Route
        api_response = api_instance.get_route_v1_twilio_service_get()
        print("The response of TwilioConversationServiceApi->get_route_v1_twilio_service_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationServiceApi->get_route_v1_twilio_service_get: %s\n" % e)
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

# **post_push_credential_v1_twilio_service_push_credential_post**
> object post_push_credential_v1_twilio_service_push_credential_post(push_credential)

Post Push Credential

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.push_credential import PushCredential
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
    api_instance = valstorm_api.TwilioConversationServiceApi(api_client)
    push_credential = valstorm_api.PushCredential() # PushCredential | 

    try:
        # Post Push Credential
        api_response = api_instance.post_push_credential_v1_twilio_service_push_credential_post(push_credential)
        print("The response of TwilioConversationServiceApi->post_push_credential_v1_twilio_service_push_credential_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationServiceApi->post_push_credential_v1_twilio_service_push_credential_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **push_credential** | [**PushCredential**](PushCredential.md)|  | 

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

# **post_route_v1_twilio_service_post**
> object post_route_v1_twilio_service_post(service)

Post Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.service import Service
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
    api_instance = valstorm_api.TwilioConversationServiceApi(api_client)
    service = valstorm_api.Service() # Service | 

    try:
        # Post Route
        api_response = api_instance.post_route_v1_twilio_service_post(service)
        print("The response of TwilioConversationServiceApi->post_route_v1_twilio_service_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationServiceApi->post_route_v1_twilio_service_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service** | [**Service**](Service.md)|  | 

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


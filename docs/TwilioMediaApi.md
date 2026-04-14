# valstorm_api.TwilioMediaApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**async_create_media_v1_twilio_media_service_sid_post**](TwilioMediaApi.md#async_create_media_v1_twilio_media_service_sid_post) | **POST** /v1/twilio/media/{service_sid} | Async Create Media
[**get_media_v1_twilio_media_service_sid_get**](TwilioMediaApi.md#get_media_v1_twilio_media_service_sid_get) | **GET** /v1/twilio/media/{service_sid} | Get Media
[**get_recording_v1_twilio_media_recording_sid_get**](TwilioMediaApi.md#get_recording_v1_twilio_media_recording_sid_get) | **GET** /v1/twilio/media/recording/{sid} | Get Recording


# **async_create_media_v1_twilio_media_service_sid_post**
> object async_create_media_v1_twilio_media_service_sid_post(service_sid, create_media_request)

Async Create Media

Creates a new media resource in Twilio by fetching an existing file from S3.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.create_media_request import CreateMediaRequest
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
    api_instance = valstorm_api.TwilioMediaApi(api_client)
    service_sid = 'service_sid_example' # str | 
    create_media_request = valstorm_api.CreateMediaRequest() # CreateMediaRequest | 

    try:
        # Async Create Media
        api_response = api_instance.async_create_media_v1_twilio_media_service_sid_post(service_sid, create_media_request)
        print("The response of TwilioMediaApi->async_create_media_v1_twilio_media_service_sid_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioMediaApi->async_create_media_v1_twilio_media_service_sid_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_sid** | **str**|  | 
 **create_media_request** | [**CreateMediaRequest**](CreateMediaRequest.md)|  | 

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

# **get_media_v1_twilio_media_service_sid_get**
> object get_media_v1_twilio_media_service_sid_get(service_sid, sids)

Get Media

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
    api_instance = valstorm_api.TwilioMediaApi(api_client)
    service_sid = 'service_sid_example' # str | 
    sids = 'sids_example' # str | 

    try:
        # Get Media
        api_response = api_instance.get_media_v1_twilio_media_service_sid_get(service_sid, sids)
        print("The response of TwilioMediaApi->get_media_v1_twilio_media_service_sid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioMediaApi->get_media_v1_twilio_media_service_sid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_sid** | **str**|  | 
 **sids** | **str**|  | 

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

# **get_recording_v1_twilio_media_recording_sid_get**
> object get_recording_v1_twilio_media_recording_sid_get(sid, media_type=media_type, ios=ios)

Get Recording

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
    api_instance = valstorm_api.TwilioMediaApi(api_client)
    sid = 'sid_example' # str | 
    media_type = 'mp3' # str |  (optional) (default to 'mp3')
    ios = 'false' # str |  (optional) (default to 'false')

    try:
        # Get Recording
        api_response = api_instance.get_recording_v1_twilio_media_recording_sid_get(sid, media_type=media_type, ios=ios)
        print("The response of TwilioMediaApi->get_recording_v1_twilio_media_recording_sid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioMediaApi->get_recording_v1_twilio_media_recording_sid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 
 **media_type** | **str**|  | [optional] [default to &#39;mp3&#39;]
 **ios** | **str**|  | [optional] [default to &#39;false&#39;]

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


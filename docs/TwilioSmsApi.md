# valstorm_api.TwilioSmsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_sms_route_v1_twilio_sms_sms_sid_get**](TwilioSmsApi.md#get_sms_route_v1_twilio_sms_sms_sid_get) | **GET** /v1/twilio/sms/{sms_sid} | Get Sms Route
[**send_sms_route_v1_twilio_sms_post**](TwilioSmsApi.md#send_sms_route_v1_twilio_sms_post) | **POST** /v1/twilio/sms | Send Sms Route
[**sms_callback_route_v1_twilio_sms_callback_org_id_post**](TwilioSmsApi.md#sms_callback_route_v1_twilio_sms_callback_org_id_post) | **POST** /v1/twilio/sms/callback/{org_id} | Sms Callback Route
[**sms_inbound_route_v1_twilio_sms_inbound_org_id_post**](TwilioSmsApi.md#sms_inbound_route_v1_twilio_sms_inbound_org_id_post) | **POST** /v1/twilio/sms/inbound/{org_id} | Sms Inbound Route


# **get_sms_route_v1_twilio_sms_sms_sid_get**
> object get_sms_route_v1_twilio_sms_sms_sid_get(sms_sid)

Get Sms Route

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
    api_instance = valstorm_api.TwilioSmsApi(api_client)
    sms_sid = 'sms_sid_example' # str | 

    try:
        # Get Sms Route
        api_response = api_instance.get_sms_route_v1_twilio_sms_sms_sid_get(sms_sid)
        print("The response of TwilioSmsApi->get_sms_route_v1_twilio_sms_sms_sid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioSmsApi->get_sms_route_v1_twilio_sms_sms_sid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sms_sid** | **str**|  | 

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

# **send_sms_route_v1_twilio_sms_post**
> object send_sms_route_v1_twilio_sms_post(data2)

Send Sms Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.data2 import Data2
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
    api_instance = valstorm_api.TwilioSmsApi(api_client)
    data2 = valstorm_api.Data2() # Data2 | 

    try:
        # Send Sms Route
        api_response = api_instance.send_sms_route_v1_twilio_sms_post(data2)
        print("The response of TwilioSmsApi->send_sms_route_v1_twilio_sms_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioSmsApi->send_sms_route_v1_twilio_sms_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data2** | [**Data2**](Data2.md)|  | 

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

# **sms_callback_route_v1_twilio_sms_callback_org_id_post**
> object sms_callback_route_v1_twilio_sms_callback_org_id_post(org_id)

Sms Callback Route

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
    api_instance = valstorm_api.TwilioSmsApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Sms Callback Route
        api_response = api_instance.sms_callback_route_v1_twilio_sms_callback_org_id_post(org_id)
        print("The response of TwilioSmsApi->sms_callback_route_v1_twilio_sms_callback_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioSmsApi->sms_callback_route_v1_twilio_sms_callback_org_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 

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

# **sms_inbound_route_v1_twilio_sms_inbound_org_id_post**
> object sms_inbound_route_v1_twilio_sms_inbound_org_id_post(org_id)

Sms Inbound Route

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
    api_instance = valstorm_api.TwilioSmsApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Sms Inbound Route
        api_response = api_instance.sms_inbound_route_v1_twilio_sms_inbound_org_id_post(org_id)
        print("The response of TwilioSmsApi->sms_inbound_route_v1_twilio_sms_inbound_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioSmsApi->sms_inbound_route_v1_twilio_sms_inbound_org_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 

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


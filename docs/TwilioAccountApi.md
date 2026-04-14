# valstorm_api.TwilioAccountApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_route_v1_twilio_account_application_get**](TwilioAccountApi.md#get_route_v1_twilio_account_application_get) | **GET** /v1/twilio/account/application | Get Route
[**patch_route_v1_twilio_account_application_patch**](TwilioAccountApi.md#patch_route_v1_twilio_account_application_patch) | **PATCH** /v1/twilio/account/application | Patch Route
[**post_route_v1_twilio_account_application_post**](TwilioAccountApi.md#post_route_v1_twilio_account_application_post) | **POST** /v1/twilio/account/application | Post Route
[**post_subaccount_route_v1_twilio_account_subaccount_post**](TwilioAccountApi.md#post_subaccount_route_v1_twilio_account_subaccount_post) | **POST** /v1/twilio/account/subaccount | Post Subaccount Route


# **get_route_v1_twilio_account_application_get**
> object get_route_v1_twilio_account_application_get()

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
    api_instance = valstorm_api.TwilioAccountApi(api_client)

    try:
        # Get Route
        api_response = api_instance.get_route_v1_twilio_account_application_get()
        print("The response of TwilioAccountApi->get_route_v1_twilio_account_application_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioAccountApi->get_route_v1_twilio_account_application_get: %s\n" % e)
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

# **patch_route_v1_twilio_account_application_patch**
> object patch_route_v1_twilio_account_application_patch(twiml_application_update)

Patch Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.twiml_application_update import TwimlApplicationUpdate
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
    api_instance = valstorm_api.TwilioAccountApi(api_client)
    twiml_application_update = valstorm_api.TwimlApplicationUpdate() # TwimlApplicationUpdate | 

    try:
        # Patch Route
        api_response = api_instance.patch_route_v1_twilio_account_application_patch(twiml_application_update)
        print("The response of TwilioAccountApi->patch_route_v1_twilio_account_application_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioAccountApi->patch_route_v1_twilio_account_application_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **twiml_application_update** | [**TwimlApplicationUpdate**](TwimlApplicationUpdate.md)|  | 

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

# **post_route_v1_twilio_account_application_post**
> object post_route_v1_twilio_account_application_post(twiml_application)

Post Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.twiml_application import TwimlApplication
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
    api_instance = valstorm_api.TwilioAccountApi(api_client)
    twiml_application = valstorm_api.TwimlApplication() # TwimlApplication | 

    try:
        # Post Route
        api_response = api_instance.post_route_v1_twilio_account_application_post(twiml_application)
        print("The response of TwilioAccountApi->post_route_v1_twilio_account_application_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioAccountApi->post_route_v1_twilio_account_application_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **twiml_application** | [**TwimlApplication**](TwimlApplication.md)|  | 

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

# **post_subaccount_route_v1_twilio_account_subaccount_post**
> object post_subaccount_route_v1_twilio_account_subaccount_post()

Post Subaccount Route

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
    api_instance = valstorm_api.TwilioAccountApi(api_client)

    try:
        # Post Subaccount Route
        api_response = api_instance.post_subaccount_route_v1_twilio_account_subaccount_post()
        print("The response of TwilioAccountApi->post_subaccount_route_v1_twilio_account_subaccount_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioAccountApi->post_subaccount_route_v1_twilio_account_subaccount_post: %s\n" % e)
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


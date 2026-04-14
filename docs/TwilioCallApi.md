# valstorm_api.TwilioCallApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**available_route_v1_twilio_call_available_post**](TwilioCallApi.md#available_route_v1_twilio_call_available_post) | **POST** /v1/twilio/call/available | Available Route
[**call_callback_route_v1_twilio_call_callback_org_id_post**](TwilioCallApi.md#call_callback_route_v1_twilio_call_callback_org_id_post) | **POST** /v1/twilio/call/callback/{org_id} | Call Callback Route
[**call_route_v1_twilio_call_fetch_call_id_get**](TwilioCallApi.md#call_route_v1_twilio_call_fetch_call_id_get) | **GET** /v1/twilio/call/fetch/{call_id} | Call Route
[**client_route_v1_twilio_call_client_user_id_post**](TwilioCallApi.md#client_route_v1_twilio_call_client_user_id_post) | **POST** /v1/twilio/call/client/{user_id} | Client Route
[**conference_callback_v1_twilio_call_conference_callback_org_id_post**](TwilioCallApi.md#conference_callback_v1_twilio_call_conference_callback_org_id_post) | **POST** /v1/twilio/call/conference-callback/{org_id} | Conference Callback
[**force_voicemail_route_v1_twilio_call_voicemail_force_org_id_post**](TwilioCallApi.md#force_voicemail_route_v1_twilio_call_voicemail_force_org_id_post) | **POST** /v1/twilio/call/voicemail/force/{org_id} | Force Voicemail Route
[**handle_inbound_call_route_test_v1_twilio_call_org_id_test_post**](TwilioCallApi.md#handle_inbound_call_route_test_v1_twilio_call_org_id_test_post) | **POST** /v1/twilio/call/{org_id}/test | Handle Inbound Call Route Test
[**lookup_route_v1_twilio_call_lookup_get**](TwilioCallApi.md#lookup_route_v1_twilio_call_lookup_get) | **GET** /v1/twilio/call/lookup | Lookup Route
[**platform_token_route_v1_twilio_call_token_platform_get**](TwilioCallApi.md#platform_token_route_v1_twilio_call_token_platform_get) | **GET** /v1/twilio/call/token/{platform} | Platform Token Route
[**post_call_route_v1_twilio_call_org_id_post**](TwilioCallApi.md#post_call_route_v1_twilio_call_org_id_post) | **POST** /v1/twilio/call/{org_id} | Post Call Route
[**post_voicemail_route_v1_twilio_call_voicemail_org_id_post**](TwilioCallApi.md#post_voicemail_route_v1_twilio_call_voicemail_org_id_post) | **POST** /v1/twilio/call/voicemail/{org_id} | Post Voicemail Route
[**recording_callback_route_v1_twilio_call_recording_callback_org_id_post**](TwilioCallApi.md#recording_callback_route_v1_twilio_call_recording_callback_org_id_post) | **POST** /v1/twilio/call/recording/callback/{org_id} | Recording Callback Route
[**recording_route_v1_twilio_call_recording_recording_id_get**](TwilioCallApi.md#recording_route_v1_twilio_call_recording_recording_id_get) | **GET** /v1/twilio/call/recording/{recording_id} | Recording Route
[**salesforce_click_to_dial_v1_twilio_call_salesforce_click_to_dial_post**](TwilioCallApi.md#salesforce_click_to_dial_v1_twilio_call_salesforce_click_to_dial_post) | **POST** /v1/twilio/call/salesforce-click-to-dial | Salesforce Click To Dial
[**salesforce_sucks_route_v1_twilio_call_salesforce_navigate_to_record_post**](TwilioCallApi.md#salesforce_sucks_route_v1_twilio_call_salesforce_navigate_to_record_post) | **POST** /v1/twilio/call/salesforce-navigate-to-record | Salesforce Sucks Route
[**save_client_call_route_v1_twilio_call_save_client_call_sid_post**](TwilioCallApi.md#save_client_call_route_v1_twilio_call_save_client_call_sid_post) | **POST** /v1/twilio/call/save-client-call/{sid} | Save Client Call Route
[**studio_route_v1_twilio_call_studio_org_id_post**](TwilioCallApi.md#studio_route_v1_twilio_call_studio_org_id_post) | **POST** /v1/twilio/call/studio/{org_id} | Studio Route
[**token_route_v1_twilio_call_token_get**](TwilioCallApi.md#token_route_v1_twilio_call_token_get) | **GET** /v1/twilio/call/token | Token Route
[**update_call_route_v1_twilio_call_patch**](TwilioCallApi.md#update_call_route_v1_twilio_call_patch) | **PATCH** /v1/twilio/call | Update Call Route
[**update_call_route_v1_twilio_call_update_sid_post**](TwilioCallApi.md#update_call_route_v1_twilio_call_update_sid_post) | **POST** /v1/twilio/call/update/{sid} | Update Call Route
[**voicemail_callback_route_v1_twilio_call_voicemail_callback_org_id_post**](TwilioCallApi.md#voicemail_callback_route_v1_twilio_call_voicemail_callback_org_id_post) | **POST** /v1/twilio/call/voicemail/callback/{org_id} | Voicemail Callback Route
[**voicemail_recording_callback_route_v1_twilio_call_voicemail_recording_org_id_post**](TwilioCallApi.md#voicemail_recording_callback_route_v1_twilio_call_voicemail_recording_org_id_post) | **POST** /v1/twilio/call/voicemail/recording/{org_id} | Voicemail Recording Callback Route
[**voicemail_start_route_v1_twilio_call_voicemail_start_org_id_post**](TwilioCallApi.md#voicemail_start_route_v1_twilio_call_voicemail_start_org_id_post) | **POST** /v1/twilio/call/voicemail/start/{org_id} | Voicemail Start Route


# **available_route_v1_twilio_call_available_post**
> object available_route_v1_twilio_call_available_post(twilio_routes_twilio_call_available)

Available Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.twilio_routes_twilio_call_available import TwilioRoutesTwilioCallAvailable
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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    twilio_routes_twilio_call_available = valstorm_api.TwilioRoutesTwilioCallAvailable() # TwilioRoutesTwilioCallAvailable | 

    try:
        # Available Route
        api_response = api_instance.available_route_v1_twilio_call_available_post(twilio_routes_twilio_call_available)
        print("The response of TwilioCallApi->available_route_v1_twilio_call_available_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->available_route_v1_twilio_call_available_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **twilio_routes_twilio_call_available** | [**TwilioRoutesTwilioCallAvailable**](TwilioRoutesTwilioCallAvailable.md)|  | 

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

# **call_callback_route_v1_twilio_call_callback_org_id_post**
> object call_callback_route_v1_twilio_call_callback_org_id_post(org_id)

Call Callback Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Call Callback Route
        api_response = api_instance.call_callback_route_v1_twilio_call_callback_org_id_post(org_id)
        print("The response of TwilioCallApi->call_callback_route_v1_twilio_call_callback_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->call_callback_route_v1_twilio_call_callback_org_id_post: %s\n" % e)
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

# **call_route_v1_twilio_call_fetch_call_id_get**
> object call_route_v1_twilio_call_fetch_call_id_get(call_id)

Call Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    call_id = 'call_id_example' # str | 

    try:
        # Call Route
        api_response = api_instance.call_route_v1_twilio_call_fetch_call_id_get(call_id)
        print("The response of TwilioCallApi->call_route_v1_twilio_call_fetch_call_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->call_route_v1_twilio_call_fetch_call_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **call_id** | **str**|  | 

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

# **client_route_v1_twilio_call_client_user_id_post**
> object client_route_v1_twilio_call_client_user_id_post(user_id, client_call_data)

Client Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.client_call_data import ClientCallData
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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    user_id = 'user_id_example' # str | 
    client_call_data = valstorm_api.ClientCallData() # ClientCallData | 

    try:
        # Client Route
        api_response = api_instance.client_route_v1_twilio_call_client_user_id_post(user_id, client_call_data)
        print("The response of TwilioCallApi->client_route_v1_twilio_call_client_user_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->client_route_v1_twilio_call_client_user_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**|  | 
 **client_call_data** | [**ClientCallData**](ClientCallData.md)|  | 

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

# **conference_callback_v1_twilio_call_conference_callback_org_id_post**
> conference_callback_v1_twilio_call_conference_callback_org_id_post(org_id)

Conference Callback

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Conference Callback
        api_instance.conference_callback_v1_twilio_call_conference_callback_org_id_post(org_id)
    except Exception as e:
        print("Exception when calling TwilioCallApi->conference_callback_v1_twilio_call_conference_callback_org_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **force_voicemail_route_v1_twilio_call_voicemail_force_org_id_post**
> object force_voicemail_route_v1_twilio_call_voicemail_force_org_id_post(org_id)

Force Voicemail Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Force Voicemail Route
        api_response = api_instance.force_voicemail_route_v1_twilio_call_voicemail_force_org_id_post(org_id)
        print("The response of TwilioCallApi->force_voicemail_route_v1_twilio_call_voicemail_force_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->force_voicemail_route_v1_twilio_call_voicemail_force_org_id_post: %s\n" % e)
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

# **handle_inbound_call_route_test_v1_twilio_call_org_id_test_post**
> object handle_inbound_call_route_test_v1_twilio_call_org_id_test_post(org_id)

Handle Inbound Call Route Test

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Handle Inbound Call Route Test
        api_response = api_instance.handle_inbound_call_route_test_v1_twilio_call_org_id_test_post(org_id)
        print("The response of TwilioCallApi->handle_inbound_call_route_test_v1_twilio_call_org_id_test_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->handle_inbound_call_route_test_v1_twilio_call_org_id_test_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 

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

# **lookup_route_v1_twilio_call_lookup_get**
> object lookup_route_v1_twilio_call_lookup_get(phone_number)

Lookup Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    phone_number = 'phone_number_example' # str | 

    try:
        # Lookup Route
        api_response = api_instance.lookup_route_v1_twilio_call_lookup_get(phone_number)
        print("The response of TwilioCallApi->lookup_route_v1_twilio_call_lookup_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->lookup_route_v1_twilio_call_lookup_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **phone_number** | **str**|  | 

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

# **platform_token_route_v1_twilio_call_token_platform_get**
> object platform_token_route_v1_twilio_call_token_platform_get(platform)

Platform Token Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    platform = 'platform_example' # str | 

    try:
        # Platform Token Route
        api_response = api_instance.platform_token_route_v1_twilio_call_token_platform_get(platform)
        print("The response of TwilioCallApi->platform_token_route_v1_twilio_call_token_platform_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->platform_token_route_v1_twilio_call_token_platform_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **platform** | **str**|  | 

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

# **post_call_route_v1_twilio_call_org_id_post**
> object post_call_route_v1_twilio_call_org_id_post(org_id)

Post Call Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Post Call Route
        api_response = api_instance.post_call_route_v1_twilio_call_org_id_post(org_id)
        print("The response of TwilioCallApi->post_call_route_v1_twilio_call_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->post_call_route_v1_twilio_call_org_id_post: %s\n" % e)
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

# **post_voicemail_route_v1_twilio_call_voicemail_org_id_post**
> object post_voicemail_route_v1_twilio_call_voicemail_org_id_post(org_id)

Post Voicemail Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Post Voicemail Route
        api_response = api_instance.post_voicemail_route_v1_twilio_call_voicemail_org_id_post(org_id)
        print("The response of TwilioCallApi->post_voicemail_route_v1_twilio_call_voicemail_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->post_voicemail_route_v1_twilio_call_voicemail_org_id_post: %s\n" % e)
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

# **recording_callback_route_v1_twilio_call_recording_callback_org_id_post**
> object recording_callback_route_v1_twilio_call_recording_callback_org_id_post(org_id)

Recording Callback Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Recording Callback Route
        api_response = api_instance.recording_callback_route_v1_twilio_call_recording_callback_org_id_post(org_id)
        print("The response of TwilioCallApi->recording_callback_route_v1_twilio_call_recording_callback_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->recording_callback_route_v1_twilio_call_recording_callback_org_id_post: %s\n" % e)
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

# **recording_route_v1_twilio_call_recording_recording_id_get**
> object recording_route_v1_twilio_call_recording_recording_id_get(recording_id)

Recording Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    recording_id = 'recording_id_example' # str | 

    try:
        # Recording Route
        api_response = api_instance.recording_route_v1_twilio_call_recording_recording_id_get(recording_id)
        print("The response of TwilioCallApi->recording_route_v1_twilio_call_recording_recording_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->recording_route_v1_twilio_call_recording_recording_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **recording_id** | **str**|  | 

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

# **salesforce_click_to_dial_v1_twilio_call_salesforce_click_to_dial_post**
> object salesforce_click_to_dial_v1_twilio_call_salesforce_click_to_dial_post(request_body)

Salesforce Click To Dial

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Salesforce Click To Dial
        api_response = api_instance.salesforce_click_to_dial_v1_twilio_call_salesforce_click_to_dial_post(request_body)
        print("The response of TwilioCallApi->salesforce_click_to_dial_v1_twilio_call_salesforce_click_to_dial_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->salesforce_click_to_dial_v1_twilio_call_salesforce_click_to_dial_post: %s\n" % e)
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
**202** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **salesforce_sucks_route_v1_twilio_call_salesforce_navigate_to_record_post**
> object salesforce_sucks_route_v1_twilio_call_salesforce_navigate_to_record_post(salesforce_navigate_to_record)

Salesforce Sucks Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.salesforce_navigate_to_record import SalesforceNavigateToRecord
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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    salesforce_navigate_to_record = valstorm_api.SalesforceNavigateToRecord() # SalesforceNavigateToRecord | 

    try:
        # Salesforce Sucks Route
        api_response = api_instance.salesforce_sucks_route_v1_twilio_call_salesforce_navigate_to_record_post(salesforce_navigate_to_record)
        print("The response of TwilioCallApi->salesforce_sucks_route_v1_twilio_call_salesforce_navigate_to_record_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->salesforce_sucks_route_v1_twilio_call_salesforce_navigate_to_record_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **salesforce_navigate_to_record** | [**SalesforceNavigateToRecord**](SalesforceNavigateToRecord.md)|  | 

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

# **save_client_call_route_v1_twilio_call_save_client_call_sid_post**
> object save_client_call_route_v1_twilio_call_save_client_call_sid_post(sid, twilio_save_client_call)

Save Client Call Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.twilio_save_client_call import TwilioSaveClientCall
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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    sid = 'sid_example' # str | 
    twilio_save_client_call = valstorm_api.TwilioSaveClientCall() # TwilioSaveClientCall | 

    try:
        # Save Client Call Route
        api_response = api_instance.save_client_call_route_v1_twilio_call_save_client_call_sid_post(sid, twilio_save_client_call)
        print("The response of TwilioCallApi->save_client_call_route_v1_twilio_call_save_client_call_sid_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->save_client_call_route_v1_twilio_call_save_client_call_sid_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 
 **twilio_save_client_call** | [**TwilioSaveClientCall**](TwilioSaveClientCall.md)|  | 

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

# **studio_route_v1_twilio_call_studio_org_id_post**
> object studio_route_v1_twilio_call_studio_org_id_post(org_id)

Studio Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Studio Route
        api_response = api_instance.studio_route_v1_twilio_call_studio_org_id_post(org_id)
        print("The response of TwilioCallApi->studio_route_v1_twilio_call_studio_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->studio_route_v1_twilio_call_studio_org_id_post: %s\n" % e)
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

# **token_route_v1_twilio_call_token_get**
> object token_route_v1_twilio_call_token_get()

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
    api_instance = valstorm_api.TwilioCallApi(api_client)

    try:
        # Token Route
        api_response = api_instance.token_route_v1_twilio_call_token_get()
        print("The response of TwilioCallApi->token_route_v1_twilio_call_token_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->token_route_v1_twilio_call_token_get: %s\n" % e)
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

# **update_call_route_v1_twilio_call_patch**
> object update_call_route_v1_twilio_call_patch()

Update Call Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)

    try:
        # Update Call Route
        api_response = api_instance.update_call_route_v1_twilio_call_patch()
        print("The response of TwilioCallApi->update_call_route_v1_twilio_call_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->update_call_route_v1_twilio_call_patch: %s\n" % e)
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

# **update_call_route_v1_twilio_call_update_sid_post**
> object update_call_route_v1_twilio_call_update_sid_post(sid, request_body)

Update Call Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    sid = 'sid_example' # str | 
    request_body = None # Dict[str, object] | 

    try:
        # Update Call Route
        api_response = api_instance.update_call_route_v1_twilio_call_update_sid_post(sid, request_body)
        print("The response of TwilioCallApi->update_call_route_v1_twilio_call_update_sid_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->update_call_route_v1_twilio_call_update_sid_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 
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

# **voicemail_callback_route_v1_twilio_call_voicemail_callback_org_id_post**
> object voicemail_callback_route_v1_twilio_call_voicemail_callback_org_id_post(org_id)

Voicemail Callback Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Voicemail Callback Route
        api_response = api_instance.voicemail_callback_route_v1_twilio_call_voicemail_callback_org_id_post(org_id)
        print("The response of TwilioCallApi->voicemail_callback_route_v1_twilio_call_voicemail_callback_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->voicemail_callback_route_v1_twilio_call_voicemail_callback_org_id_post: %s\n" % e)
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

# **voicemail_recording_callback_route_v1_twilio_call_voicemail_recording_org_id_post**
> object voicemail_recording_callback_route_v1_twilio_call_voicemail_recording_org_id_post(org_id)

Voicemail Recording Callback Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Voicemail Recording Callback Route
        api_response = api_instance.voicemail_recording_callback_route_v1_twilio_call_voicemail_recording_org_id_post(org_id)
        print("The response of TwilioCallApi->voicemail_recording_callback_route_v1_twilio_call_voicemail_recording_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->voicemail_recording_callback_route_v1_twilio_call_voicemail_recording_org_id_post: %s\n" % e)
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

# **voicemail_start_route_v1_twilio_call_voicemail_start_org_id_post**
> object voicemail_start_route_v1_twilio_call_voicemail_start_org_id_post(org_id)

Voicemail Start Route

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
    api_instance = valstorm_api.TwilioCallApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Voicemail Start Route
        api_response = api_instance.voicemail_start_route_v1_twilio_call_voicemail_start_org_id_post(org_id)
        print("The response of TwilioCallApi->voicemail_start_route_v1_twilio_call_voicemail_start_org_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioCallApi->voicemail_start_route_v1_twilio_call_voicemail_start_org_id_post: %s\n" % e)
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


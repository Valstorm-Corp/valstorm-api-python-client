# valstorm_api.TwilioPhoneApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_phone_address_v1_twilio_phone_address_service_sid_post**](TwilioPhoneApi.md#create_phone_address_v1_twilio_phone_address_service_sid_post) | **POST** /v1/twilio/phone/address/{service_sid} | Create Phone Address
[**find_phone_address_v1_twilio_phone_search_get**](TwilioPhoneApi.md#find_phone_address_v1_twilio_phone_search_get) | **GET** /v1/twilio/phone/search | Find Phone Address
[**get_route_v1_twilio_phone_get**](TwilioPhoneApi.md#get_route_v1_twilio_phone_get) | **GET** /v1/twilio/phone | Get Route
[**lookup_route_v1_twilio_phone_lookup_get**](TwilioPhoneApi.md#lookup_route_v1_twilio_phone_lookup_get) | **GET** /v1/twilio/phone/lookup | Lookup Route
[**patch_route_v1_twilio_phone_patch**](TwilioPhoneApi.md#patch_route_v1_twilio_phone_patch) | **PATCH** /v1/twilio/phone | Patch Route
[**purchase_phone_address_v1_twilio_phone_purchase_post**](TwilioPhoneApi.md#purchase_phone_address_v1_twilio_phone_purchase_post) | **POST** /v1/twilio/phone/purchase | Purchase Phone Address


# **create_phone_address_v1_twilio_phone_address_service_sid_post**
> CreatePhoneResponse create_phone_address_v1_twilio_phone_address_service_sid_post(service_sid, phone_address_config)

Create Phone Address

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.create_phone_response import CreatePhoneResponse
from valstorm_api.models.phone_address_config import PhoneAddressConfig
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
    api_instance = valstorm_api.TwilioPhoneApi(api_client)
    service_sid = 'service_sid_example' # str | 
    phone_address_config = valstorm_api.PhoneAddressConfig() # PhoneAddressConfig | 

    try:
        # Create Phone Address
        api_response = api_instance.create_phone_address_v1_twilio_phone_address_service_sid_post(service_sid, phone_address_config)
        print("The response of TwilioPhoneApi->create_phone_address_v1_twilio_phone_address_service_sid_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioPhoneApi->create_phone_address_v1_twilio_phone_address_service_sid_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **service_sid** | **str**|  | 
 **phone_address_config** | [**PhoneAddressConfig**](PhoneAddressConfig.md)|  | 

### Return type

[**CreatePhoneResponse**](CreatePhoneResponse.md)

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

# **find_phone_address_v1_twilio_phone_search_get**
> object find_phone_address_v1_twilio_phone_search_get()

Find Phone Address

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
    api_instance = valstorm_api.TwilioPhoneApi(api_client)

    try:
        # Find Phone Address
        api_response = api_instance.find_phone_address_v1_twilio_phone_search_get()
        print("The response of TwilioPhoneApi->find_phone_address_v1_twilio_phone_search_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioPhoneApi->find_phone_address_v1_twilio_phone_search_get: %s\n" % e)
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

# **get_route_v1_twilio_phone_get**
> object get_route_v1_twilio_phone_get()

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
    api_instance = valstorm_api.TwilioPhoneApi(api_client)

    try:
        # Get Route
        api_response = api_instance.get_route_v1_twilio_phone_get()
        print("The response of TwilioPhoneApi->get_route_v1_twilio_phone_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioPhoneApi->get_route_v1_twilio_phone_get: %s\n" % e)
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

# **lookup_route_v1_twilio_phone_lookup_get**
> object lookup_route_v1_twilio_phone_lookup_get(phone_number)

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
    api_instance = valstorm_api.TwilioPhoneApi(api_client)
    phone_number = 'phone_number_example' # str | 

    try:
        # Lookup Route
        api_response = api_instance.lookup_route_v1_twilio_phone_lookup_get(phone_number)
        print("The response of TwilioPhoneApi->lookup_route_v1_twilio_phone_lookup_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioPhoneApi->lookup_route_v1_twilio_phone_lookup_get: %s\n" % e)
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

# **patch_route_v1_twilio_phone_patch**
> object patch_route_v1_twilio_phone_patch(request_body)

Patch Route

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
    api_instance = valstorm_api.TwilioPhoneApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Patch Route
        api_response = api_instance.patch_route_v1_twilio_phone_patch(request_body)
        print("The response of TwilioPhoneApi->patch_route_v1_twilio_phone_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioPhoneApi->patch_route_v1_twilio_phone_patch: %s\n" % e)
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

# **purchase_phone_address_v1_twilio_phone_purchase_post**
> object purchase_phone_address_v1_twilio_phone_purchase_post(buy_phone_request)

Purchase Phone Address

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.buy_phone_request import BuyPhoneRequest
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
    api_instance = valstorm_api.TwilioPhoneApi(api_client)
    buy_phone_request = valstorm_api.BuyPhoneRequest() # BuyPhoneRequest | 

    try:
        # Purchase Phone Address
        api_response = api_instance.purchase_phone_address_v1_twilio_phone_purchase_post(buy_phone_request)
        print("The response of TwilioPhoneApi->purchase_phone_address_v1_twilio_phone_purchase_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioPhoneApi->purchase_phone_address_v1_twilio_phone_purchase_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **buy_phone_request** | [**BuyPhoneRequest**](BuyPhoneRequest.md)|  | 

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


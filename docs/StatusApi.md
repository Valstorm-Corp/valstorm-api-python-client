# valstorm_api.StatusApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**available_route_v1_status_availability_post**](StatusApi.md#available_route_v1_status_availability_post) | **POST** /v1/status/availability | Available Route
[**get_a_user_v1_status_user_user_id_get**](StatusApi.md#get_a_user_v1_status_user_user_id_get) | **GET** /v1/status/user/{user_id} | Get A User
[**get_all_users_v1_status_users_get**](StatusApi.md#get_all_users_v1_status_users_get) | **GET** /v1/status/users | Get All Users
[**me_v1_status_me_get**](StatusApi.md#me_v1_status_me_get) | **GET** /v1/status/me | Me
[**status_v1_status_get**](StatusApi.md#status_v1_status_get) | **GET** /v1/status | Health Check Endpoint
[**user_status_v1_status_v1_user_status_post**](StatusApi.md#user_status_v1_status_v1_user_status_post) | **POST** /v1/status/v1/user/status | User Status


# **available_route_v1_status_availability_post**
> object available_route_v1_status_availability_post(status_status_routes_available)

Available Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.status_status_routes_available import StatusStatusRoutesAvailable
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
    api_instance = valstorm_api.StatusApi(api_client)
    status_status_routes_available = valstorm_api.StatusStatusRoutesAvailable() # StatusStatusRoutesAvailable | 

    try:
        # Available Route
        api_response = api_instance.available_route_v1_status_availability_post(status_status_routes_available)
        print("The response of StatusApi->available_route_v1_status_availability_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StatusApi->available_route_v1_status_availability_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status_status_routes_available** | [**StatusStatusRoutesAvailable**](StatusStatusRoutesAvailable.md)|  | 

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

# **get_a_user_v1_status_user_user_id_get**
> object get_a_user_v1_status_user_user_id_get(user_id)

Get A User

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
    api_instance = valstorm_api.StatusApi(api_client)
    user_id = 'user_id_example' # str | 

    try:
        # Get A User
        api_response = api_instance.get_a_user_v1_status_user_user_id_get(user_id)
        print("The response of StatusApi->get_a_user_v1_status_user_user_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StatusApi->get_a_user_v1_status_user_user_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**|  | 

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

# **get_all_users_v1_status_users_get**
> object get_all_users_v1_status_users_get()

Get All Users

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
    api_instance = valstorm_api.StatusApi(api_client)

    try:
        # Get All Users
        api_response = api_instance.get_all_users_v1_status_users_get()
        print("The response of StatusApi->get_all_users_v1_status_users_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StatusApi->get_all_users_v1_status_users_get: %s\n" % e)
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

# **me_v1_status_me_get**
> object me_v1_status_me_get()

Me

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
    api_instance = valstorm_api.StatusApi(api_client)

    try:
        # Me
        api_response = api_instance.me_v1_status_me_get()
        print("The response of StatusApi->me_v1_status_me_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StatusApi->me_v1_status_me_get: %s\n" % e)
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

# **status_v1_status_get**
> StatusResponse status_v1_status_get()

Health Check Endpoint

### Example


```python
import valstorm_api
from valstorm_api.models.status_response import StatusResponse
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
    api_instance = valstorm_api.StatusApi(api_client)

    try:
        # Health Check Endpoint
        api_response = api_instance.status_v1_status_get()
        print("The response of StatusApi->status_v1_status_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StatusApi->status_v1_status_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**StatusResponse**](StatusResponse.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **user_status_v1_status_v1_user_status_post**
> object user_status_v1_status_v1_user_status_post(user_status)

User Status

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.user_status import UserStatus
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
    api_instance = valstorm_api.StatusApi(api_client)
    user_status = valstorm_api.UserStatus() # UserStatus | 

    try:
        # User Status
        api_response = api_instance.user_status_v1_status_v1_user_status_post(user_status)
        print("The response of StatusApi->user_status_v1_status_v1_user_status_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StatusApi->user_status_v1_status_v1_user_status_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_status** | [**UserStatus**](UserStatus.md)|  | 

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


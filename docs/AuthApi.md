# valstorm_api.AuthApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**initial_load_v1_auth_load_get**](AuthApi.md#initial_load_v1_auth_load_get) | **GET** /v1/auth/load | Initial Load
[**login_as_v1_auth_login_as_user_post**](AuthApi.md#login_as_v1_auth_login_as_user_post) | **POST** /v1/auth/login-as-user | Login As
[**logout_v1_auth_logout_post**](AuthApi.md#logout_v1_auth_logout_post) | **POST** /v1/auth/logout | Logout
[**switch_org_v1_auth_switch_post**](AuthApi.md#switch_org_v1_auth_switch_post) | **POST** /v1/auth/switch | Switch Org


# **initial_load_v1_auth_load_get**
> object initial_load_v1_auth_load_get()

Initial Load

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
    api_instance = valstorm_api.AuthApi(api_client)

    try:
        # Initial Load
        api_response = api_instance.initial_load_v1_auth_load_get()
        print("The response of AuthApi->initial_load_v1_auth_load_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->initial_load_v1_auth_load_get: %s\n" % e)
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

# **login_as_v1_auth_login_as_user_post**
> Token login_as_v1_auth_login_as_user_post(login_as_request)

Login As

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.login_as_request import LoginAsRequest
from valstorm_api.models.token import Token
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
    api_instance = valstorm_api.AuthApi(api_client)
    login_as_request = valstorm_api.LoginAsRequest() # LoginAsRequest | 

    try:
        # Login As
        api_response = api_instance.login_as_v1_auth_login_as_user_post(login_as_request)
        print("The response of AuthApi->login_as_v1_auth_login_as_user_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->login_as_v1_auth_login_as_user_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **login_as_request** | [**LoginAsRequest**](LoginAsRequest.md)|  | 

### Return type

[**Token**](Token.md)

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

# **logout_v1_auth_logout_post**
> logout_v1_auth_logout_post()

Logout

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
    api_instance = valstorm_api.AuthApi(api_client)

    try:
        # Logout
        api_instance.logout_v1_auth_logout_post()
    except Exception as e:
        print("Exception when calling AuthApi->logout_v1_auth_logout_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Successful Response |  -  |
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **switch_org_v1_auth_switch_post**
> Token switch_org_v1_auth_switch_post(request_body)

Switch Org

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.token import Token
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
    api_instance = valstorm_api.AuthApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Switch Org
        api_response = api_instance.switch_org_v1_auth_switch_post(request_body)
        print("The response of AuthApi->switch_org_v1_auth_switch_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->switch_org_v1_auth_switch_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request_body** | [**Dict[str, object]**](object.md)|  | 

### Return type

[**Token**](Token.md)

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


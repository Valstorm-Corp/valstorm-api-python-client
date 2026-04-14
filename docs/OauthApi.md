# valstorm_api.OauthApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**authorize_route_v1_oauth2_authorize_post**](OauthApi.md#authorize_route_v1_oauth2_authorize_post) | **POST** /v1/oauth2/authorize | Authorize Route
[**code_route_v1_oauth2_code_post**](OauthApi.md#code_route_v1_oauth2_code_post) | **POST** /v1/oauth2/code | Code Route
[**login_route_v1_oauth2_login_post**](OauthApi.md#login_route_v1_oauth2_login_post) | **POST** /v1/oauth2/login | Login Route
[**refresh_token_route_v1_oauth2_refresh_post**](OauthApi.md#refresh_token_route_v1_oauth2_refresh_post) | **POST** /v1/oauth2/refresh | Refresh Token Route
[**request_magic_code_route_v1_auth_request_magic_code_post**](OauthApi.md#request_magic_code_route_v1_auth_request_magic_code_post) | **POST** /v1/auth/request-magic-code | Request Magic Code Route
[**token_route_v1_oauth2_token_post**](OauthApi.md#token_route_v1_oauth2_token_post) | **POST** /v1/oauth2/token | Token Route
[**verify2fa_route_v1_oauth2_verify2fa_post**](OauthApi.md#verify2fa_route_v1_oauth2_verify2fa_post) | **POST** /v1/oauth2/verify-2fa | Verify 2Fa Route


# **authorize_route_v1_oauth2_authorize_post**
> AuthorizationCode authorize_route_v1_oauth2_authorize_post(oauth_authorize_input)

Authorize Route

### Example


```python
import valstorm_api
from valstorm_api.models.authorization_code import AuthorizationCode
from valstorm_api.models.oauth_authorize_input import OauthAuthorizeInput
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
    api_instance = valstorm_api.OauthApi(api_client)
    oauth_authorize_input = valstorm_api.OauthAuthorizeInput() # OauthAuthorizeInput | 

    try:
        # Authorize Route
        api_response = api_instance.authorize_route_v1_oauth2_authorize_post(oauth_authorize_input)
        print("The response of OauthApi->authorize_route_v1_oauth2_authorize_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OauthApi->authorize_route_v1_oauth2_authorize_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **oauth_authorize_input** | [**OauthAuthorizeInput**](OauthAuthorizeInput.md)|  | 

### Return type

[**AuthorizationCode**](AuthorizationCode.md)

### Authorization

No authorization required

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

# **code_route_v1_oauth2_code_post**
> CodeUrl code_route_v1_oauth2_code_post(oauth_code_input)

Code Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.code_url import CodeUrl
from valstorm_api.models.oauth_code_input import OauthCodeInput
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
    api_instance = valstorm_api.OauthApi(api_client)
    oauth_code_input = valstorm_api.OauthCodeInput() # OauthCodeInput | 

    try:
        # Code Route
        api_response = api_instance.code_route_v1_oauth2_code_post(oauth_code_input)
        print("The response of OauthApi->code_route_v1_oauth2_code_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OauthApi->code_route_v1_oauth2_code_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **oauth_code_input** | [**OauthCodeInput**](OauthCodeInput.md)|  | 

### Return type

[**CodeUrl**](CodeUrl.md)

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

# **login_route_v1_oauth2_login_post**
> ResponseLoginRouteV1Oauth2LoginPost login_route_v1_oauth2_login_post(grant_type, username, password, scope=scope, client_id=client_id, client_secret=client_secret)

Login Route

### Example


```python
import valstorm_api
from valstorm_api.models.response_login_route_v1_oauth2_login_post import ResponseLoginRouteV1Oauth2LoginPost
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
    api_instance = valstorm_api.OauthApi(api_client)
    grant_type = 'grant_type_example' # str | 
    username = 'username_example' # str | 
    password = 'password_example' # str | 
    scope = '' # str |  (optional) (default to '')
    client_id = 'client_id_example' # str |  (optional)
    client_secret = 'client_secret_example' # str |  (optional)

    try:
        # Login Route
        api_response = api_instance.login_route_v1_oauth2_login_post(grant_type, username, password, scope=scope, client_id=client_id, client_secret=client_secret)
        print("The response of OauthApi->login_route_v1_oauth2_login_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OauthApi->login_route_v1_oauth2_login_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **grant_type** | **str**|  | 
 **username** | **str**|  | 
 **password** | **str**|  | 
 **scope** | **str**|  | [optional] [default to &#39;&#39;]
 **client_id** | **str**|  | [optional] 
 **client_secret** | **str**|  | [optional] 

### Return type

[**ResponseLoginRouteV1Oauth2LoginPost**](ResponseLoginRouteV1Oauth2LoginPost.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **refresh_token_route_v1_oauth2_refresh_post**
> AccessToken refresh_token_route_v1_oauth2_refresh_post(refresh_token)

Refresh Token Route

### Example


```python
import valstorm_api
from valstorm_api.models.access_token import AccessToken
from valstorm_api.models.refresh_token import RefreshToken
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
    api_instance = valstorm_api.OauthApi(api_client)
    refresh_token = valstorm_api.RefreshToken() # RefreshToken | 

    try:
        # Refresh Token Route
        api_response = api_instance.refresh_token_route_v1_oauth2_refresh_post(refresh_token)
        print("The response of OauthApi->refresh_token_route_v1_oauth2_refresh_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OauthApi->refresh_token_route_v1_oauth2_refresh_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **refresh_token** | [**RefreshToken**](RefreshToken.md)|  | 

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

No authorization required

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

# **request_magic_code_route_v1_auth_request_magic_code_post**
> AcceptedResponse request_magic_code_route_v1_auth_request_magic_code_post(magic_code_request)

Request Magic Code Route

### Example


```python
import valstorm_api
from valstorm_api.models.accepted_response import AcceptedResponse
from valstorm_api.models.magic_code_request import MagicCodeRequest
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
    api_instance = valstorm_api.OauthApi(api_client)
    magic_code_request = valstorm_api.MagicCodeRequest() # MagicCodeRequest | 

    try:
        # Request Magic Code Route
        api_response = api_instance.request_magic_code_route_v1_auth_request_magic_code_post(magic_code_request)
        print("The response of OauthApi->request_magic_code_route_v1_auth_request_magic_code_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OauthApi->request_magic_code_route_v1_auth_request_magic_code_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **magic_code_request** | [**MagicCodeRequest**](MagicCodeRequest.md)|  | 

### Return type

[**AcceptedResponse**](AcceptedResponse.md)

### Authorization

No authorization required

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

# **token_route_v1_oauth2_token_post**
> Token token_route_v1_oauth2_token_post(oauth_request_token)

Token Route

### Example


```python
import valstorm_api
from valstorm_api.models.oauth_request_token import OauthRequestToken
from valstorm_api.models.token import Token
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
    api_instance = valstorm_api.OauthApi(api_client)
    oauth_request_token = valstorm_api.OauthRequestToken() # OauthRequestToken | 

    try:
        # Token Route
        api_response = api_instance.token_route_v1_oauth2_token_post(oauth_request_token)
        print("The response of OauthApi->token_route_v1_oauth2_token_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OauthApi->token_route_v1_oauth2_token_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **oauth_request_token** | [**OauthRequestToken**](OauthRequestToken.md)|  | 

### Return type

[**Token**](Token.md)

### Authorization

No authorization required

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

# **verify2fa_route_v1_oauth2_verify2fa_post**
> Token verify2fa_route_v1_oauth2_verify2fa_post(verify2_fa_payload)

Verify 2Fa Route

### Example


```python
import valstorm_api
from valstorm_api.models.token import Token
from valstorm_api.models.verify2_fa_payload import Verify2FAPayload
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
    api_instance = valstorm_api.OauthApi(api_client)
    verify2_fa_payload = valstorm_api.Verify2FAPayload() # Verify2FAPayload | 

    try:
        # Verify 2Fa Route
        api_response = api_instance.verify2fa_route_v1_oauth2_verify2fa_post(verify2_fa_payload)
        print("The response of OauthApi->verify2fa_route_v1_oauth2_verify2fa_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OauthApi->verify2fa_route_v1_oauth2_verify2fa_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **verify2_fa_payload** | [**Verify2FAPayload**](Verify2FAPayload.md)|  | 

### Return type

[**Token**](Token.md)

### Authorization

No authorization required

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


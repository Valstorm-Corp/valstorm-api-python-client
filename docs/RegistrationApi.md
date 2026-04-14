# valstorm_api.RegistrationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activate_invite_v1_register_activate_invite_post**](RegistrationApi.md#activate_invite_v1_register_activate_invite_post) | **POST** /v1/register/activate-invite | Activate Invite
[**activate_user_v1_register_activate_post**](RegistrationApi.md#activate_user_v1_register_activate_post) | **POST** /v1/register/activate | Activate User
[**register_user_to_org_v1_register_user_post**](RegistrationApi.md#register_user_to_org_v1_register_user_post) | **POST** /v1/register/user | Register User To Org
[**register_user_v1_register_post**](RegistrationApi.md#register_user_v1_register_post) | **POST** /v1/register | Register User


# **activate_invite_v1_register_activate_invite_post**
> object activate_invite_v1_register_activate_invite_post(accept_activation_invite)

Activate Invite

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.accept_activation_invite import AcceptActivationInvite
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
    api_instance = valstorm_api.RegistrationApi(api_client)
    accept_activation_invite = valstorm_api.AcceptActivationInvite() # AcceptActivationInvite | 

    try:
        # Activate Invite
        api_response = api_instance.activate_invite_v1_register_activate_invite_post(accept_activation_invite)
        print("The response of RegistrationApi->activate_invite_v1_register_activate_invite_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistrationApi->activate_invite_v1_register_activate_invite_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept_activation_invite** | [**AcceptActivationInvite**](AcceptActivationInvite.md)|  | 

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
**201** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activate_user_v1_register_activate_post**
> ActivationResponse activate_user_v1_register_activate_post(user_activation_request)

Activate User

### Example


```python
import valstorm_api
from valstorm_api.models.activation_response import ActivationResponse
from valstorm_api.models.user_activation_request import UserActivationRequest
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
    api_instance = valstorm_api.RegistrationApi(api_client)
    user_activation_request = valstorm_api.UserActivationRequest() # UserActivationRequest | 

    try:
        # Activate User
        api_response = api_instance.activate_user_v1_register_activate_post(user_activation_request)
        print("The response of RegistrationApi->activate_user_v1_register_activate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistrationApi->activate_user_v1_register_activate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_activation_request** | [**UserActivationRequest**](UserActivationRequest.md)|  | 

### Return type

[**ActivationResponse**](ActivationResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **register_user_to_org_v1_register_user_post**
> UserRegistrationResponse register_user_to_org_v1_register_user_post(user_registration_request)

Register User To Org

Registers a user to an organization.
- If user is new to Valstorm: Creates globally and in Org.
- If user exists in Valstorm: Links existing user to this Org.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.user_registration_request import UserRegistrationRequest
from valstorm_api.models.user_registration_response import UserRegistrationResponse
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
    api_instance = valstorm_api.RegistrationApi(api_client)
    user_registration_request = valstorm_api.UserRegistrationRequest() # UserRegistrationRequest | 

    try:
        # Register User To Org
        api_response = api_instance.register_user_to_org_v1_register_user_post(user_registration_request)
        print("The response of RegistrationApi->register_user_to_org_v1_register_user_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistrationApi->register_user_to_org_v1_register_user_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_registration_request** | [**UserRegistrationRequest**](UserRegistrationRequest.md)|  | 

### Return type

[**UserRegistrationResponse**](UserRegistrationResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **register_user_v1_register_post**
> RegistrationResponse register_user_v1_register_post(registration_request)

Register User

### Example


```python
import valstorm_api
from valstorm_api.models.registration_request import RegistrationRequest
from valstorm_api.models.registration_response import RegistrationResponse
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
    api_instance = valstorm_api.RegistrationApi(api_client)
    registration_request = valstorm_api.RegistrationRequest() # RegistrationRequest | 

    try:
        # Register User
        api_response = api_instance.register_user_v1_register_post(registration_request)
        print("The response of RegistrationApi->register_user_v1_register_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistrationApi->register_user_v1_register_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registration_request** | [**RegistrationRequest**](RegistrationRequest.md)|  | 

### Return type

[**RegistrationResponse**](RegistrationResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


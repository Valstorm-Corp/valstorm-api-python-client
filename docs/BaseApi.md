# valstorm_api.BaseApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**forgot_password_v1_forgot_password_post**](BaseApi.md#forgot_password_v1_forgot_password_post) | **POST** /v1/forgot-password | Forgot Password


# **forgot_password_v1_forgot_password_post**
> object forgot_password_v1_forgot_password_post(request_body)

Forgot Password

Initiates the password reset flow.
Generates a new activation code and emails the user.

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
    api_instance = valstorm_api.BaseApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Forgot Password
        api_response = api_instance.forgot_password_v1_forgot_password_post(request_body)
        print("The response of BaseApi->forgot_password_v1_forgot_password_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BaseApi->forgot_password_v1_forgot_password_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request_body** | [**Dict[str, object]**](object.md)|  | 

### Return type

**object**

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


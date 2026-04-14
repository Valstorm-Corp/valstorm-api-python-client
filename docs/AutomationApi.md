# valstorm_api.AutomationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**resume_automation_route_v1_automation_resume_run_id_post**](AutomationApi.md#resume_automation_route_v1_automation_resume_run_id_post) | **POST** /v1/automation/resume/{run_id} | Resume Automation Route
[**run_automation_by_id_route_v1_automation_automation_id_post**](AutomationApi.md#run_automation_by_id_route_v1_automation_automation_id_post) | **POST** /v1/automation/{automation_id} | Run Automation By Id Route
[**run_automation_route_v1_automation_post**](AutomationApi.md#run_automation_route_v1_automation_post) | **POST** /v1/automation | Run Automation Route
[**run_function_automation_route_v1_automation_function_post**](AutomationApi.md#run_function_automation_route_v1_automation_function_post) | **POST** /v1/automation/function | Run Function Automation Route
[**run_partial_automation_route_v1_automation_run_partial_run_id_post**](AutomationApi.md#run_partial_automation_route_v1_automation_run_partial_run_id_post) | **POST** /v1/automation/run-partial/{run_id} | Run Partial Automation Route
[**run_public_automation_route_v1_public_automation_org_id_automation_id_post**](AutomationApi.md#run_public_automation_route_v1_public_automation_org_id_automation_id_post) | **POST** /v1/public/automation/{org_id}/{automation_id} | Run Public Automation Route


# **resume_automation_route_v1_automation_resume_run_id_post**
> object resume_automation_route_v1_automation_resume_run_id_post(run_id)

Resume Automation Route

Automatically resumes a workflow from where it last stopped.

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
    api_instance = valstorm_api.AutomationApi(api_client)
    run_id = 'run_id_example' # str | 

    try:
        # Resume Automation Route
        api_response = api_instance.resume_automation_route_v1_automation_resume_run_id_post(run_id)
        print("The response of AutomationApi->resume_automation_route_v1_automation_resume_run_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->resume_automation_route_v1_automation_resume_run_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **run_id** | **str**|  | 

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

# **run_automation_by_id_route_v1_automation_automation_id_post**
> object run_automation_by_id_route_v1_automation_automation_id_post(automation_id)

Run Automation By Id Route

Runs a saved automation by its ID, using the incoming request body as inputs.

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
    api_instance = valstorm_api.AutomationApi(api_client)
    automation_id = 'automation_id_example' # str | 

    try:
        # Run Automation By Id Route
        api_response = api_instance.run_automation_by_id_route_v1_automation_automation_id_post(automation_id)
        print("The response of AutomationApi->run_automation_by_id_route_v1_automation_automation_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->run_automation_by_id_route_v1_automation_automation_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **automation_id** | **str**|  | 

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

# **run_automation_route_v1_automation_post**
> object run_automation_route_v1_automation_post()

Run Automation Route

Runs a new automation from a raw payload (JSON, form-data, etc.).

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
    api_instance = valstorm_api.AutomationApi(api_client)

    try:
        # Run Automation Route
        api_response = api_instance.run_automation_route_v1_automation_post()
        print("The response of AutomationApi->run_automation_route_v1_automation_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->run_automation_route_v1_automation_post: %s\n" % e)
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

# **run_function_automation_route_v1_automation_function_post**
> object run_function_automation_route_v1_automation_function_post(function_request)

Run Function Automation Route

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.function_request import FunctionRequest
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
    api_instance = valstorm_api.AutomationApi(api_client)
    function_request = valstorm_api.FunctionRequest() # FunctionRequest | 

    try:
        # Run Function Automation Route
        api_response = api_instance.run_function_automation_route_v1_automation_function_post(function_request)
        print("The response of AutomationApi->run_function_automation_route_v1_automation_function_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->run_function_automation_route_v1_automation_function_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **function_request** | [**FunctionRequest**](FunctionRequest.md)|  | 

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

# **run_partial_automation_route_v1_automation_run_partial_run_id_post**
> object run_partial_automation_route_v1_automation_run_partial_run_id_post(run_id)

Run Partial Automation Route

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
    api_instance = valstorm_api.AutomationApi(api_client)
    run_id = 'run_id_example' # str | 

    try:
        # Run Partial Automation Route
        api_response = api_instance.run_partial_automation_route_v1_automation_run_partial_run_id_post(run_id)
        print("The response of AutomationApi->run_partial_automation_route_v1_automation_run_partial_run_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->run_partial_automation_route_v1_automation_run_partial_run_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **run_id** | **str**|  | 

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

# **run_public_automation_route_v1_public_automation_org_id_automation_id_post**
> object run_public_automation_route_v1_public_automation_org_id_automation_id_post(org_id, automation_id)

Run Public Automation Route

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
    api_instance = valstorm_api.AutomationApi(api_client)
    org_id = 'org_id_example' # str | 
    automation_id = 'automation_id_example' # str | 

    try:
        # Run Public Automation Route
        api_response = api_instance.run_public_automation_route_v1_public_automation_org_id_automation_id_post(org_id, automation_id)
        print("The response of AutomationApi->run_public_automation_route_v1_public_automation_org_id_automation_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->run_public_automation_route_v1_public_automation_org_id_automation_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 
 **automation_id** | **str**|  | 

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


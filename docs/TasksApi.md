# valstorm_api.TasksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**check_availability_v1_tasks_availability_post**](TasksApi.md#check_availability_v1_tasks_availability_post) | **POST** /v1/tasks/availability | Check Availability
[**fix_convos_task_v1_tasks_fix_convos_post**](TasksApi.md#fix_convos_task_v1_tasks_fix_convos_post) | **POST** /v1/tasks/fix-convos | Fix Convos Task
[**rebuild_schemas_route_v1_tasks_rebuild_schemas_post**](TasksApi.md#rebuild_schemas_route_v1_tasks_rebuild_schemas_post) | **POST** /v1/tasks/rebuild_schemas | Rebuild Schemas Route
[**start_function_v1_tasks_functions_post**](TasksApi.md#start_function_v1_tasks_functions_post) | **POST** /v1/tasks/functions | Start Function
[**start_task_v1_tasks_post**](TasksApi.md#start_task_v1_tasks_post) | **POST** /v1/tasks | Start Task
[**system_alert_v1_tasks_system_alert_post**](TasksApi.md#system_alert_v1_tasks_system_alert_post) | **POST** /v1/tasks/system-alert | System Alert


# **check_availability_v1_tasks_availability_post**
> object check_availability_v1_tasks_availability_post(check_availability)

Check Availability

Checks user availability hourly

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.check_availability import CheckAvailability
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
    api_instance = valstorm_api.TasksApi(api_client)
    check_availability = valstorm_api.CheckAvailability() # CheckAvailability | 

    try:
        # Check Availability
        api_response = api_instance.check_availability_v1_tasks_availability_post(check_availability)
        print("The response of TasksApi->check_availability_v1_tasks_availability_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->check_availability_v1_tasks_availability_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **check_availability** | [**CheckAvailability**](CheckAvailability.md)|  | 

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

# **fix_convos_task_v1_tasks_fix_convos_post**
> object fix_convos_task_v1_tasks_fix_convos_post()

Fix Convos Task

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
    api_instance = valstorm_api.TasksApi(api_client)

    try:
        # Fix Convos Task
        api_response = api_instance.fix_convos_task_v1_tasks_fix_convos_post()
        print("The response of TasksApi->fix_convos_task_v1_tasks_fix_convos_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->fix_convos_task_v1_tasks_fix_convos_post: %s\n" % e)
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

# **rebuild_schemas_route_v1_tasks_rebuild_schemas_post**
> object rebuild_schemas_route_v1_tasks_rebuild_schemas_post()

Rebuild Schemas Route

Rebuilds schemas for the organization

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
    api_instance = valstorm_api.TasksApi(api_client)

    try:
        # Rebuild Schemas Route
        api_response = api_instance.rebuild_schemas_route_v1_tasks_rebuild_schemas_post()
        print("The response of TasksApi->rebuild_schemas_route_v1_tasks_rebuild_schemas_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->rebuild_schemas_route_v1_tasks_rebuild_schemas_post: %s\n" % e)
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

# **start_function_v1_tasks_functions_post**
> object start_function_v1_tasks_functions_post(start_task)

Start Function

Runs Dynamic Code

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.start_task import StartTask
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
    api_instance = valstorm_api.TasksApi(api_client)
    start_task = valstorm_api.StartTask() # StartTask | 

    try:
        # Start Function
        api_response = api_instance.start_function_v1_tasks_functions_post(start_task)
        print("The response of TasksApi->start_function_v1_tasks_functions_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->start_function_v1_tasks_functions_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **start_task** | [**StartTask**](StartTask.md)|  | 

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

# **start_task_v1_tasks_post**
> object start_task_v1_tasks_post(start_task)

Start Task

Runs defined tasks from the tasks folder

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.start_task import StartTask
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
    api_instance = valstorm_api.TasksApi(api_client)
    start_task = valstorm_api.StartTask() # StartTask | 

    try:
        # Start Task
        api_response = api_instance.start_task_v1_tasks_post(start_task)
        print("The response of TasksApi->start_task_v1_tasks_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->start_task_v1_tasks_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **start_task** | [**StartTask**](StartTask.md)|  | 

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

# **system_alert_v1_tasks_system_alert_post**
> object system_alert_v1_tasks_system_alert_post(request_body)

System Alert

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
    api_instance = valstorm_api.TasksApi(api_client)
    request_body = None # List[Dict[str, object]] | 

    try:
        # System Alert
        api_response = api_instance.system_alert_v1_tasks_system_alert_post(request_body)
        print("The response of TasksApi->system_alert_v1_tasks_system_alert_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->system_alert_v1_tasks_system_alert_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request_body** | [**List[Dict[str, object]]**](Dict.md)|  | 

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


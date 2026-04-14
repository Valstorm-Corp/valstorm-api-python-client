# valstorm_api.SalesforceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bulk_query_results_salesforce_v1_c_salesforce_bulk_query_job_id_results_get**](SalesforceApi.md#bulk_query_results_salesforce_v1_c_salesforce_bulk_query_job_id_results_get) | **GET** /v1/c/salesforce/bulk/query/{job_id}/results | Bulk Query Results Salesforce
[**bulk_query_salesforce_v1_c_salesforce_bulk_query_post**](SalesforceApi.md#bulk_query_salesforce_v1_c_salesforce_bulk_query_post) | **POST** /v1/c/salesforce/bulk/query | Bulk Query Salesforce
[**bulk_query_status_salesforce_v1_c_salesforce_bulk_query_job_id_get**](SalesforceApi.md#bulk_query_status_salesforce_v1_c_salesforce_bulk_query_job_id_get) | **GET** /v1/c/salesforce/bulk/query/{job_id} | Bulk Query Status Salesforce
[**create_salesforce_records_route_v1_c_salesforce_sobjects_post**](SalesforceApi.md#create_salesforce_records_route_v1_c_salesforce_sobjects_post) | **POST** /v1/c/salesforce/sobjects | Create Salesforce Records Route
[**describe_salesforce_route_v1_c_salesforce_describe_object_name_get**](SalesforceApi.md#describe_salesforce_route_v1_c_salesforce_describe_object_name_get) | **GET** /v1/c/salesforce/describe/{object_name} | Describe Salesforce Route
[**get_report_v1_c_salesforce_reports_report_id_get**](SalesforceApi.md#get_report_v1_c_salesforce_reports_report_id_get) | **GET** /v1/c/salesforce/reports/{report_id} | Get Report
[**query_salesforce_route_v1_c_salesforce_query_get**](SalesforceApi.md#query_salesforce_route_v1_c_salesforce_query_get) | **GET** /v1/c/salesforce/query | Query Salesforce Route
[**update_salesforce_records_route_v1_c_salesforce_sobjects_patch**](SalesforceApi.md#update_salesforce_records_route_v1_c_salesforce_sobjects_patch) | **PATCH** /v1/c/salesforce/sobjects | Update Salesforce Records Route


# **bulk_query_results_salesforce_v1_c_salesforce_bulk_query_job_id_results_get**
> object bulk_query_results_salesforce_v1_c_salesforce_bulk_query_job_id_results_get(job_id)

Bulk Query Results Salesforce

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
    api_instance = valstorm_api.SalesforceApi(api_client)
    job_id = 'job_id_example' # str | 

    try:
        # Bulk Query Results Salesforce
        api_response = api_instance.bulk_query_results_salesforce_v1_c_salesforce_bulk_query_job_id_results_get(job_id)
        print("The response of SalesforceApi->bulk_query_results_salesforce_v1_c_salesforce_bulk_query_job_id_results_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SalesforceApi->bulk_query_results_salesforce_v1_c_salesforce_bulk_query_job_id_results_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **job_id** | **str**|  | 

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

# **bulk_query_salesforce_v1_c_salesforce_bulk_query_post**
> object bulk_query_salesforce_v1_c_salesforce_bulk_query_post(request_body)

Bulk Query Salesforce

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
    api_instance = valstorm_api.SalesforceApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Bulk Query Salesforce
        api_response = api_instance.bulk_query_salesforce_v1_c_salesforce_bulk_query_post(request_body)
        print("The response of SalesforceApi->bulk_query_salesforce_v1_c_salesforce_bulk_query_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SalesforceApi->bulk_query_salesforce_v1_c_salesforce_bulk_query_post: %s\n" % e)
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

# **bulk_query_status_salesforce_v1_c_salesforce_bulk_query_job_id_get**
> object bulk_query_status_salesforce_v1_c_salesforce_bulk_query_job_id_get(job_id)

Bulk Query Status Salesforce

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
    api_instance = valstorm_api.SalesforceApi(api_client)
    job_id = 'job_id_example' # str | 

    try:
        # Bulk Query Status Salesforce
        api_response = api_instance.bulk_query_status_salesforce_v1_c_salesforce_bulk_query_job_id_get(job_id)
        print("The response of SalesforceApi->bulk_query_status_salesforce_v1_c_salesforce_bulk_query_job_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SalesforceApi->bulk_query_status_salesforce_v1_c_salesforce_bulk_query_job_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **job_id** | **str**|  | 

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

# **create_salesforce_records_route_v1_c_salesforce_sobjects_post**
> object create_salesforce_records_route_v1_c_salesforce_sobjects_post(request_body)

Create Salesforce Records Route

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
    api_instance = valstorm_api.SalesforceApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Create Salesforce Records Route
        api_response = api_instance.create_salesforce_records_route_v1_c_salesforce_sobjects_post(request_body)
        print("The response of SalesforceApi->create_salesforce_records_route_v1_c_salesforce_sobjects_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SalesforceApi->create_salesforce_records_route_v1_c_salesforce_sobjects_post: %s\n" % e)
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

# **describe_salesforce_route_v1_c_salesforce_describe_object_name_get**
> object describe_salesforce_route_v1_c_salesforce_describe_object_name_get(object_name)

Describe Salesforce Route

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
    api_instance = valstorm_api.SalesforceApi(api_client)
    object_name = 'object_name_example' # str | 

    try:
        # Describe Salesforce Route
        api_response = api_instance.describe_salesforce_route_v1_c_salesforce_describe_object_name_get(object_name)
        print("The response of SalesforceApi->describe_salesforce_route_v1_c_salesforce_describe_object_name_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SalesforceApi->describe_salesforce_route_v1_c_salesforce_describe_object_name_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_name** | **str**|  | 

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

# **get_report_v1_c_salesforce_reports_report_id_get**
> object get_report_v1_c_salesforce_reports_report_id_get(report_id)

Get Report

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
    api_instance = valstorm_api.SalesforceApi(api_client)
    report_id = 'report_id_example' # str | 

    try:
        # Get Report
        api_response = api_instance.get_report_v1_c_salesforce_reports_report_id_get(report_id)
        print("The response of SalesforceApi->get_report_v1_c_salesforce_reports_report_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SalesforceApi->get_report_v1_c_salesforce_reports_report_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **report_id** | **str**|  | 

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

# **query_salesforce_route_v1_c_salesforce_query_get**
> object query_salesforce_route_v1_c_salesforce_query_get()

Query Salesforce Route

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
    api_instance = valstorm_api.SalesforceApi(api_client)

    try:
        # Query Salesforce Route
        api_response = api_instance.query_salesforce_route_v1_c_salesforce_query_get()
        print("The response of SalesforceApi->query_salesforce_route_v1_c_salesforce_query_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SalesforceApi->query_salesforce_route_v1_c_salesforce_query_get: %s\n" % e)
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

# **update_salesforce_records_route_v1_c_salesforce_sobjects_patch**
> object update_salesforce_records_route_v1_c_salesforce_sobjects_patch(request_body)

Update Salesforce Records Route

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
    api_instance = valstorm_api.SalesforceApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Update Salesforce Records Route
        api_response = api_instance.update_salesforce_records_route_v1_c_salesforce_sobjects_patch(request_body)
        print("The response of SalesforceApi->update_salesforce_records_route_v1_c_salesforce_sobjects_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SalesforceApi->update_salesforce_records_route_v1_c_salesforce_sobjects_patch: %s\n" % e)
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


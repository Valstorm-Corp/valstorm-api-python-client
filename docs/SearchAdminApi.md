# valstorm_api.SearchAdminApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**check_opensearch_connection_v1_search_admin_connection_get**](SearchAdminApi.md#check_opensearch_connection_v1_search_admin_connection_get) | **GET** /v1/search-admin/connection | Check OpenSearch Connection
[**create_new_index_v1_search_admin_index_index_name_post**](SearchAdminApi.md#create_new_index_v1_search_admin_index_index_name_post) | **POST** /v1/search-admin/index/{index_name} | Create Index
[**delete_existing_index_v1_search_admin_index_index_name_delete**](SearchAdminApi.md#delete_existing_index_v1_search_admin_index_index_name_delete) | **DELETE** /v1/search-admin/index/{index_name} | Delete Index
[**flush_opensearch_database_v1_search_admin_flush_db_delete**](SearchAdminApi.md#flush_opensearch_database_v1_search_admin_flush_db_delete) | **DELETE** /v1/search-admin/flush-db | Flush Application Indexes
[**get_all_documents_in_index_v1_search_admin_index_index_name_documents_get**](SearchAdminApi.md#get_all_documents_in_index_v1_search_admin_index_index_name_documents_get) | **GET** /v1/search-admin/index/{index_name}/documents | Get All Documents in Index
[**get_index_info_v1_search_admin_index_index_name_get**](SearchAdminApi.md#get_index_info_v1_search_admin_index_index_name_get) | **GET** /v1/search-admin/index/{index_name} | Get Index Information
[**list_all_system_opensearch_indexes_v1_search_admin_index_all_system_get**](SearchAdminApi.md#list_all_system_opensearch_indexes_v1_search_admin_index_all_system_get) | **GET** /v1/search-admin/index/all-system | List All System Indexes
[**list_app_opensearch_indexes_v1_search_admin_index_app_indexes_get**](SearchAdminApi.md#list_app_opensearch_indexes_v1_search_admin_index_app_indexes_get) | **GET** /v1/search-admin/index/app-indexes | List Application Indexes
[**trigger_doc_indexing_v1_search_admin_index_docs_post**](SearchAdminApi.md#trigger_doc_indexing_v1_search_admin_index_docs_post) | **POST** /v1/search-admin/index/docs | Trigger Documentation Indexing
[**update_index_configuration_v1_search_admin_index_index_name_settings_put**](SearchAdminApi.md#update_index_configuration_v1_search_admin_index_index_name_settings_put) | **PUT** /v1/search-admin/index/{index_name}/settings | Update Index Settings


# **check_opensearch_connection_v1_search_admin_connection_get**
> object check_opensearch_connection_v1_search_admin_connection_get()

Check OpenSearch Connection

Checks the connection status to the OpenSearch cluster.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)

    try:
        # Check OpenSearch Connection
        api_response = api_instance.check_opensearch_connection_v1_search_admin_connection_get()
        print("The response of SearchAdminApi->check_opensearch_connection_v1_search_admin_connection_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->check_opensearch_connection_v1_search_admin_connection_get: %s\n" % e)
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

# **create_new_index_v1_search_admin_index_index_name_post**
> object create_new_index_v1_search_admin_index_index_name_post(index_name, request_body=request_body)

Create Index

Creates a new application-specific ('vs_*') index in OpenSearch.
- **index_name**: The base name of the index to create (e.g., 'my_index').
- **settings**: (Optional) A JSON body with index settings.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)
    index_name = 'index_name_example' # str | 
    request_body = None # Dict[str, object] |  (optional)

    try:
        # Create Index
        api_response = api_instance.create_new_index_v1_search_admin_index_index_name_post(index_name, request_body=request_body)
        print("The response of SearchAdminApi->create_new_index_v1_search_admin_index_index_name_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->create_new_index_v1_search_admin_index_index_name_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **index_name** | **str**|  | 
 **request_body** | [**Dict[str, object]**](object.md)|  | [optional] 

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

# **delete_existing_index_v1_search_admin_index_index_name_delete**
> object delete_existing_index_v1_search_admin_index_index_name_delete(index_name)

Delete Index

Deletes a specific application-specific ('vs_*') index.
- **index_name**: The base name of the index to delete.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)
    index_name = 'index_name_example' # str | 

    try:
        # Delete Index
        api_response = api_instance.delete_existing_index_v1_search_admin_index_index_name_delete(index_name)
        print("The response of SearchAdminApi->delete_existing_index_v1_search_admin_index_index_name_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->delete_existing_index_v1_search_admin_index_index_name_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **index_name** | **str**|  | 

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

# **flush_opensearch_database_v1_search_admin_flush_db_delete**
> object flush_opensearch_database_v1_search_admin_flush_db_delete()

Flush Application Indexes

**DANGEROUS OPERATION.** Deletes all application-specific ('vs_*') indexes.
This is intended for resetting the testing environment.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)

    try:
        # Flush Application Indexes
        api_response = api_instance.flush_opensearch_database_v1_search_admin_flush_db_delete()
        print("The response of SearchAdminApi->flush_opensearch_database_v1_search_admin_flush_db_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->flush_opensearch_database_v1_search_admin_flush_db_delete: %s\n" % e)
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

# **get_all_documents_in_index_v1_search_admin_index_index_name_documents_get**
> object get_all_documents_in_index_v1_search_admin_index_index_name_documents_get(index_name, limit=limit)

Get All Documents in Index

Retrieves all documents from a specific application-specific ('vs_*') index.
Mainly for debugging to verify index contents.
- **index_name**: The base name of the index to query.
- **limit**: The maximum number of documents to return.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)
    index_name = 'index_name_example' # str | 
    limit = 100 # int |  (optional) (default to 100)

    try:
        # Get All Documents in Index
        api_response = api_instance.get_all_documents_in_index_v1_search_admin_index_index_name_documents_get(index_name, limit=limit)
        print("The response of SearchAdminApi->get_all_documents_in_index_v1_search_admin_index_index_name_documents_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->get_all_documents_in_index_v1_search_admin_index_index_name_documents_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **index_name** | **str**|  | 
 **limit** | **int**|  | [optional] [default to 100]

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

# **get_index_info_v1_search_admin_index_index_name_get**
> object get_index_info_v1_search_admin_index_index_name_get(index_name)

Get Index Information

Retrieves information for a specific application-specific ('vs_*') index.
- **index_name**: The base name of the index to retrieve.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)
    index_name = 'index_name_example' # str | 

    try:
        # Get Index Information
        api_response = api_instance.get_index_info_v1_search_admin_index_index_name_get(index_name)
        print("The response of SearchAdminApi->get_index_info_v1_search_admin_index_index_name_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->get_index_info_v1_search_admin_index_index_name_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **index_name** | **str**|  | 

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

# **list_all_system_opensearch_indexes_v1_search_admin_index_all_system_get**
> object list_all_system_opensearch_indexes_v1_search_admin_index_all_system_get()

List All System Indexes

Retrieves a list of ALL index names currently in the OpenSearch cluster, 
including protected system indexes.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)

    try:
        # List All System Indexes
        api_response = api_instance.list_all_system_opensearch_indexes_v1_search_admin_index_all_system_get()
        print("The response of SearchAdminApi->list_all_system_opensearch_indexes_v1_search_admin_index_all_system_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->list_all_system_opensearch_indexes_v1_search_admin_index_all_system_get: %s\n" % e)
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

# **list_app_opensearch_indexes_v1_search_admin_index_app_indexes_get**
> object list_app_opensearch_indexes_v1_search_admin_index_app_indexes_get()

List Application Indexes

Retrieves a list of all application-specific index names (prefixed with 'vs_') 
currently in the OpenSearch cluster.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)

    try:
        # List Application Indexes
        api_response = api_instance.list_app_opensearch_indexes_v1_search_admin_index_app_indexes_get()
        print("The response of SearchAdminApi->list_app_opensearch_indexes_v1_search_admin_index_app_indexes_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->list_app_opensearch_indexes_v1_search_admin_index_app_indexes_get: %s\n" % e)
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

# **trigger_doc_indexing_v1_search_admin_index_docs_post**
> object trigger_doc_indexing_v1_search_admin_index_docs_post(index_name=index_name, run_async=run_async)

Trigger Documentation Indexing

Manually triggers the OpenSearch indexing task for documentation site data.

- **run_async**: If `true`, the task runs in the background and the API returns a task ID.
If `false` (default), the API waits for the task to complete and returns the full result.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)
    index_name = 'docs_index' # str |  (optional) (default to 'docs_index')
    run_async = False # bool |  (optional) (default to False)

    try:
        # Trigger Documentation Indexing
        api_response = api_instance.trigger_doc_indexing_v1_search_admin_index_docs_post(index_name=index_name, run_async=run_async)
        print("The response of SearchAdminApi->trigger_doc_indexing_v1_search_admin_index_docs_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->trigger_doc_indexing_v1_search_admin_index_docs_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **index_name** | **str**|  | [optional] [default to &#39;docs_index&#39;]
 **run_async** | **bool**|  | [optional] [default to False]

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

# **update_index_configuration_v1_search_admin_index_index_name_settings_put**
> object update_index_configuration_v1_search_admin_index_index_name_settings_put(index_name, request_body)

Update Index Settings

Updates the settings of an existing application-specific ('vs_*') index.
- **index_name**: The base name of the index to update.
- **settings**: A JSON body with the settings to update.
- **Requires admin privileges.**

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
    api_instance = valstorm_api.SearchAdminApi(api_client)
    index_name = 'index_name_example' # str | 
    request_body = None # Dict[str, object] | 

    try:
        # Update Index Settings
        api_response = api_instance.update_index_configuration_v1_search_admin_index_index_name_settings_put(index_name, request_body)
        print("The response of SearchAdminApi->update_index_configuration_v1_search_admin_index_index_name_settings_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchAdminApi->update_index_configuration_v1_search_admin_index_index_name_settings_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **index_name** | **str**|  | 
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


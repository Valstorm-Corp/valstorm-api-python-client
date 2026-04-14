# valstorm_api.RecordsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_records_api_v1_object_collection_name_post**](RecordsApi.md#create_records_api_v1_object_collection_name_post) | **POST** /v1/object/{collection_name} | Create Records Api
[**csv_to_json_v1_csv_to_json_post**](RecordsApi.md#csv_to_json_v1_csv_to_json_post) | **POST** /v1/csv-to-json | Csv To Json
[**decrypt_record_route_v1_decrypt_collection_name_get**](RecordsApi.md#decrypt_record_route_v1_decrypt_collection_name_get) | **GET** /v1/decrypt/{collection_name} | Decrypt Record Route
[**delete_organization_route_v1_organization_organization_id_delete**](RecordsApi.md#delete_organization_route_v1_organization_organization_id_delete) | **DELETE** /v1/organization/{organization_id} | Delete Organization Route
[**delete_record_api_v1_object_collection_name_object_id_delete**](RecordsApi.md#delete_record_api_v1_object_collection_name_object_id_delete) | **DELETE** /v1/object/{collection_name}/{object_id} | Delete Record Api
[**delete_records_api_v1_object_collection_name_delete**](RecordsApi.md#delete_records_api_v1_object_collection_name_delete) | **DELETE** /v1/object/{collection_name} | Delete Records Api
[**export_records_api_v1_object_export_post**](RecordsApi.md#export_records_api_v1_object_export_post) | **POST** /v1/object/export | Export Records Api
[**import_records_api_v1_object_collection_name_import_post**](RecordsApi.md#import_records_api_v1_object_collection_name_import_post) | **POST** /v1/object/{collection_name}/import | Import Records Api
[**merge_records_api_v1_merge_post**](RecordsApi.md#merge_records_api_v1_merge_post) | **POST** /v1/merge | Merge Records Api
[**update_records_api_v1_object_collection_name_patch**](RecordsApi.md#update_records_api_v1_object_collection_name_patch) | **PATCH** /v1/object/{collection_name} | Update Records Api


# **create_records_api_v1_object_collection_name_post**
> object create_records_api_v1_object_collection_name_post(collection_name, data)

Create Records Api

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.data import Data
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
    api_instance = valstorm_api.RecordsApi(api_client)
    collection_name = 'collection_name_example' # str | 
    data = valstorm_api.Data() # Data | 

    try:
        # Create Records Api
        api_response = api_instance.create_records_api_v1_object_collection_name_post(collection_name, data)
        print("The response of RecordsApi->create_records_api_v1_object_collection_name_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->create_records_api_v1_object_collection_name_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **collection_name** | **str**|  | 
 **data** | [**Data**](Data.md)|  | 

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

# **csv_to_json_v1_csv_to_json_post**
> object csv_to_json_v1_csv_to_json_post(files)

Csv To Json

Convert uploaded CSV file to JSON format.

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
    api_instance = valstorm_api.RecordsApi(api_client)
    files = ['files_example'] # List[str] | 

    try:
        # Csv To Json
        api_response = api_instance.csv_to_json_v1_csv_to_json_post(files)
        print("The response of RecordsApi->csv_to_json_v1_csv_to_json_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->csv_to_json_v1_csv_to_json_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **files** | [**List[str]**](str.md)|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **decrypt_record_route_v1_decrypt_collection_name_get**
> object decrypt_record_route_v1_decrypt_collection_name_get(collection_name, record_id, var_field)

Decrypt Record Route

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
    api_instance = valstorm_api.RecordsApi(api_client)
    collection_name = 'collection_name_example' # str | 
    record_id = 'record_id_example' # str | 
    var_field = 'var_field_example' # str | 

    try:
        # Decrypt Record Route
        api_response = api_instance.decrypt_record_route_v1_decrypt_collection_name_get(collection_name, record_id, var_field)
        print("The response of RecordsApi->decrypt_record_route_v1_decrypt_collection_name_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->decrypt_record_route_v1_decrypt_collection_name_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **collection_name** | **str**|  | 
 **record_id** | **str**|  | 
 **var_field** | **str**|  | 

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

# **delete_organization_route_v1_organization_organization_id_delete**
> object delete_organization_route_v1_organization_organization_id_delete(organization_id)

Delete Organization Route

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
    api_instance = valstorm_api.RecordsApi(api_client)
    organization_id = 'organization_id_example' # str | 

    try:
        # Delete Organization Route
        api_response = api_instance.delete_organization_route_v1_organization_organization_id_delete(organization_id)
        print("The response of RecordsApi->delete_organization_route_v1_organization_organization_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->delete_organization_route_v1_organization_organization_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organization_id** | **str**|  | 

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

# **delete_record_api_v1_object_collection_name_object_id_delete**
> object delete_record_api_v1_object_collection_name_object_id_delete(collection_name, object_id)

Delete Record Api

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
    api_instance = valstorm_api.RecordsApi(api_client)
    collection_name = 'collection_name_example' # str | 
    object_id = 'object_id_example' # str | 

    try:
        # Delete Record Api
        api_response = api_instance.delete_record_api_v1_object_collection_name_object_id_delete(collection_name, object_id)
        print("The response of RecordsApi->delete_record_api_v1_object_collection_name_object_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->delete_record_api_v1_object_collection_name_object_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **collection_name** | **str**|  | 
 **object_id** | **str**|  | 

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

# **delete_records_api_v1_object_collection_name_delete**
> object delete_records_api_v1_object_collection_name_delete(collection_name)

Delete Records Api

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
    api_instance = valstorm_api.RecordsApi(api_client)
    collection_name = 'collection_name_example' # str | 

    try:
        # Delete Records Api
        api_response = api_instance.delete_records_api_v1_object_collection_name_delete(collection_name)
        print("The response of RecordsApi->delete_records_api_v1_object_collection_name_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->delete_records_api_v1_object_collection_name_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **collection_name** | **str**|  | 

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

# **export_records_api_v1_object_export_post**
> object export_records_api_v1_object_export_post(export_records_request)

Export Records Api

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.export_records_request import ExportRecordsRequest
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
    api_instance = valstorm_api.RecordsApi(api_client)
    export_records_request = valstorm_api.ExportRecordsRequest() # ExportRecordsRequest | 

    try:
        # Export Records Api
        api_response = api_instance.export_records_api_v1_object_export_post(export_records_request)
        print("The response of RecordsApi->export_records_api_v1_object_export_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->export_records_api_v1_object_export_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **export_records_request** | [**ExportRecordsRequest**](ExportRecordsRequest.md)|  | 

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

# **import_records_api_v1_object_collection_name_import_post**
> object import_records_api_v1_object_collection_name_import_post(collection_name, file, operation=operation)

Import Records Api

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
    api_instance = valstorm_api.RecordsApi(api_client)
    collection_name = 'collection_name_example' # str | 
    file = 'file_example' # str | 
    operation = 'operation_example' # str |  (optional)

    try:
        # Import Records Api
        api_response = api_instance.import_records_api_v1_object_collection_name_import_post(collection_name, file, operation=operation)
        print("The response of RecordsApi->import_records_api_v1_object_collection_name_import_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->import_records_api_v1_object_collection_name_import_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **collection_name** | **str**|  | 
 **file** | **str**|  | 
 **operation** | **str**|  | [optional] 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **merge_records_api_v1_merge_post**
> object merge_records_api_v1_merge_post(merge_records_request, background_task=background_task)

Merge Records Api

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.merge_records_request import MergeRecordsRequest
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
    api_instance = valstorm_api.RecordsApi(api_client)
    merge_records_request = valstorm_api.MergeRecordsRequest() # MergeRecordsRequest | 
    background_task = None # object |  (optional)

    try:
        # Merge Records Api
        api_response = api_instance.merge_records_api_v1_merge_post(merge_records_request, background_task=background_task)
        print("The response of RecordsApi->merge_records_api_v1_merge_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->merge_records_api_v1_merge_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **merge_records_request** | [**MergeRecordsRequest**](MergeRecordsRequest.md)|  | 
 **background_task** | [**object**](.md)|  | [optional] 

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

# **update_records_api_v1_object_collection_name_patch**
> object update_records_api_v1_object_collection_name_patch(collection_name, data)

Update Records Api

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.data import Data
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
    api_instance = valstorm_api.RecordsApi(api_client)
    collection_name = 'collection_name_example' # str | 
    data = valstorm_api.Data() # Data | 

    try:
        # Update Records Api
        api_response = api_instance.update_records_api_v1_object_collection_name_patch(collection_name, data)
        print("The response of RecordsApi->update_records_api_v1_object_collection_name_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordsApi->update_records_api_v1_object_collection_name_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **collection_name** | **str**|  | 
 **data** | [**Data**](Data.md)|  | 

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


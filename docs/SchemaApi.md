# valstorm_api.SchemaApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_schema_field_v1_schema_field_post**](SchemaApi.md#create_schema_field_v1_schema_field_post) | **POST** /v1/schema/field | Create Schema Field
[**create_schema_v1_schema_post**](SchemaApi.md#create_schema_v1_schema_post) | **POST** /v1/schema | Create Schema
[**delete_schema_field_v1_schema_object_id_field_name_delete**](SchemaApi.md#delete_schema_field_v1_schema_object_id_field_name_delete) | **DELETE** /v1/schema/{object_id}/{field_name} | Delete Schema Field
[**delete_schema_route_v1_schema_schema_id_delete**](SchemaApi.md#delete_schema_route_v1_schema_schema_id_delete) | **DELETE** /v1/schema/{schema_id} | Delete Schema Route
[**generate_schema_v1_schema_generate_post**](SchemaApi.md#generate_schema_v1_schema_generate_post) | **POST** /v1/schema/generate/ | Generate Schema
[**get_schema_v1_schema_object_get**](SchemaApi.md#get_schema_v1_schema_object_get) | **GET** /v1/schema/{object} | Get Schema
[**get_schemas_v1_schemas_get**](SchemaApi.md#get_schemas_v1_schemas_get) | **GET** /v1/schemas | Get Schemas
[**update_schema_field_v1_schema_field_patch**](SchemaApi.md#update_schema_field_v1_schema_field_patch) | **PATCH** /v1/schema/field | Update Schema Field
[**update_schema_v1_schema_patch**](SchemaApi.md#update_schema_v1_schema_patch) | **PATCH** /v1/schema | Update Schema


# **create_schema_field_v1_schema_field_post**
> object create_schema_field_v1_schema_field_post(field_create_update_request)

Create Schema Field

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.field_create_update_request import FieldCreateUpdateRequest
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
    api_instance = valstorm_api.SchemaApi(api_client)
    field_create_update_request = valstorm_api.FieldCreateUpdateRequest() # FieldCreateUpdateRequest | 

    try:
        # Create Schema Field
        api_response = api_instance.create_schema_field_v1_schema_field_post(field_create_update_request)
        print("The response of SchemaApi->create_schema_field_v1_schema_field_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SchemaApi->create_schema_field_v1_schema_field_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **field_create_update_request** | [**FieldCreateUpdateRequest**](FieldCreateUpdateRequest.md)|  | 

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

# **create_schema_v1_schema_post**
> object create_schema_v1_schema_post(schema_create_request)

Create Schema

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.schema_create_request import SchemaCreateRequest
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
    api_instance = valstorm_api.SchemaApi(api_client)
    schema_create_request = valstorm_api.SchemaCreateRequest() # SchemaCreateRequest | 

    try:
        # Create Schema
        api_response = api_instance.create_schema_v1_schema_post(schema_create_request)
        print("The response of SchemaApi->create_schema_v1_schema_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SchemaApi->create_schema_v1_schema_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **schema_create_request** | [**SchemaCreateRequest**](SchemaCreateRequest.md)|  | 

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

# **delete_schema_field_v1_schema_object_id_field_name_delete**
> object delete_schema_field_v1_schema_object_id_field_name_delete(object_id, field_name)

Delete Schema Field

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
    api_instance = valstorm_api.SchemaApi(api_client)
    object_id = 'object_id_example' # str | 
    field_name = 'field_name_example' # str | 

    try:
        # Delete Schema Field
        api_response = api_instance.delete_schema_field_v1_schema_object_id_field_name_delete(object_id, field_name)
        print("The response of SchemaApi->delete_schema_field_v1_schema_object_id_field_name_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SchemaApi->delete_schema_field_v1_schema_object_id_field_name_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_id** | **str**|  | 
 **field_name** | **str**|  | 

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

# **delete_schema_route_v1_schema_schema_id_delete**
> object delete_schema_route_v1_schema_schema_id_delete(schema_id)

Delete Schema Route

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
    api_instance = valstorm_api.SchemaApi(api_client)
    schema_id = 'schema_id_example' # str | 

    try:
        # Delete Schema Route
        api_response = api_instance.delete_schema_route_v1_schema_schema_id_delete(schema_id)
        print("The response of SchemaApi->delete_schema_route_v1_schema_schema_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SchemaApi->delete_schema_route_v1_schema_schema_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **schema_id** | **str**|  | 

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

# **generate_schema_v1_schema_generate_post**
> object generate_schema_v1_schema_generate_post()

Generate Schema

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
    api_instance = valstorm_api.SchemaApi(api_client)

    try:
        # Generate Schema
        api_response = api_instance.generate_schema_v1_schema_generate_post()
        print("The response of SchemaApi->generate_schema_v1_schema_generate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SchemaApi->generate_schema_v1_schema_generate_post: %s\n" % e)
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

# **get_schema_v1_schema_object_get**
> object get_schema_v1_schema_object_get(object)

Get Schema

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
    api_instance = valstorm_api.SchemaApi(api_client)
    object = 'object_example' # str | 

    try:
        # Get Schema
        api_response = api_instance.get_schema_v1_schema_object_get(object)
        print("The response of SchemaApi->get_schema_v1_schema_object_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SchemaApi->get_schema_v1_schema_object_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object** | **str**|  | 

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

# **get_schemas_v1_schemas_get**
> object get_schemas_v1_schemas_get()

Get Schemas

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
    api_instance = valstorm_api.SchemaApi(api_client)

    try:
        # Get Schemas
        api_response = api_instance.get_schemas_v1_schemas_get()
        print("The response of SchemaApi->get_schemas_v1_schemas_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SchemaApi->get_schemas_v1_schemas_get: %s\n" % e)
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

# **update_schema_field_v1_schema_field_patch**
> object update_schema_field_v1_schema_field_patch(field_create_update_request)

Update Schema Field

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.field_create_update_request import FieldCreateUpdateRequest
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
    api_instance = valstorm_api.SchemaApi(api_client)
    field_create_update_request = valstorm_api.FieldCreateUpdateRequest() # FieldCreateUpdateRequest | 

    try:
        # Update Schema Field
        api_response = api_instance.update_schema_field_v1_schema_field_patch(field_create_update_request)
        print("The response of SchemaApi->update_schema_field_v1_schema_field_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SchemaApi->update_schema_field_v1_schema_field_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **field_create_update_request** | [**FieldCreateUpdateRequest**](FieldCreateUpdateRequest.md)|  | 

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

# **update_schema_v1_schema_patch**
> update_schema_v1_schema_patch(schema_update_request)

Update Schema

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.schema_update_request import SchemaUpdateRequest
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
    api_instance = valstorm_api.SchemaApi(api_client)
    schema_update_request = valstorm_api.SchemaUpdateRequest() # SchemaUpdateRequest | 

    try:
        # Update Schema
        api_instance.update_schema_v1_schema_patch(schema_update_request)
    except Exception as e:
        print("Exception when calling SchemaApi->update_schema_v1_schema_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **schema_update_request** | [**SchemaUpdateRequest**](SchemaUpdateRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


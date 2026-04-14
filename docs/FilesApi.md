# valstorm_api.FilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_file_route_v1_files_file_id_delete**](FilesApi.md#delete_file_route_v1_files_file_id_delete) | **DELETE** /v1/files/{file_id} | Delete File Route
[**generate_file_access_token_v1_files_token_post**](FilesApi.md#generate_file_access_token_v1_files_token_post) | **POST** /v1/files/token | Generate File Access Token
[**get_file_by_location_v1_files_location_post**](FilesApi.md#get_file_by_location_v1_files_location_post) | **POST** /v1/files/location | Get File By Location
[**get_file_route_v1_files_file_id_get**](FilesApi.md#get_file_route_v1_files_file_id_get) | **GET** /v1/files/{file_id} | Get File Route
[**stream_file_by_location_v1_files_stream_get**](FilesApi.md#stream_file_by_location_v1_files_stream_get) | **GET** /v1/files/stream | Stream File By Location
[**upload_files_route_v1_files_post**](FilesApi.md#upload_files_route_v1_files_post) | **POST** /v1/files | Upload Files Route


# **delete_file_route_v1_files_file_id_delete**
> object delete_file_route_v1_files_file_id_delete(file_id)

Delete File Route

Deletes a file from DB and S3 via the service layer.

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
    api_instance = valstorm_api.FilesApi(api_client)
    file_id = 'file_id_example' # str | 

    try:
        # Delete File Route
        api_response = api_instance.delete_file_route_v1_files_file_id_delete(file_id)
        print("The response of FilesApi->delete_file_route_v1_files_file_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->delete_file_route_v1_files_file_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file_id** | **str**|  | 

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

# **generate_file_access_token_v1_files_token_post**
> object generate_file_access_token_v1_files_token_post()

Generate File Access Token

Generates a short-lived (5 min) access token.
Used by the frontend to construct authorized video stream URLs.

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
    api_instance = valstorm_api.FilesApi(api_client)

    try:
        # Generate File Access Token
        api_response = api_instance.generate_file_access_token_v1_files_token_post()
        print("The response of FilesApi->generate_file_access_token_v1_files_token_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->generate_file_access_token_v1_files_token_post: %s\n" % e)
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

# **get_file_by_location_v1_files_location_post**
> object get_file_by_location_v1_files_location_post(get_file)

Get File By Location

Streams a file directly from S3 given its full location key.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.get_file import GetFile
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
    api_instance = valstorm_api.FilesApi(api_client)
    get_file = valstorm_api.GetFile() # GetFile | 

    try:
        # Get File By Location
        api_response = api_instance.get_file_by_location_v1_files_location_post(get_file)
        print("The response of FilesApi->get_file_by_location_v1_files_location_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->get_file_by_location_v1_files_location_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **get_file** | [**GetFile**](GetFile.md)|  | 

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

# **get_file_route_v1_files_file_id_get**
> object get_file_route_v1_files_file_id_get(file_id)

Get File Route

Finds a file by its ID in the database and streams it from S3.

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
    api_instance = valstorm_api.FilesApi(api_client)
    file_id = 'file_id_example' # str | 

    try:
        # Get File Route
        api_response = api_instance.get_file_route_v1_files_file_id_get(file_id)
        print("The response of FilesApi->get_file_route_v1_files_file_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->get_file_route_v1_files_file_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file_id** | **str**|  | 

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

# **stream_file_by_location_v1_files_stream_get**
> object stream_file_by_location_v1_files_stream_get(location, token, range=range)

Stream File By Location

Streams a file for HTML5 Video tags.
Supports Range requests (Seeking/Skipping).

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
    api_instance = valstorm_api.FilesApi(api_client)
    location = 'location_example' # str | 
    token = 'token_example' # str | 
    range = 'range_example' # str |  (optional)

    try:
        # Stream File By Location
        api_response = api_instance.stream_file_by_location_v1_files_stream_get(location, token, range=range)
        print("The response of FilesApi->stream_file_by_location_v1_files_stream_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->stream_file_by_location_v1_files_stream_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **str**|  | 
 **token** | **str**|  | 
 **range** | **str**|  | [optional] 

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

# **upload_files_route_v1_files_post**
> object upload_files_route_v1_files_post(files, public_file=public_file, compression_config=compression_config)

Upload Files Route

Handles multiple file uploads.
Delegates complex video processing and S3 logic to the service layer.

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
    api_instance = valstorm_api.FilesApi(api_client)
    files = ['files_example'] # List[str] | 
    public_file = False # bool |  (optional) (default to False)
    compression_config = 'compression_config_example' # str |  (optional)

    try:
        # Upload Files Route
        api_response = api_instance.upload_files_route_v1_files_post(files, public_file=public_file, compression_config=compression_config)
        print("The response of FilesApi->upload_files_route_v1_files_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->upload_files_route_v1_files_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **files** | [**List[str]**](str.md)|  | 
 **public_file** | **bool**|  | [optional] [default to False]
 **compression_config** | **str**|  | [optional] 

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


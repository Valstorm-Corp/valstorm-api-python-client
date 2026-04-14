# valstorm_api.PublicApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_app_products_v1_public_app_products_get**](PublicApi.md#get_app_products_v1_public_app_products_get) | **GET** /v1/public/app-products | Get App Products
[**get_apps_v1_public_apps_get**](PublicApi.md#get_apps_v1_public_apps_get) | **GET** /v1/public/apps | Get Apps
[**get_org_blog_v1_public_blog_organization_id_get**](PublicApi.md#get_org_blog_v1_public_blog_organization_id_get) | **GET** /v1/public/blog/{organization_id} | Get Org Blog
[**get_org_marketing_v1_public_marketing_organization_id_get**](PublicApi.md#get_org_marketing_v1_public_marketing_organization_id_get) | **GET** /v1/public/marketing/{organization_id} | Get Org Marketing
[**get_pages_v1_public_pages_org_name_get**](PublicApi.md#get_pages_v1_public_pages_org_name_get) | **GET** /v1/public/pages/{org_name} | Get Pages
[**get_products_v1_public_products_org_name_get**](PublicApi.md#get_products_v1_public_products_org_name_get) | **GET** /v1/public/products/{org_name} | Get Products
[**get_public_docs_v1_public_docs_get**](PublicApi.md#get_public_docs_v1_public_docs_get) | **GET** /v1/public/docs | Get Public Docs
[**get_public_marketing_v1_public_marketing_get**](PublicApi.md#get_public_marketing_v1_public_marketing_get) | **GET** /v1/public/marketing | Get Public Marketing
[**post_query_v1_public_query_object_name_org_name_post**](PublicApi.md#post_query_v1_public_query_object_name_org_name_post) | **POST** /v1/public/query/{object_name}/{org_name} | Post Query
[**question_route_v1_public_question_post**](PublicApi.md#question_route_v1_public_question_post) | **POST** /v1/public/question | Question Route
[**search_public_docs_v1_public_docs_organization_id_search_get**](PublicApi.md#search_public_docs_v1_public_docs_organization_id_search_get) | **GET** /v1/public/docs/{organization_id}/search | Search Public Docs


# **get_app_products_v1_public_app_products_get**
> object get_app_products_v1_public_app_products_get()

Get App Products

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
    api_instance = valstorm_api.PublicApi(api_client)

    try:
        # Get App Products
        api_response = api_instance.get_app_products_v1_public_app_products_get()
        print("The response of PublicApi->get_app_products_v1_public_app_products_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->get_app_products_v1_public_app_products_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_apps_v1_public_apps_get**
> object get_apps_v1_public_apps_get()

Get Apps

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
    api_instance = valstorm_api.PublicApi(api_client)

    try:
        # Get Apps
        api_response = api_instance.get_apps_v1_public_apps_get()
        print("The response of PublicApi->get_apps_v1_public_apps_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->get_apps_v1_public_apps_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_org_blog_v1_public_blog_organization_id_get**
> object get_org_blog_v1_public_blog_organization_id_get(organization_id)

Get Org Blog

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
    api_instance = valstorm_api.PublicApi(api_client)
    organization_id = 'organization_id_example' # str | 

    try:
        # Get Org Blog
        api_response = api_instance.get_org_blog_v1_public_blog_organization_id_get(organization_id)
        print("The response of PublicApi->get_org_blog_v1_public_blog_organization_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->get_org_blog_v1_public_blog_organization_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organization_id** | **str**|  | 

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

# **get_org_marketing_v1_public_marketing_organization_id_get**
> object get_org_marketing_v1_public_marketing_organization_id_get(organization_id)

Get Org Marketing

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
    api_instance = valstorm_api.PublicApi(api_client)
    organization_id = 'organization_id_example' # str | 

    try:
        # Get Org Marketing
        api_response = api_instance.get_org_marketing_v1_public_marketing_organization_id_get(organization_id)
        print("The response of PublicApi->get_org_marketing_v1_public_marketing_organization_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->get_org_marketing_v1_public_marketing_organization_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organization_id** | **str**|  | 

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

# **get_pages_v1_public_pages_org_name_get**
> object get_pages_v1_public_pages_org_name_get(org_name)

Get Pages

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
    api_instance = valstorm_api.PublicApi(api_client)
    org_name = 'org_name_example' # str | 

    try:
        # Get Pages
        api_response = api_instance.get_pages_v1_public_pages_org_name_get(org_name)
        print("The response of PublicApi->get_pages_v1_public_pages_org_name_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->get_pages_v1_public_pages_org_name_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_name** | **str**|  | 

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

# **get_products_v1_public_products_org_name_get**
> object get_products_v1_public_products_org_name_get(org_name)

Get Products

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
    api_instance = valstorm_api.PublicApi(api_client)
    org_name = 'org_name_example' # str | 

    try:
        # Get Products
        api_response = api_instance.get_products_v1_public_products_org_name_get(org_name)
        print("The response of PublicApi->get_products_v1_public_products_org_name_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->get_products_v1_public_products_org_name_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_name** | **str**|  | 

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

# **get_public_docs_v1_public_docs_get**
> object get_public_docs_v1_public_docs_get()

Get Public Docs

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
    api_instance = valstorm_api.PublicApi(api_client)

    try:
        # Get Public Docs
        api_response = api_instance.get_public_docs_v1_public_docs_get()
        print("The response of PublicApi->get_public_docs_v1_public_docs_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->get_public_docs_v1_public_docs_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_public_marketing_v1_public_marketing_get**
> object get_public_marketing_v1_public_marketing_get()

Get Public Marketing

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
    api_instance = valstorm_api.PublicApi(api_client)

    try:
        # Get Public Marketing
        api_response = api_instance.get_public_marketing_v1_public_marketing_get()
        print("The response of PublicApi->get_public_marketing_v1_public_marketing_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->get_public_marketing_v1_public_marketing_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_query_v1_public_query_object_name_org_name_post**
> object post_query_v1_public_query_object_name_org_name_post(object_name, org_name, request_body)

Post Query

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
    api_instance = valstorm_api.PublicApi(api_client)
    object_name = 'object_name_example' # str | 
    org_name = 'org_name_example' # str | 
    request_body = None # Dict[str, object] | 

    try:
        # Post Query
        api_response = api_instance.post_query_v1_public_query_object_name_org_name_post(object_name, org_name, request_body)
        print("The response of PublicApi->post_query_v1_public_query_object_name_org_name_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->post_query_v1_public_query_object_name_org_name_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_name** | **str**|  | 
 **org_name** | **str**|  | 
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

# **question_route_v1_public_question_post**
> object question_route_v1_public_question_post(request_body)

Question Route

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
    api_instance = valstorm_api.PublicApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Question Route
        api_response = api_instance.question_route_v1_public_question_post(request_body)
        print("The response of PublicApi->question_route_v1_public_question_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->question_route_v1_public_question_post: %s\n" % e)
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

# **search_public_docs_v1_public_docs_organization_id_search_get**
> object search_public_docs_v1_public_docs_organization_id_search_get(organization_id, q=q)

Search Public Docs

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
    api_instance = valstorm_api.PublicApi(api_client)
    organization_id = 'organization_id_example' # str | 
    q = '' # str |  (optional) (default to '')

    try:
        # Search Public Docs
        api_response = api_instance.search_public_docs_v1_public_docs_organization_id_search_get(organization_id, q=q)
        print("The response of PublicApi->search_public_docs_v1_public_docs_organization_id_search_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->search_public_docs_v1_public_docs_organization_id_search_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organization_id** | **str**|  | 
 **q** | **str**|  | [optional] [default to &#39;&#39;]

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


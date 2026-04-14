# valstorm_api.QueryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**mongo_query_route_v2_v1_query_mongo_post**](QueryApi.md#mongo_query_route_v2_v1_query_mongo_post) | **POST** /v1/query/mongo | Mongo Query Route V2
[**sql_query_post_route_v1_query_post**](QueryApi.md#sql_query_post_route_v1_query_post) | **POST** /v1/query | Sql Query Post Route
[**sql_query_route_v1_query_get**](QueryApi.md#sql_query_route_v1_query_get) | **GET** /v1/query | Sql Query Route


# **mongo_query_route_v2_v1_query_mongo_post**
> object mongo_query_route_v2_v1_query_mongo_post(mongo_query_request)

Mongo Query Route V2

Direct MongoDB Aggregation Endpoint (V2) - Async
Returns records in body and Pagination Metadata in Headers.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.mongo_query_request import MongoQueryRequest
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
    api_instance = valstorm_api.QueryApi(api_client)
    mongo_query_request = valstorm_api.MongoQueryRequest() # MongoQueryRequest | 

    try:
        # Mongo Query Route V2
        api_response = api_instance.mongo_query_route_v2_v1_query_mongo_post(mongo_query_request)
        print("The response of QueryApi->mongo_query_route_v2_v1_query_mongo_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueryApi->mongo_query_route_v2_v1_query_mongo_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mongo_query_request** | [**MongoQueryRequest**](MongoQueryRequest.md)|  | 

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

# **sql_query_post_route_v1_query_post**
> object sql_query_post_route_v1_query_post(request_body)

Sql Query Post Route

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
    api_instance = valstorm_api.QueryApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Sql Query Post Route
        api_response = api_instance.sql_query_post_route_v1_query_post(request_body)
        print("The response of QueryApi->sql_query_post_route_v1_query_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueryApi->sql_query_post_route_v1_query_post: %s\n" % e)
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

# **sql_query_route_v1_query_get**
> object sql_query_route_v1_query_get()

Sql Query Route

Description
    SQL Query Engine for Valstorm API
Args:
    query (str): SQL query string
    current_user (User, optional): Current authenticated user. Defaults to Depends(get_current_user).
Returns:
    dict: Dictionary containing records and headers
        Examples
        --------

        
        Select All Fields And Records
        SELECT * FROM contact

        Select Specific Fields
        SELECT name, phone FROM Contact

        Where Field Equals
        SELECT name, phone FROM Contact WHERE name = 'Jared Simpson'

        Where LIKE Starts With
        SELECT name, phone, email FROM Contact WHERE name LIKE 'Unk%'

        Where LIKE Ends With
        SELECT name, phone, email FROM Contact WHERE name LIKE '%n'

        Where LIKE Contains
        SELECT name, phone, email FROM Contact WHERE name LIKE '%j%'

        WHERE IN
        SELECT name, phone, email FROM Contact WHERE name IN ['Jared', 'John']

        WHERE OR
        SELECT name, phone, email FROM Contact WHERE name = 'Jared' OR phone = '555-555-5555'

        WHERE AND
        SELECT name, phone, email FROM Contact WHERE name = 'Jared' AND phone = '555-555-5555'

        WHERE LIMIT
        SELECT name, phone, email FROM Contact WHERE name = 'Jared' LIMIT 10

        WHERE ORDER BY DESC
        SELECT name, phone, email FROM Contact WHERE name = 'Jared' ORDER BY phone DESC

        WHERE ORDER BY ASC
        SELECT name, phone, email FROM Contact WHERE name = 'Jared' ORDER BY phone ASC

        ORDER BY MULTIPLE
        SELECT name, phone, email FROM Contact WHERE name = 'Jared' ORDER BY phone ASC, email DESC

        OFFSET
        SELECT name, phone, email FROM Contact WHERE name = 'Jared' OFFSET 10

        Parent to Child JOIN Query
        SELECT first_name, last_name, twilio_message.body, twilio_message.id, twilio_message.direction FROM contact JOIN twilio_message ON contact.id = twilio_message.contact WHERE first_name = 'Jared' ORDER BY twilio_message.created_date DESC LIMIT 10

        Child to Parent Join
        SELECT id, disposition, name, contact.name FROM call JOIN contact ON call.contact = contact.id

        Multi Join
        SELECT id, name, phone, call.*, twilio_message.* FROM contact JOIN call ON contact.id = call.contact JOIN twilio_message ON contact.id = twilio_message.contact WHERE contact.name LIKE '%Jared%' ORDER BY contact.created_at DESC LIMIT 50 OFFSET 0

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
    api_instance = valstorm_api.QueryApi(api_client)

    try:
        # Sql Query Route
        api_response = api_instance.sql_query_route_v1_query_get()
        print("The response of QueryApi->sql_query_route_v1_query_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueryApi->sql_query_route_v1_query_get: %s\n" % e)
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


# valstorm_api.WebsocketsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_websocket_v1_ws_create_get**](WebsocketsApi.md#create_websocket_v1_ws_create_get) | **GET** /v1/ws/create | Create Websocket
[**send_message_route_v1_ws_send_message_post**](WebsocketsApi.md#send_message_route_v1_ws_send_message_post) | **POST** /v1/ws/send_message | Send Message Route


# **create_websocket_v1_ws_create_get**
> object create_websocket_v1_ws_create_get()

Create Websocket

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
    api_instance = valstorm_api.WebsocketsApi(api_client)

    try:
        # Create Websocket
        api_response = api_instance.create_websocket_v1_ws_create_get()
        print("The response of WebsocketsApi->create_websocket_v1_ws_create_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebsocketsApi->create_websocket_v1_ws_create_get: %s\n" % e)
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

# **send_message_route_v1_ws_send_message_post**
> object send_message_route_v1_ws_send_message_post(request_body)

Send Message Route

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
    api_instance = valstorm_api.WebsocketsApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Send Message Route
        api_response = api_instance.send_message_route_v1_ws_send_message_post(request_body)
        print("The response of WebsocketsApi->send_message_route_v1_ws_send_message_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebsocketsApi->send_message_route_v1_ws_send_message_post: %s\n" % e)
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


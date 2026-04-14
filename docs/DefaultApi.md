# valstorm_api.DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_routers_v1_routes_get**](DefaultApi.md#list_routers_v1_routes_get) | **GET** /v1/routes | List Routers


# **list_routers_v1_routes_get**
> object list_routers_v1_routes_get()

List Routers

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
    api_instance = valstorm_api.DefaultApi(api_client)

    try:
        # List Routers
        api_response = api_instance.list_routers_v1_routes_get()
        print("The response of DefaultApi->list_routers_v1_routes_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->list_routers_v1_routes_get: %s\n" % e)
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


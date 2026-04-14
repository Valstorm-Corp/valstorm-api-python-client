# valstorm_api.ApplyAppsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apply_apps_route_v1_apps_apply_apps_post**](ApplyAppsApi.md#apply_apps_route_v1_apps_apply_apps_post) | **POST** /v1/apps/apply-apps | Apply Apps Route


# **apply_apps_route_v1_apps_apply_apps_post**
> object apply_apps_route_v1_apps_apply_apps_post(request_body)

Apply Apps Route

Bulk installs a list of Apps by ID.

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
    api_instance = valstorm_api.ApplyAppsApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Apply Apps Route
        api_response = api_instance.apply_apps_route_v1_apps_apply_apps_post(request_body)
        print("The response of ApplyAppsApi->apply_apps_route_v1_apps_apply_apps_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplyAppsApi->apply_apps_route_v1_apps_apply_apps_post: %s\n" % e)
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
**201** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


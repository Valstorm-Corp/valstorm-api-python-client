# valstorm_api.DeployAppsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_update_subscribers_v1_apps_app_update_subscribers_post**](DeployAppsApi.md#app_update_subscribers_v1_apps_app_update_subscribers_post) | **POST** /v1/apps/app-update-subscribers | App Update Subscribers
[**deploy_app_v1_apps_deploy_app_id_get**](DeployAppsApi.md#deploy_app_v1_apps_deploy_app_id_get) | **GET** /v1/apps/deploy/{app_id} | Deploy App
[**marketplace_deployment_v1_apps_marketplace_deployment_post**](DeployAppsApi.md#marketplace_deployment_v1_apps_marketplace_deployment_post) | **POST** /v1/apps/marketplace-deployment | Marketplace Deployment
[**receive_app_deploy_v1_apps_deploy_put**](DeployAppsApi.md#receive_app_deploy_v1_apps_deploy_put) | **PUT** /v1/apps/deploy | Receive App Deploy


# **app_update_subscribers_v1_apps_app_update_subscribers_post**
> object app_update_subscribers_v1_apps_app_update_subscribers_post(request_body)

App Update Subscribers

Updates all organizations that are subscribed to the provided App.

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
    api_instance = valstorm_api.DeployAppsApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # App Update Subscribers
        api_response = api_instance.app_update_subscribers_v1_apps_app_update_subscribers_post(request_body)
        print("The response of DeployAppsApi->app_update_subscribers_v1_apps_app_update_subscribers_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeployAppsApi->app_update_subscribers_v1_apps_app_update_subscribers_post: %s\n" % e)
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

# **deploy_app_v1_apps_deploy_app_id_get**
> object deploy_app_v1_apps_deploy_app_id_get(app_id)

Deploy App

Triggers a deployment by sending the App Data to the CICD service.
(This logic mostly remains the same as it's an outbound HTTP call, not an internal sync)

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
    api_instance = valstorm_api.DeployAppsApi(api_client)
    app_id = 'app_id_example' # str | 

    try:
        # Deploy App
        api_response = api_instance.deploy_app_v1_apps_deploy_app_id_get(app_id)
        print("The response of DeployAppsApi->deploy_app_v1_apps_deploy_app_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeployAppsApi->deploy_app_v1_apps_deploy_app_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_id** | **str**|  | 

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

# **marketplace_deployment_v1_apps_marketplace_deployment_post**
> object marketplace_deployment_v1_apps_marketplace_deployment_post(request_body)

Marketplace Deployment

Deploys the current app state to the 'Base' database (The Marketplace).

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
    api_instance = valstorm_api.DeployAppsApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Marketplace Deployment
        api_response = api_instance.marketplace_deployment_v1_apps_marketplace_deployment_post(request_body)
        print("The response of DeployAppsApi->marketplace_deployment_v1_apps_marketplace_deployment_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeployAppsApi->marketplace_deployment_v1_apps_marketplace_deployment_post: %s\n" % e)
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

# **receive_app_deploy_v1_apps_deploy_put**
> object receive_app_deploy_v1_apps_deploy_put(request_body)

Receive App Deploy

Receives an app package from CICD and deploys it to the Current User's Organization.

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
    api_instance = valstorm_api.DeployAppsApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Receive App Deploy
        api_response = api_instance.receive_app_deploy_v1_apps_deploy_put(request_body)
        print("The response of DeployAppsApi->receive_app_deploy_v1_apps_deploy_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeployAppsApi->receive_app_deploy_v1_apps_deploy_put: %s\n" % e)
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


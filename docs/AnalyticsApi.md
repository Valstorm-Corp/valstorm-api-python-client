# valstorm_api.AnalyticsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**report_frontend_v1_analytics_report_post**](AnalyticsApi.md#report_frontend_v1_analytics_report_post) | **POST** /v1/analytics/report | Report Frontend


# **report_frontend_v1_analytics_report_post**
> object report_frontend_v1_analytics_report_post(data1)

Report Frontend

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.data1 import Data1
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
    api_instance = valstorm_api.AnalyticsApi(api_client)
    data1 = valstorm_api.Data1() # Data1 | 

    try:
        # Report Frontend
        api_response = api_instance.report_frontend_v1_analytics_report_post(data1)
        print("The response of AnalyticsApi->report_frontend_v1_analytics_report_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsApi->report_frontend_v1_analytics_report_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data1** | [**Data1**](Data1.md)|  | 

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


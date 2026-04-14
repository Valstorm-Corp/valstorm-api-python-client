# valstorm_api.AlertsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**send_email_v1_alerts_email_post**](AlertsApi.md#send_email_v1_alerts_email_post) | **POST** /v1/alerts/email | Send Email


# **send_email_v1_alerts_email_post**
> object send_email_v1_alerts_email_post(email_template)

Send Email

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.email_template import EmailTemplate
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
    api_instance = valstorm_api.AlertsApi(api_client)
    email_template = valstorm_api.EmailTemplate() # EmailTemplate | 

    try:
        # Send Email
        api_response = api_instance.send_email_v1_alerts_email_post(email_template)
        print("The response of AlertsApi->send_email_v1_alerts_email_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlertsApi->send_email_v1_alerts_email_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_template** | [**EmailTemplate**](EmailTemplate.md)|  | 

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


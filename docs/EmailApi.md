# valstorm_api.EmailApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_message_details_v1_email_services_sendgrid_messages_message_id_post**](EmailApi.md#get_message_details_v1_email_services_sendgrid_messages_message_id_post) | **POST** /v1/email-services/sendgrid/messages/{message_id} | Get Message Details
[**search_messages_v1_email_services_sendgrid_messages_search_post**](EmailApi.md#search_messages_v1_email_services_sendgrid_messages_search_post) | **POST** /v1/email-services/sendgrid/messages/search | Search Messages
[**send_email_v1_email_services_sendgrid_send_post**](EmailApi.md#send_email_v1_email_services_sendgrid_send_post) | **POST** /v1/email-services/sendgrid/send | Send Email
[**sendgrid_webhook_v1_email_services_sendgrid_webhook_organization_id_post**](EmailApi.md#sendgrid_webhook_v1_email_services_sendgrid_webhook_organization_id_post) | **POST** /v1/email-services/sendgrid/webhook/{organization_id} | Sendgrid Webhook
[**validate_email_v1_email_services_validate_email_post**](EmailApi.md#validate_email_v1_email_services_validate_email_post) | **POST** /v1/email-services/validate-email | Validate Email


# **get_message_details_v1_email_services_sendgrid_messages_message_id_post**
> Dict[str, object] get_message_details_v1_email_services_sendgrid_messages_message_id_post(message_id)

Get Message Details

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
    api_instance = valstorm_api.EmailApi(api_client)
    message_id = 'message_id_example' # str | 

    try:
        # Get Message Details
        api_response = api_instance.get_message_details_v1_email_services_sendgrid_messages_message_id_post(message_id)
        print("The response of EmailApi->get_message_details_v1_email_services_sendgrid_messages_message_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->get_message_details_v1_email_services_sendgrid_messages_message_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**|  | 

### Return type

**Dict[str, object]**

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

# **search_messages_v1_email_services_sendgrid_messages_search_post**
> Dict[str, object] search_messages_v1_email_services_sendgrid_messages_search_post(email_log_search_request=email_log_search_request)

Search Messages

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.email_log_search_request import EmailLogSearchRequest
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
    api_instance = valstorm_api.EmailApi(api_client)
    email_log_search_request = valstorm_api.EmailLogSearchRequest() # EmailLogSearchRequest |  (optional)

    try:
        # Search Messages
        api_response = api_instance.search_messages_v1_email_services_sendgrid_messages_search_post(email_log_search_request=email_log_search_request)
        print("The response of EmailApi->search_messages_v1_email_services_sendgrid_messages_search_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->search_messages_v1_email_services_sendgrid_messages_search_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_log_search_request** | [**EmailLogSearchRequest**](EmailLogSearchRequest.md)|  | [optional] 

### Return type

**Dict[str, object]**

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

# **send_email_v1_email_services_sendgrid_send_post**
> Dict[str, object] send_email_v1_email_services_sendgrid_send_post(send_grid_email_request)

Send Email

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.send_grid_email_request import SendGridEmailRequest
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
    api_instance = valstorm_api.EmailApi(api_client)
    send_grid_email_request = valstorm_api.SendGridEmailRequest() # SendGridEmailRequest | 

    try:
        # Send Email
        api_response = api_instance.send_email_v1_email_services_sendgrid_send_post(send_grid_email_request)
        print("The response of EmailApi->send_email_v1_email_services_sendgrid_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->send_email_v1_email_services_sendgrid_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_grid_email_request** | [**SendGridEmailRequest**](SendGridEmailRequest.md)|  | 

### Return type

**Dict[str, object]**

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

# **sendgrid_webhook_v1_email_services_sendgrid_webhook_organization_id_post**
> sendgrid_webhook_v1_email_services_sendgrid_webhook_organization_id_post(organization_id)

Sendgrid Webhook

Webhook received and being processed

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
    api_instance = valstorm_api.EmailApi(api_client)
    organization_id = 'organization_id_example' # str | 

    try:
        # Sendgrid Webhook
        api_instance.sendgrid_webhook_v1_email_services_sendgrid_webhook_organization_id_post(organization_id)
    except Exception as e:
        print("Exception when calling EmailApi->sendgrid_webhook_v1_email_services_sendgrid_webhook_organization_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organization_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_email_v1_email_services_validate_email_post**
> EmailValidationResponse validate_email_v1_email_services_validate_email_post(email_validation_request)

Validate Email

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.email_validation_request import EmailValidationRequest
from valstorm_api.models.email_validation_response import EmailValidationResponse
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
    api_instance = valstorm_api.EmailApi(api_client)
    email_validation_request = valstorm_api.EmailValidationRequest() # EmailValidationRequest | 

    try:
        # Validate Email
        api_response = api_instance.validate_email_v1_email_services_validate_email_post(email_validation_request)
        print("The response of EmailApi->validate_email_v1_email_services_validate_email_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->validate_email_v1_email_services_validate_email_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_validation_request** | [**EmailValidationRequest**](EmailValidationRequest.md)|  | 

### Return type

[**EmailValidationResponse**](EmailValidationResponse.md)

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


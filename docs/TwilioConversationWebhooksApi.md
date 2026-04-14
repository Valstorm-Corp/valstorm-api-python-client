# valstorm_api.TwilioConversationWebhooksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_conversation_webhooks_v1_twilio_conversation_org_id_post_webhook_post**](TwilioConversationWebhooksApi.md#create_conversation_webhooks_v1_twilio_conversation_org_id_post_webhook_post) | **POST** /v1/twilio/conversation/{org_id}/post-webhook | Create Conversation Webhooks
[**get_conversation_webhooks_v1_twilio_conversation_webhooks_get**](TwilioConversationWebhooksApi.md#get_conversation_webhooks_v1_twilio_conversation_webhooks_get) | **GET** /v1/twilio/conversation/webhooks | Get Conversation Webhooks
[**update_webhook_v1_twilio_conversation_webhooks_post**](TwilioConversationWebhooksApi.md#update_webhook_v1_twilio_conversation_webhooks_post) | **POST** /v1/twilio/conversation/webhooks | Update Webhook


# **create_conversation_webhooks_v1_twilio_conversation_org_id_post_webhook_post**
> object create_conversation_webhooks_v1_twilio_conversation_org_id_post_webhook_post(org_id)

Create Conversation Webhooks

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
    api_instance = valstorm_api.TwilioConversationWebhooksApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Create Conversation Webhooks
        api_response = api_instance.create_conversation_webhooks_v1_twilio_conversation_org_id_post_webhook_post(org_id)
        print("The response of TwilioConversationWebhooksApi->create_conversation_webhooks_v1_twilio_conversation_org_id_post_webhook_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationWebhooksApi->create_conversation_webhooks_v1_twilio_conversation_org_id_post_webhook_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 

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

# **get_conversation_webhooks_v1_twilio_conversation_webhooks_get**
> Webhook get_conversation_webhooks_v1_twilio_conversation_webhooks_get()

Get Conversation Webhooks

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.webhook import Webhook
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
    api_instance = valstorm_api.TwilioConversationWebhooksApi(api_client)

    try:
        # Get Conversation Webhooks
        api_response = api_instance.get_conversation_webhooks_v1_twilio_conversation_webhooks_get()
        print("The response of TwilioConversationWebhooksApi->get_conversation_webhooks_v1_twilio_conversation_webhooks_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationWebhooksApi->get_conversation_webhooks_v1_twilio_conversation_webhooks_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Webhook**](Webhook.md)

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

# **update_webhook_v1_twilio_conversation_webhooks_post**
> Webhook update_webhook_v1_twilio_conversation_webhooks_post()

Update Webhook

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.webhook import Webhook
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
    api_instance = valstorm_api.TwilioConversationWebhooksApi(api_client)

    try:
        # Update Webhook
        api_response = api_instance.update_webhook_v1_twilio_conversation_webhooks_post()
        print("The response of TwilioConversationWebhooksApi->update_webhook_v1_twilio_conversation_webhooks_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwilioConversationWebhooksApi->update_webhook_v1_twilio_conversation_webhooks_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Webhook**](Webhook.md)

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


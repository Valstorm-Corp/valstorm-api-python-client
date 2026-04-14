# valstorm_api.MarketingApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bulk_send_v1_marketing_campaign_bulk_send_post**](MarketingApi.md#bulk_send_v1_marketing_campaign_bulk_send_post) | **POST** /v1/marketing/campaign/bulk-send | Bulk Send
[**csv_to_json_v1_marketing_campaign_csv_to_json_post**](MarketingApi.md#csv_to_json_v1_marketing_campaign_csv_to_json_post) | **POST** /v1/marketing/campaign/csv-to-json | Csv To Json


# **bulk_send_v1_marketing_campaign_bulk_send_post**
> AcceptedResponse bulk_send_v1_marketing_campaign_bulk_send_post(bulk_send)

Bulk Send

Endpoint to send bulk outreach.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.accepted_response import AcceptedResponse
from valstorm_api.models.bulk_send import BulkSend
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
    api_instance = valstorm_api.MarketingApi(api_client)
    bulk_send = valstorm_api.BulkSend() # BulkSend | 

    try:
        # Bulk Send
        api_response = api_instance.bulk_send_v1_marketing_campaign_bulk_send_post(bulk_send)
        print("The response of MarketingApi->bulk_send_v1_marketing_campaign_bulk_send_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketingApi->bulk_send_v1_marketing_campaign_bulk_send_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulk_send** | [**BulkSend**](BulkSend.md)|  | 

### Return type

[**AcceptedResponse**](AcceptedResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **csv_to_json_v1_marketing_campaign_csv_to_json_post**
> object csv_to_json_v1_marketing_campaign_csv_to_json_post(files)

Csv To Json

Convert uploaded CSV file to JSON format.

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
    api_instance = valstorm_api.MarketingApi(api_client)
    files = ['files_example'] # List[str] | 

    try:
        # Csv To Json
        api_response = api_instance.csv_to_json_v1_marketing_campaign_csv_to_json_post(files)
        print("The response of MarketingApi->csv_to_json_v1_marketing_campaign_csv_to_json_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketingApi->csv_to_json_v1_marketing_campaign_csv_to_json_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **files** | [**List[str]**](str.md)|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**404** | Not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


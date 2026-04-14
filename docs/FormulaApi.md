# valstorm_api.FormulaApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**evaluate_formula_v1_formula_evaluate_post**](FormulaApi.md#evaluate_formula_v1_formula_evaluate_post) | **POST** /v1/formula/evaluate | Evaluate Formula


# **evaluate_formula_v1_formula_evaluate_post**
> object evaluate_formula_v1_formula_evaluate_post(evaluate_request)

Evaluate Formula

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.evaluate_request import EvaluateRequest
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
    api_instance = valstorm_api.FormulaApi(api_client)
    evaluate_request = valstorm_api.EvaluateRequest() # EvaluateRequest | 

    try:
        # Evaluate Formula
        api_response = api_instance.evaluate_formula_v1_formula_evaluate_post(evaluate_request)
        print("The response of FormulaApi->evaluate_formula_v1_formula_evaluate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormulaApi->evaluate_formula_v1_formula_evaluate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **evaluate_request** | [**EvaluateRequest**](EvaluateRequest.md)|  | 

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
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


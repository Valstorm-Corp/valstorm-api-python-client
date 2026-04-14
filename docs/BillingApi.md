# valstorm_api.BillingApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_checkout_session_v1_billing_create_checkout_session_post**](BillingApi.md#create_checkout_session_v1_billing_create_checkout_session_post) | **POST** /v1/billing/create-checkout-session | Create Checkout Session
[**create_portal_session_v1_billing_portal_get**](BillingApi.md#create_portal_session_v1_billing_portal_get) | **GET** /v1/billing/portal | Create Portal Session
[**create_registration_checkout_session_v1_billing_create_registration_checkout_session_post**](BillingApi.md#create_registration_checkout_session_v1_billing_create_registration_checkout_session_post) | **POST** /v1/billing/create-registration-checkout-session | Create Registration Checkout Session
[**hooks_route_v1_billing_hooks_post**](BillingApi.md#hooks_route_v1_billing_hooks_post) | **POST** /v1/billing/hooks | Hooks Route
[**session_status_v1_billing_session_status_session_id_product_id_price_id_quantity_get**](BillingApi.md#session_status_v1_billing_session_status_session_id_product_id_price_id_quantity_get) | **GET** /v1/billing/session-status/{session_id}/{product_id}/{price_id}/{quantity} | Session Status


# **create_checkout_session_v1_billing_create_checkout_session_post**
> object create_checkout_session_v1_billing_create_checkout_session_post(stripe_checkout_session)

Create Checkout Session

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import valstorm_api
from valstorm_api.models.stripe_checkout_session import StripeCheckoutSession
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
    api_instance = valstorm_api.BillingApi(api_client)
    stripe_checkout_session = valstorm_api.StripeCheckoutSession() # StripeCheckoutSession | 

    try:
        # Create Checkout Session
        api_response = api_instance.create_checkout_session_v1_billing_create_checkout_session_post(stripe_checkout_session)
        print("The response of BillingApi->create_checkout_session_v1_billing_create_checkout_session_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->create_checkout_session_v1_billing_create_checkout_session_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stripe_checkout_session** | [**StripeCheckoutSession**](StripeCheckoutSession.md)|  | 

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

# **create_portal_session_v1_billing_portal_get**
> object create_portal_session_v1_billing_portal_get()

Create Portal Session

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
    api_instance = valstorm_api.BillingApi(api_client)

    try:
        # Create Portal Session
        api_response = api_instance.create_portal_session_v1_billing_portal_get()
        print("The response of BillingApi->create_portal_session_v1_billing_portal_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->create_portal_session_v1_billing_portal_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_registration_checkout_session_v1_billing_create_registration_checkout_session_post**
> object create_registration_checkout_session_v1_billing_create_registration_checkout_session_post(request_body)

Create Registration Checkout Session

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
    api_instance = valstorm_api.BillingApi(api_client)
    request_body = None # Dict[str, object] | 

    try:
        # Create Registration Checkout Session
        api_response = api_instance.create_registration_checkout_session_v1_billing_create_registration_checkout_session_post(request_body)
        print("The response of BillingApi->create_registration_checkout_session_v1_billing_create_registration_checkout_session_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->create_registration_checkout_session_v1_billing_create_registration_checkout_session_post: %s\n" % e)
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

# **hooks_route_v1_billing_hooks_post**
> object hooks_route_v1_billing_hooks_post()

Hooks Route

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
    api_instance = valstorm_api.BillingApi(api_client)

    try:
        # Hooks Route
        api_response = api_instance.hooks_route_v1_billing_hooks_post()
        print("The response of BillingApi->hooks_route_v1_billing_hooks_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->hooks_route_v1_billing_hooks_post: %s\n" % e)
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

# **session_status_v1_billing_session_status_session_id_product_id_price_id_quantity_get**
> object session_status_v1_billing_session_status_session_id_product_id_price_id_quantity_get(session_id, product_id, price_id, quantity)

Session Status

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
    api_instance = valstorm_api.BillingApi(api_client)
    session_id = 'session_id_example' # str | 
    product_id = 'product_id_example' # str | 
    price_id = 'price_id_example' # str | 
    quantity = 'quantity_example' # str | 

    try:
        # Session Status
        api_response = api_instance.session_status_v1_billing_session_status_session_id_product_id_price_id_quantity_get(session_id, product_id, price_id, quantity)
        print("The response of BillingApi->session_status_v1_billing_session_status_session_id_product_id_price_id_quantity_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->session_status_v1_billing_session_status_session_id_product_id_price_id_quantity_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **session_id** | **str**|  | 
 **product_id** | **str**|  | 
 **price_id** | **str**|  | 
 **quantity** | **str**|  | 

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


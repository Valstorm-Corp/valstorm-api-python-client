# StripeCheckoutSession


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product_id** | **str** |  | 
**price** | **str** |  | 
**quantity** | **str** |  | 
**mode** | **str** |  | [optional] [default to 'subscription']
**trial** | **Dict[str, object]** |  | [optional] 
**return_url** | **bool** |  | [optional] [default to True]
**url** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.stripe_checkout_session import StripeCheckoutSession

# TODO update the JSON string below
json = "{}"
# create an instance of StripeCheckoutSession from a JSON string
stripe_checkout_session_instance = StripeCheckoutSession.from_json(json)
# print the JSON string representation of the object
print(StripeCheckoutSession.to_json())

# convert the object into a dict
stripe_checkout_session_dict = stripe_checkout_session_instance.to_dict()
# create an instance of StripeCheckoutSession from a dict
stripe_checkout_session_from_dict = StripeCheckoutSession.from_dict(stripe_checkout_session_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



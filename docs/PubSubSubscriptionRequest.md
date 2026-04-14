# PubSubSubscriptionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sub_path** | **str** |  | [optional] [default to 'gmail_watcher']
**push_endpoint** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.pub_sub_subscription_request import PubSubSubscriptionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PubSubSubscriptionRequest from a JSON string
pub_sub_subscription_request_instance = PubSubSubscriptionRequest.from_json(json)
# print the JSON string representation of the object
print(PubSubSubscriptionRequest.to_json())

# convert the object into a dict
pub_sub_subscription_request_dict = pub_sub_subscription_request_instance.to_dict()
# create an instance of PubSubSubscriptionRequest from a dict
pub_sub_subscription_request_from_dict = PubSubSubscriptionRequest.from_dict(pub_sub_subscription_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



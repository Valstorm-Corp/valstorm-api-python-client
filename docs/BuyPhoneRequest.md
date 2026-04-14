# BuyPhoneRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**phone_number** | **str** |  | 

## Example

```python
from valstorm_api.models.buy_phone_request import BuyPhoneRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BuyPhoneRequest from a JSON string
buy_phone_request_instance = BuyPhoneRequest.from_json(json)
# print the JSON string representation of the object
print(BuyPhoneRequest.to_json())

# convert the object into a dict
buy_phone_request_dict = buy_phone_request_instance.to_dict()
# create an instance of BuyPhoneRequest from a dict
buy_phone_request_from_dict = BuyPhoneRequest.from_dict(buy_phone_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



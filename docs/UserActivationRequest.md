# UserActivationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activation_code** | **str** |  | 
**password** | **str** |  | 

## Example

```python
from valstorm_api.models.user_activation_request import UserActivationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserActivationRequest from a JSON string
user_activation_request_instance = UserActivationRequest.from_json(json)
# print the JSON string representation of the object
print(UserActivationRequest.to_json())

# convert the object into a dict
user_activation_request_dict = user_activation_request_instance.to_dict()
# create an instance of UserActivationRequest from a dict
user_activation_request_from_dict = UserActivationRequest.from_dict(user_activation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



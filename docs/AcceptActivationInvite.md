# AcceptActivationInvite


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activation_code** | **str** |  | 
**organization_id** | **str** |  | 
**user_id** | **str** |  | 

## Example

```python
from valstorm_api.models.accept_activation_invite import AcceptActivationInvite

# TODO update the JSON string below
json = "{}"
# create an instance of AcceptActivationInvite from a JSON string
accept_activation_invite_instance = AcceptActivationInvite.from_json(json)
# print the JSON string representation of the object
print(AcceptActivationInvite.to_json())

# convert the object into a dict
accept_activation_invite_dict = accept_activation_invite_instance.to_dict()
# create an instance of AcceptActivationInvite from a dict
accept_activation_invite_from_dict = AcceptActivationInvite.from_dict(accept_activation_invite_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



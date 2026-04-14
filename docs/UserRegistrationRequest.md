# UserRegistrationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first_name** | **str** |  | 
**last_name** | **str** |  | 
**email** | **str** |  | 
**phone** | [**Phone**](Phone.md) |  | [optional] 
**organization_id** | **str** |  | [optional] 
**permissions** | **List[str]** |  | [optional] [default to []]
**role** | **Dict[str, object]** |  | [optional] 
**manager** | **Dict[str, object]** |  | [optional] 
**system_user** | **bool** |  | [optional] [default to False]

## Example

```python
from valstorm_api.models.user_registration_request import UserRegistrationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserRegistrationRequest from a JSON string
user_registration_request_instance = UserRegistrationRequest.from_json(json)
# print the JSON string representation of the object
print(UserRegistrationRequest.to_json())

# convert the object into a dict
user_registration_request_dict = user_registration_request_instance.to_dict()
# create an instance of UserRegistrationRequest from a dict
user_registration_request_from_dict = UserRegistrationRequest.from_dict(user_registration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



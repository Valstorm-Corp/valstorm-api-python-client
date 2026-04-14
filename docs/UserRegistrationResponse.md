# UserRegistrationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activation_code** | **str** |  | [optional] 
**user_id** | **str** |  | 
**status** | **str** |  | 

## Example

```python
from valstorm_api.models.user_registration_response import UserRegistrationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserRegistrationResponse from a JSON string
user_registration_response_instance = UserRegistrationResponse.from_json(json)
# print the JSON string representation of the object
print(UserRegistrationResponse.to_json())

# convert the object into a dict
user_registration_response_dict = user_registration_response_instance.to_dict()
# create an instance of UserRegistrationResponse from a dict
user_registration_response_from_dict = UserRegistrationResponse.from_dict(user_registration_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



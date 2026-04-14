# UserStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | **str** |  | 
**status** | **str** |  | 
**token** | **str** |  | 

## Example

```python
from valstorm_api.models.user_status import UserStatus

# TODO update the JSON string below
json = "{}"
# create an instance of UserStatus from a JSON string
user_status_instance = UserStatus.from_json(json)
# print the JSON string representation of the object
print(UserStatus.to_json())

# convert the object into a dict
user_status_dict = user_status_instance.to_dict()
# create an instance of UserStatus from a dict
user_status_from_dict = UserStatus.from_dict(user_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



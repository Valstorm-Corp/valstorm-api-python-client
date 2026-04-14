# LoginAsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 

## Example

```python
from valstorm_api.models.login_as_request import LoginAsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of LoginAsRequest from a JSON string
login_as_request_instance = LoginAsRequest.from_json(json)
# print the JSON string representation of the object
print(LoginAsRequest.to_json())

# convert the object into a dict
login_as_request_dict = login_as_request_instance.to_dict()
# create an instance of LoginAsRequest from a dict
login_as_request_from_dict = LoginAsRequest.from_dict(login_as_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# PushCredential


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**sandbox** | **bool** |  | [optional] [default to False]

## Example

```python
from valstorm_api.models.push_credential import PushCredential

# TODO update the JSON string below
json = "{}"
# create an instance of PushCredential from a JSON string
push_credential_instance = PushCredential.from_json(json)
# print the JSON string representation of the object
print(PushCredential.to_json())

# convert the object into a dict
push_credential_dict = push_credential_instance.to_dict()
# create an instance of PushCredential from a dict
push_credential_from_dict = PushCredential.from_dict(push_credential_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



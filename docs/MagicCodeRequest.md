# MagicCodeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**client_id** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.magic_code_request import MagicCodeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MagicCodeRequest from a JSON string
magic_code_request_instance = MagicCodeRequest.from_json(json)
# print the JSON string representation of the object
print(MagicCodeRequest.to_json())

# convert the object into a dict
magic_code_request_dict = magic_code_request_instance.to_dict()
# create an instance of MagicCodeRequest from a dict
magic_code_request_from_dict = MagicCodeRequest.from_dict(magic_code_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



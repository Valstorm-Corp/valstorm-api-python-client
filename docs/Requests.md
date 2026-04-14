# Requests


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | 
**body** | **str** |  | 
**type** | **str** |  | [optional] [default to 'dynamic']
**user_id** | **str** |  | [optional] 
**data** | **Dict[str, object]** |  | [optional] 
**save** | **bool** |  | [optional] [default to True]
**notify** | **bool** |  | [optional] [default to True]
**push_to_mobile** | **bool** |  | [optional] [default to False]
**record_id** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.requests import Requests

# TODO update the JSON string below
json = "{}"
# create an instance of Requests from a JSON string
requests_instance = Requests.from_json(json)
# print the JSON string representation of the object
print(Requests.to_json())

# convert the object into a dict
requests_dict = requests_instance.to_dict()
# create an instance of Requests from a dict
requests_from_dict = Requests.from_dict(requests_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



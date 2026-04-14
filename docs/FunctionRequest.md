# FunctionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**function_id** | **str** |  | [optional] 
**function_name** | **str** |  | [optional] 
**system_function** | **bool** |  | [optional] 
**inputs** | **Dict[str, object]** |  | [optional] 

## Example

```python
from valstorm_api.models.function_request import FunctionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FunctionRequest from a JSON string
function_request_instance = FunctionRequest.from_json(json)
# print the JSON string representation of the object
print(FunctionRequest.to_json())

# convert the object into a dict
function_request_dict = function_request_instance.to_dict()
# create an instance of FunctionRequest from a dict
function_request_from_dict = FunctionRequest.from_dict(function_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ConfirmToolRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**agent_id** | **str** |  | [optional] 
**approved** | **bool** |  | 
**ai_chat** | **str** |  | 
**model** | **str** |  | [optional] 
**system_prompt** | **str** |  | [optional] 
**allowed_tools** | **List[str]** |  | [optional] 

## Example

```python
from valstorm_api.models.confirm_tool_request import ConfirmToolRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ConfirmToolRequest from a JSON string
confirm_tool_request_instance = ConfirmToolRequest.from_json(json)
# print the JSON string representation of the object
print(ConfirmToolRequest.to_json())

# convert the object into a dict
confirm_tool_request_dict = confirm_tool_request_instance.to_dict()
# create an instance of ConfirmToolRequest from a dict
confirm_tool_request_from_dict = ConfirmToolRequest.from_dict(confirm_tool_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



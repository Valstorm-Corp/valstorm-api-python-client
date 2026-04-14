# SchemaUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**app** | **str** |  | 
**ownership** | **bool** |  | 
**exclusive_ownership** | **bool** |  | 
**junction_object** | **bool** |  | 
**relates_to_any_object** | **bool** |  | 
**icon** | **str** |  | [optional] 
**color** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.schema_update_request import SchemaUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SchemaUpdateRequest from a JSON string
schema_update_request_instance = SchemaUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SchemaUpdateRequest.to_json())

# convert the object into a dict
schema_update_request_dict = schema_update_request_instance.to_dict()
# create an instance of SchemaUpdateRequest from a dict
schema_update_request_from_dict = SchemaUpdateRequest.from_dict(schema_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



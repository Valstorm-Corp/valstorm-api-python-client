# SchemaCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**app** | **str** |  | 
**ownership** | **bool** |  | 
**exclusive_ownership** | **bool** |  | 
**junction_object** | **bool** |  | 
**relates_to_any_object** | **bool** |  | 

## Example

```python
from valstorm_api.models.schema_create_request import SchemaCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SchemaCreateRequest from a JSON string
schema_create_request_instance = SchemaCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SchemaCreateRequest.to_json())

# convert the object into a dict
schema_create_request_dict = schema_create_request_instance.to_dict()
# create an instance of SchemaCreateRequest from a dict
schema_create_request_from_dict = SchemaCreateRequest.from_dict(schema_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# FieldCreateUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**object_id** | **str** |  | 
**name** | **str** |  | 
**api_name** | **str** |  | 
**description** | **str** |  | [optional] 
**help_text** | **str** |  | [optional] 
**type** | **str** |  | 
**format** | **str** |  | [optional] 
**required** | **bool** |  | 
**default** | [**AnyOf**](AnyOf.md) |  | [optional] 
**sensitive** | **bool** |  | [optional] [default to False]
**encrypted** | **bool** |  | [optional] [default to False]
**app** | **str** |  | 
**var_schema** | **str** |  | [optional] 
**values** | **List[object]** |  | [optional] 
**global_** | **bool** |  | [optional] [default to False]
**global_list_name** | **str** |  | [optional] 
**object** | **str** |  | [optional] 
**restricted** | **bool** |  | [optional] [default to False]
**pii** | **bool** |  | [optional] [default to False]
**phi** | **bool** |  | [optional] [default to False]
**plural_name** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.field_create_update_request import FieldCreateUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FieldCreateUpdateRequest from a JSON string
field_create_update_request_instance = FieldCreateUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(FieldCreateUpdateRequest.to_json())

# convert the object into a dict
field_create_update_request_dict = field_create_update_request_instance.to_dict()
# create an instance of FieldCreateUpdateRequest from a dict
field_create_update_request_from_dict = FieldCreateUpdateRequest.from_dict(field_create_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



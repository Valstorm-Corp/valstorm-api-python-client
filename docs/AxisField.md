# AxisField


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **str** |  | 
**label** | **str** |  | [optional] 
**aggregate** | **str** |  | [optional] 
**group_by_date_time** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.axis_field import AxisField

# TODO update the JSON string below
json = "{}"
# create an instance of AxisField from a JSON string
axis_field_instance = AxisField.from_json(json)
# print the JSON string representation of the object
print(AxisField.to_json())

# convert the object into a dict
axis_field_dict = axis_field_instance.to_dict()
# create an instance of AxisField from a dict
axis_field_from_dict = AxisField.from_dict(axis_field_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Data1


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | 
**chart_type** | **str** |  | 
**var_field** | [**List[ModelField]**](ModelField.md) |  | [optional] 
**x** | [**List[AxisField]**](AxisField.md) |  | [optional] 
**y** | [**List[AxisField]**](AxisField.md) |  | [optional] 
**aggregate** | **str** |  | [optional] 
**summarize_by** | **str** |  | [optional] 
**group_by_date_time** | **str** |  | [optional] 
**dashboard_id** | **str** |  | [optional] 
**component_id** | **str** |  | [optional] 
**object_id** | **str** |  | [optional] 
**item** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.data1 import Data1

# TODO update the JSON string below
json = "{}"
# create an instance of Data1 from a JSON string
data1_instance = Data1.from_json(json)
# print the JSON string representation of the object
print(Data1.to_json())

# convert the object into a dict
data1_dict = data1_instance.to_dict()
# create an instance of Data1 from a dict
data1_from_dict = Data1.from_dict(data1_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



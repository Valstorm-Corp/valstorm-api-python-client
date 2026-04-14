# Data2


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_number** | [**FromNumber**](FromNumber.md) |  | [optional] 
**to** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**template_id** | [**TemplateId1**](TemplateId1.md) |  | [optional] 
**merge_data** | [**MergeData**](MergeData.md) |  | [optional] 
**conversation_sid** | **str** |  | [optional] 
**media_sid** | **str** |  | [optional] 
**media** | **List[object]** |  | [optional] 
**automated** | **bool** |  | [optional] [default to True]
**use_conversations** | **bool** |  | [optional] [default to True]
**run_date_time** | **datetime** |  | [optional] 
**contact** | **Dict[str, object]** |  | [optional] 
**phone** | **Dict[str, object]** |  | [optional] 
**conversation** | **Dict[str, object]** |  | [optional] 
**participant** | **Dict[str, object]** |  | [optional] 
**scheduled_item_id** | **str** |  | [optional] 
**campaign_id** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.data2 import Data2

# TODO update the JSON string below
json = "{}"
# create an instance of Data2 from a JSON string
data2_instance = Data2.from_json(json)
# print the JSON string representation of the object
print(Data2.to_json())

# convert the object into a dict
data2_dict = data2_instance.to_dict()
# create an instance of Data2 from a dict
data2_from_dict = Data2.from_dict(data2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



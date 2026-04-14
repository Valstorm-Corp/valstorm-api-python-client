# MergeRecordsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**schema_api_name** | **str** |  | 
**master_record** | **str** |  | 
**selected_records** | **List[str]** |  | 

## Example

```python
from valstorm_api.models.merge_records_request import MergeRecordsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MergeRecordsRequest from a JSON string
merge_records_request_instance = MergeRecordsRequest.from_json(json)
# print the JSON string representation of the object
print(MergeRecordsRequest.to_json())

# convert the object into a dict
merge_records_request_dict = merge_records_request_instance.to_dict()
# create an instance of MergeRecordsRequest from a dict
merge_records_request_from_dict = MergeRecordsRequest.from_dict(merge_records_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



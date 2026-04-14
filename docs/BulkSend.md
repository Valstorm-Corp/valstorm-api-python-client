# BulkSend


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**campaign** | **str** |  | 
**template** | **str** |  | [optional] 
**file** | **str** |  | [optional] 
**action** | **str** |  | 
**schedule_date_time** | **str** |  | 
**phone_field** | **str** |  | [optional] 
**email_field** | **str** |  | [optional] 
**from_number** | **str** |  | [optional] 
**from_email** | **str** |  | [optional] 
**provider** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**attachments** | **List[str]** |  | [optional] 
**automation** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.bulk_send import BulkSend

# TODO update the JSON string below
json = "{}"
# create an instance of BulkSend from a JSON string
bulk_send_instance = BulkSend.from_json(json)
# print the JSON string representation of the object
print(BulkSend.to_json())

# convert the object into a dict
bulk_send_dict = bulk_send_instance.to_dict()
# create an instance of BulkSend from a dict
bulk_send_from_dict = BulkSend.from_dict(bulk_send_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



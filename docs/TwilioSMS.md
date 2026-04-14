# TwilioSMS


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
from valstorm_api.models.twilio_sms import TwilioSMS

# TODO update the JSON string below
json = "{}"
# create an instance of TwilioSMS from a JSON string
twilio_sms_instance = TwilioSMS.from_json(json)
# print the JSON string representation of the object
print(TwilioSMS.to_json())

# convert the object into a dict
twilio_sms_dict = twilio_sms_instance.to_dict()
# create an instance of TwilioSMS from a dict
twilio_sms_from_dict = TwilioSMS.from_dict(twilio_sms_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



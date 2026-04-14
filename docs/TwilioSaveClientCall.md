# TwilioSaveClientCall


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sid** | **str** |  | 
**disposition** | **str** |  | 
**user** | **str** |  | 
**plain_notes** | **str** |  | 

## Example

```python
from valstorm_api.models.twilio_save_client_call import TwilioSaveClientCall

# TODO update the JSON string below
json = "{}"
# create an instance of TwilioSaveClientCall from a JSON string
twilio_save_client_call_instance = TwilioSaveClientCall.from_json(json)
# print the JSON string representation of the object
print(TwilioSaveClientCall.to_json())

# convert the object into a dict
twilio_save_client_call_dict = twilio_save_client_call_instance.to_dict()
# create an instance of TwilioSaveClientCall from a dict
twilio_save_client_call_from_dict = TwilioSaveClientCall.from_dict(twilio_save_client_call_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



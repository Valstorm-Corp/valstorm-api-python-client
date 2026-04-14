# TwimlApplicationUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sid** | **str** |  | 
**friendly_name** | **str** |  | [optional] [default to 'Valstorm']
**voice_caller_id_lookup** | **bool** |  | [optional] [default to False]

## Example

```python
from valstorm_api.models.twiml_application_update import TwimlApplicationUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of TwimlApplicationUpdate from a JSON string
twiml_application_update_instance = TwimlApplicationUpdate.from_json(json)
# print the JSON string representation of the object
print(TwimlApplicationUpdate.to_json())

# convert the object into a dict
twiml_application_update_dict = twiml_application_update_instance.to_dict()
# create an instance of TwimlApplicationUpdate from a dict
twiml_application_update_from_dict = TwimlApplicationUpdate.from_dict(twiml_application_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# TwimlApplication


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**friendly_name** | **str** |  | [optional] [default to 'Valstorm']
**voice_caller_id_lookup** | **bool** |  | [optional] [default to False]

## Example

```python
from valstorm_api.models.twiml_application import TwimlApplication

# TODO update the JSON string below
json = "{}"
# create an instance of TwimlApplication from a JSON string
twiml_application_instance = TwimlApplication.from_json(json)
# print the JSON string representation of the object
print(TwimlApplication.to_json())

# convert the object into a dict
twiml_application_dict = twiml_application_instance.to_dict()
# create an instance of TwimlApplication from a dict
twiml_application_from_dict = TwimlApplication.from_dict(twiml_application_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



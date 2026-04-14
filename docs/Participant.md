# Participant


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**messaging_binding** | [**MessagingBinding**](MessagingBinding.md) |  | 
**attributes** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.participant import Participant

# TODO update the JSON string below
json = "{}"
# create an instance of Participant from a JSON string
participant_instance = Participant.from_json(json)
# print the JSON string representation of the object
print(Participant.to_json())

# convert the object into a dict
participant_dict = participant_instance.to_dict()
# create an instance of Participant from a dict
participant_from_dict = Participant.from_dict(participant_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



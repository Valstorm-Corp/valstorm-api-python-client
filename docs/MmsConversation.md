# MmsConversation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**friendly_name** | **str** |  | 
**participants** | [**List[Participant]**](Participant.md) |  | 
**chat_service_sid** | **str** |  | 
**phone** | **str** |  | 

## Example

```python
from valstorm_api.models.mms_conversation import MmsConversation

# TODO update the JSON string below
json = "{}"
# create an instance of MmsConversation from a JSON string
mms_conversation_instance = MmsConversation.from_json(json)
# print the JSON string representation of the object
print(MmsConversation.to_json())

# convert the object into a dict
mms_conversation_dict = mms_conversation_instance.to_dict()
# create an instance of MmsConversation from a dict
mms_conversation_from_dict = MmsConversation.from_dict(mms_conversation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



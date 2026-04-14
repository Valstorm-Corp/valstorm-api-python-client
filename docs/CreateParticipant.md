# CreateParticipant


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conversation_sid** | **str** |  | 
**identity** | **str** |  | [optional] 
**messaging_binding_address** | **str** |  | [optional] 
**messaging_binding_proxy_address** | **str** |  | [optional] 
**messaging_binding_projected_address** | **str** |  | [optional] 
**contact** | **str** |  | [optional] 
**user_name** | **str** |  | [optional] 
**contact_name** | **str** |  | [optional] 
**chat_service_sid** | **str** |  | [optional] 
**attributes** | **str** |  | [optional] 
**phone** | [**Phone**](Phone.md) |  | [optional] 

## Example

```python
from valstorm_api.models.create_participant import CreateParticipant

# TODO update the JSON string below
json = "{}"
# create an instance of CreateParticipant from a JSON string
create_participant_instance = CreateParticipant.from_json(json)
# print the JSON string representation of the object
print(CreateParticipant.to_json())

# convert the object into a dict
create_participant_dict = create_participant_instance.to_dict()
# create an instance of CreateParticipant from a dict
create_participant_from_dict = CreateParticipant.from_dict(create_participant_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



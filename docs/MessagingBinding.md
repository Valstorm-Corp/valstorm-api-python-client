# MessagingBinding


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **str** |  | [optional] 
**projected_address** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.messaging_binding import MessagingBinding

# TODO update the JSON string below
json = "{}"
# create an instance of MessagingBinding from a JSON string
messaging_binding_instance = MessagingBinding.from_json(json)
# print the JSON string representation of the object
print(MessagingBinding.to_json())

# convert the object into a dict
messaging_binding_dict = messaging_binding_instance.to_dict()
# create an instance of MessagingBinding from a dict
messaging_binding_from_dict = MessagingBinding.from_dict(messaging_binding_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



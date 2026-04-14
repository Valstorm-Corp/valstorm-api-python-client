# EmailMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subject** | **str** |  | 
**content** | **str** |  | 
**from_address** | **str** |  | 
**to_address** | **str** |  | 
**html_content** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.email_message import EmailMessage

# TODO update the JSON string below
json = "{}"
# create an instance of EmailMessage from a JSON string
email_message_instance = EmailMessage.from_json(json)
# print the JSON string representation of the object
print(EmailMessage.to_json())

# convert the object into a dict
email_message_dict = email_message_instance.to_dict()
# create an instance of EmailMessage from a dict
email_message_from_dict = EmailMessage.from_dict(email_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



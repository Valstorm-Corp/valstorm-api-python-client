# WebNotificationMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**token** | **str** |  | 
**data** | [**WebNotificationData**](WebNotificationData.md) |  | 

## Example

```python
from valstorm_api.models.web_notification_message import WebNotificationMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebNotificationMessage from a JSON string
web_notification_message_instance = WebNotificationMessage.from_json(json)
# print the JSON string representation of the object
print(WebNotificationMessage.to_json())

# convert the object into a dict
web_notification_message_dict = web_notification_message_instance.to_dict()
# create an instance of WebNotificationMessage from a dict
web_notification_message_from_dict = WebNotificationMessage.from_dict(web_notification_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# WebNotification


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | [**WebNotificationMessage**](WebNotificationMessage.md) |  | 

## Example

```python
from valstorm_api.models.web_notification import WebNotification

# TODO update the JSON string below
json = "{}"
# create an instance of WebNotification from a JSON string
web_notification_instance = WebNotification.from_json(json)
# print the JSON string representation of the object
print(WebNotification.to_json())

# convert the object into a dict
web_notification_dict = web_notification_instance.to_dict()
# create an instance of WebNotification from a dict
web_notification_from_dict = WebNotification.from_dict(web_notification_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



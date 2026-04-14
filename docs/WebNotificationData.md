# WebNotificationData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | 
**body** | **str** |  | 
**url** | **str** |  | [optional] 
**icon** | **str** |  | [optional] 
**image** | **str** |  | [optional] 
**tag** | **str** |  | [optional] 
**tab** | **str** |  | [optional] 
**sound** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.web_notification_data import WebNotificationData

# TODO update the JSON string below
json = "{}"
# create an instance of WebNotificationData from a JSON string
web_notification_data_instance = WebNotificationData.from_json(json)
# print the JSON string representation of the object
print(WebNotificationData.to_json())

# convert the object into a dict
web_notification_data_dict = web_notification_data_instance.to_dict()
# create an instance of WebNotificationData from a dict
web_notification_data_from_dict = WebNotificationData.from_dict(web_notification_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# SendNotificationSetting


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**data** | **Dict[str, object]** |  | [optional] 

## Example

```python
from valstorm_api.models.send_notification_setting import SendNotificationSetting

# TODO update the JSON string below
json = "{}"
# create an instance of SendNotificationSetting from a JSON string
send_notification_setting_instance = SendNotificationSetting.from_json(json)
# print the JSON string representation of the object
print(SendNotificationSetting.to_json())

# convert the object into a dict
send_notification_setting_dict = send_notification_setting_instance.to_dict()
# create an instance of SendNotificationSetting from a dict
send_notification_setting_from_dict = SendNotificationSetting.from_dict(send_notification_setting_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



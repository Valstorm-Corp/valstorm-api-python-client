# SendGridTrackingSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**click_tracking** | **bool** |  | [optional] [default to True]
**open_tracking** | **bool** |  | [optional] [default to True]
**subscription_tracking** | **bool** |  | [optional] [default to False]
**ganalytics** | **Dict[str, object]** |  | [optional] 

## Example

```python
from valstorm_api.models.send_grid_tracking_settings import SendGridTrackingSettings

# TODO update the JSON string below
json = "{}"
# create an instance of SendGridTrackingSettings from a JSON string
send_grid_tracking_settings_instance = SendGridTrackingSettings.from_json(json)
# print the JSON string representation of the object
print(SendGridTrackingSettings.to_json())

# convert the object into a dict
send_grid_tracking_settings_dict = send_grid_tracking_settings_instance.to_dict()
# create an instance of SendGridTrackingSettings from a dict
send_grid_tracking_settings_from_dict = SendGridTrackingSettings.from_dict(send_grid_tracking_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



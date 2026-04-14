# SendGridMailSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**footer_settings** | [**SendGridFooterSettings**](SendGridFooterSettings.md) |  | [optional] 
**sandbox_mode** | [**SendGridEnable**](SendGridEnable.md) |  | [optional] 
**bypass_list_management** | [**SendGridEnable**](SendGridEnable.md) |  | [optional] 
**bypass_spam_management** | [**SendGridEnable**](SendGridEnable.md) |  | [optional] 
**bypass_bounce_management** | [**SendGridEnable**](SendGridEnable.md) |  | [optional] 
**bypass_unsubscribe_management** | [**SendGridEnable**](SendGridEnable.md) |  | [optional] 

## Example

```python
from valstorm_api.models.send_grid_mail_settings import SendGridMailSettings

# TODO update the JSON string below
json = "{}"
# create an instance of SendGridMailSettings from a JSON string
send_grid_mail_settings_instance = SendGridMailSettings.from_json(json)
# print the JSON string representation of the object
print(SendGridMailSettings.to_json())

# convert the object into a dict
send_grid_mail_settings_dict = send_grid_mail_settings_instance.to_dict()
# create an instance of SendGridMailSettings from a dict
send_grid_mail_settings_from_dict = SendGridMailSettings.from_dict(send_grid_mail_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



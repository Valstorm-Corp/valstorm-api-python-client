# SendGridFooterSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enable** | **bool** |  | [optional] [default to False]
**text** | **str** |  | [optional] 
**html** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.send_grid_footer_settings import SendGridFooterSettings

# TODO update the JSON string below
json = "{}"
# create an instance of SendGridFooterSettings from a JSON string
send_grid_footer_settings_instance = SendGridFooterSettings.from_json(json)
# print the JSON string representation of the object
print(SendGridFooterSettings.to_json())

# convert the object into a dict
send_grid_footer_settings_dict = send_grid_footer_settings_instance.to_dict()
# create an instance of SendGridFooterSettings from a dict
send_grid_footer_settings_from_dict = SendGridFooterSettings.from_dict(send_grid_footer_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



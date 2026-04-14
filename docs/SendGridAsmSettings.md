# SendGridAsmSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group_id** | **int** |  | 
**groups_to_display** | **List[int]** |  | [optional] 

## Example

```python
from valstorm_api.models.send_grid_asm_settings import SendGridAsmSettings

# TODO update the JSON string below
json = "{}"
# create an instance of SendGridAsmSettings from a JSON string
send_grid_asm_settings_instance = SendGridAsmSettings.from_json(json)
# print the JSON string representation of the object
print(SendGridAsmSettings.to_json())

# convert the object into a dict
send_grid_asm_settings_dict = send_grid_asm_settings_instance.to_dict()
# create an instance of SendGridAsmSettings from a dict
send_grid_asm_settings_from_dict = SendGridAsmSettings.from_dict(send_grid_asm_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



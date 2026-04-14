# SendGridAttachment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_content** | **str** |  | 
**file_name** | **str** |  | 
**file_type** | **str** |  | [optional] 
**disposition** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.send_grid_attachment import SendGridAttachment

# TODO update the JSON string below
json = "{}"
# create an instance of SendGridAttachment from a JSON string
send_grid_attachment_instance = SendGridAttachment.from_json(json)
# print the JSON string representation of the object
print(SendGridAttachment.to_json())

# convert the object into a dict
send_grid_attachment_dict = send_grid_attachment_instance.to_dict()
# create an instance of SendGridAttachment from a dict
send_grid_attachment_from_dict = SendGridAttachment.from_dict(send_grid_attachment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



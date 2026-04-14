# SendGridEmailRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to_emails** | **List[str]** |  | 
**from_email** | **str** |  | 
**cc** | **List[str]** |  | [optional] 
**bcc** | **List[str]** |  | [optional] 
**reply_to** | **str** |  | [optional] 
**subject** | **str** |  | 
**plain_text_content** | **str** |  | 
**html_content** | **str** |  | [optional] 
**template_id** | [**TemplateId1**](TemplateId1.md) |  | [optional] 
**merge_data** | **Dict[str, object]** |  | [optional] 
**file_attachments** | **List[str]** |  | [optional] 
**attachments** | [**List[SendGridAttachment]**](SendGridAttachment.md) |  | [optional] 
**mail_settings** | [**SendGridMailSettings**](SendGridMailSettings.md) |  | [optional] 
**tracking_settings** | [**SendGridTrackingSettings**](SendGridTrackingSettings.md) |  | [optional] 
**asm_settings** | [**SendGridAsmSettings**](SendGridAsmSettings.md) |  | [optional] 

## Example

```python
from valstorm_api.models.send_grid_email_request import SendGridEmailRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendGridEmailRequest from a JSON string
send_grid_email_request_instance = SendGridEmailRequest.from_json(json)
# print the JSON string representation of the object
print(SendGridEmailRequest.to_json())

# convert the object into a dict
send_grid_email_request_dict = send_grid_email_request_instance.to_dict()
# create an instance of SendGridEmailRequest from a dict
send_grid_email_request_from_dict = SendGridEmailRequest.from_dict(send_grid_email_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



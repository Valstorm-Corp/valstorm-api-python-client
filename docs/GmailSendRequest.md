# GmailSendRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to** | [**To**](To.md) |  | 
**from_email** | **str** |  | 
**cc** | **List[str]** |  | [optional] 
**bcc** | **List[str]** |  | [optional] 
**reply_to** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**html_content** | **str** |  | [optional] 
**template_id** | [**TemplateId**](TemplateId.md) |  | [optional] 
**merge_data** | **Dict[str, object]** |  | [optional] 
**attachments** | **List[str]** |  | [optional] 

## Example

```python
from valstorm_api.models.gmail_send_request import GmailSendRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GmailSendRequest from a JSON string
gmail_send_request_instance = GmailSendRequest.from_json(json)
# print the JSON string representation of the object
print(GmailSendRequest.to_json())

# convert the object into a dict
gmail_send_request_dict = gmail_send_request_instance.to_dict()
# create an instance of GmailSendRequest from a dict
gmail_send_request_from_dict = GmailSendRequest.from_dict(gmail_send_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



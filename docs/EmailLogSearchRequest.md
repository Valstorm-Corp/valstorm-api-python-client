# EmailLogSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** | SendGrid SQL-like query. E.g.: status&#x3D;&#39;delivered&#39; AND to_email&#x3D;&#39;example@test.com&#39; | 
**limit** | **int** |  | [optional] 

## Example

```python
from valstorm_api.models.email_log_search_request import EmailLogSearchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EmailLogSearchRequest from a JSON string
email_log_search_request_instance = EmailLogSearchRequest.from_json(json)
# print the JSON string representation of the object
print(EmailLogSearchRequest.to_json())

# convert the object into a dict
email_log_search_request_dict = email_log_search_request_instance.to_dict()
# create an instance of EmailLogSearchRequest from a dict
email_log_search_request_from_dict = EmailLogSearchRequest.from_dict(email_log_search_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# EmailValidationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**check_deliverability** | **bool** |  | [optional] [default to False]

## Example

```python
from valstorm_api.models.email_validation_request import EmailValidationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EmailValidationRequest from a JSON string
email_validation_request_instance = EmailValidationRequest.from_json(json)
# print the JSON string representation of the object
print(EmailValidationRequest.to_json())

# convert the object into a dict
email_validation_request_dict = email_validation_request_instance.to_dict()
# create an instance of EmailValidationRequest from a dict
email_validation_request_from_dict = EmailValidationRequest.from_dict(email_validation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



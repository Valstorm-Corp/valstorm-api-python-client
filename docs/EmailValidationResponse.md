# EmailValidationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**is_valid** | **bool** |  | 
**normalized_email** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.email_validation_response import EmailValidationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EmailValidationResponse from a JSON string
email_validation_response_instance = EmailValidationResponse.from_json(json)
# print the JSON string representation of the object
print(EmailValidationResponse.to_json())

# convert the object into a dict
email_validation_response_dict = email_validation_response_instance.to_dict()
# create an instance of EmailValidationResponse from a dict
email_validation_response_from_dict = EmailValidationResponse.from_dict(email_validation_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



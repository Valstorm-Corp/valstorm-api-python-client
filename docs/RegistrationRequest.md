# RegistrationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**company** | **str** |  | 
**website** | **str** |  | 
**address** | [**Address**](Address.md) |  | 
**shipping_address** | [**Address**](Address.md) |  | 
**first_name** | **str** |  | 
**last_name** | **str** |  | 
**email** | **str** |  | 
**phone** | [**Phone**](Phone.md) |  | 
**system_user** | **bool** |  | [optional] [default to False]

## Example

```python
from valstorm_api.models.registration_request import RegistrationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RegistrationRequest from a JSON string
registration_request_instance = RegistrationRequest.from_json(json)
# print the JSON string representation of the object
print(RegistrationRequest.to_json())

# convert the object into a dict
registration_request_dict = registration_request_instance.to_dict()
# create an instance of RegistrationRequest from a dict
registration_request_from_dict = RegistrationRequest.from_dict(registration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



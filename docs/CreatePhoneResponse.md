# CreatePhoneResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | 

## Example

```python
from valstorm_api.models.create_phone_response import CreatePhoneResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePhoneResponse from a JSON string
create_phone_response_instance = CreatePhoneResponse.from_json(json)
# print the JSON string representation of the object
print(CreatePhoneResponse.to_json())

# convert the object into a dict
create_phone_response_dict = create_phone_response_instance.to_dict()
# create an instance of CreatePhoneResponse from a dict
create_phone_response_from_dict = CreatePhoneResponse.from_dict(create_phone_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



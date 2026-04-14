# TwoFAResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**detail** | **str** |  | [optional] [default to '2FA Required']
**two_fa_required** | **bool** |  | [optional] [default to True]
**email** | **str** |  | 

## Example

```python
from valstorm_api.models.two_fa_response import TwoFAResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TwoFAResponse from a JSON string
two_fa_response_instance = TwoFAResponse.from_json(json)
# print the JSON string representation of the object
print(TwoFAResponse.to_json())

# convert the object into a dict
two_fa_response_dict = two_fa_response_instance.to_dict()
# create an instance of TwoFAResponse from a dict
two_fa_response_from_dict = TwoFAResponse.from_dict(two_fa_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



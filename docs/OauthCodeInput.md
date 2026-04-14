# OauthCodeInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **str** |  | 
**state** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.oauth_code_input import OauthCodeInput

# TODO update the JSON string below
json = "{}"
# create an instance of OauthCodeInput from a JSON string
oauth_code_input_instance = OauthCodeInput.from_json(json)
# print the JSON string representation of the object
print(OauthCodeInput.to_json())

# convert the object into a dict
oauth_code_input_dict = oauth_code_input_instance.to_dict()
# create an instance of OauthCodeInput from a dict
oauth_code_input_from_dict = OauthCodeInput.from_dict(oauth_code_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



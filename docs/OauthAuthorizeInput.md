# OauthAuthorizeInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **str** |  | 
**redirect_uri** | **str** |  | 
**response_type** | **str** |  | 
**state** | **str** |  | [optional] 
**scope** | **str** |  | [optional] 
**code_challenge** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.oauth_authorize_input import OauthAuthorizeInput

# TODO update the JSON string below
json = "{}"
# create an instance of OauthAuthorizeInput from a JSON string
oauth_authorize_input_instance = OauthAuthorizeInput.from_json(json)
# print the JSON string representation of the object
print(OauthAuthorizeInput.to_json())

# convert the object into a dict
oauth_authorize_input_dict = oauth_authorize_input_instance.to_dict()
# create an instance of OauthAuthorizeInput from a dict
oauth_authorize_input_from_dict = OauthAuthorizeInput.from_dict(oauth_authorize_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



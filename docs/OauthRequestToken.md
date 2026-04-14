# OauthRequestToken


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **str** |  | 
**client_secret** | **str** |  | 
**grant_type** | **str** |  | 
**code** | **str** |  | 
**redirect_uri** | **str** |  | 
**run_as** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.oauth_request_token import OauthRequestToken

# TODO update the JSON string below
json = "{}"
# create an instance of OauthRequestToken from a JSON string
oauth_request_token_instance = OauthRequestToken.from_json(json)
# print the JSON string representation of the object
print(OauthRequestToken.to_json())

# convert the object into a dict
oauth_request_token_dict = oauth_request_token_instance.to_dict()
# create an instance of OauthRequestToken from a dict
oauth_request_token_from_dict = OauthRequestToken.from_dict(oauth_request_token_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



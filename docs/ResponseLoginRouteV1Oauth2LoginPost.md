# ResponseLoginRouteV1Oauth2LoginPost


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_token** | **str** |  | 
**refresh_token** | **str** |  | 
**token_type** | **str** |  | 
**detail** | **str** |  | [optional] [default to '2FA Required']
**two_fa_required** | **bool** |  | [optional] [default to True]
**email** | **str** |  | 

## Example

```python
from valstorm_api.models.response_login_route_v1_oauth2_login_post import ResponseLoginRouteV1Oauth2LoginPost

# TODO update the JSON string below
json = "{}"
# create an instance of ResponseLoginRouteV1Oauth2LoginPost from a JSON string
response_login_route_v1_oauth2_login_post_instance = ResponseLoginRouteV1Oauth2LoginPost.from_json(json)
# print the JSON string representation of the object
print(ResponseLoginRouteV1Oauth2LoginPost.to_json())

# convert the object into a dict
response_login_route_v1_oauth2_login_post_dict = response_login_route_v1_oauth2_login_post_instance.to_dict()
# create an instance of ResponseLoginRouteV1Oauth2LoginPost from a dict
response_login_route_v1_oauth2_login_post_from_dict = ResponseLoginRouteV1Oauth2LoginPost.from_dict(response_login_route_v1_oauth2_login_post_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



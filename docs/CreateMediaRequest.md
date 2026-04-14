# CreateMediaRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_id** | **str** |  | 

## Example

```python
from valstorm_api.models.create_media_request import CreateMediaRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateMediaRequest from a JSON string
create_media_request_instance = CreateMediaRequest.from_json(json)
# print the JSON string representation of the object
print(CreateMediaRequest.to_json())

# convert the object into a dict
create_media_request_dict = create_media_request_instance.to_dict()
# create an instance of CreateMediaRequest from a dict
create_media_request_from_dict = CreateMediaRequest.from_dict(create_media_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



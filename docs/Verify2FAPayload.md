# Verify2FAPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**code** | **str** |  | 

## Example

```python
from valstorm_api.models.verify2_fa_payload import Verify2FAPayload

# TODO update the JSON string below
json = "{}"
# create an instance of Verify2FAPayload from a JSON string
verify2_fa_payload_instance = Verify2FAPayload.from_json(json)
# print the JSON string representation of the object
print(Verify2FAPayload.to_json())

# convert the object into a dict
verify2_fa_payload_dict = verify2_fa_payload_instance.to_dict()
# create an instance of Verify2FAPayload from a dict
verify2_fa_payload_from_dict = Verify2FAPayload.from_dict(verify2_fa_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



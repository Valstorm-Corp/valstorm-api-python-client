# StatusStatusRoutesAvailable


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**call_status** | [**CallStatus**](CallStatus.md) |  | [optional] 
**reset** | **bool** |  | [optional] [default to False]
**user_id** | **str** |  | [optional] 
**available_for_mobile_calls** | **bool** |  | [optional] [default to True]
**available_for_web_calls** | **bool** |  | [optional] [default to True]
**allow_mobile_calls** | **bool** |  | [optional] [default to True]
**allow_web_calls** | **bool** |  | [optional] [default to True]
**has_mobile_app** | **bool** |  | [optional] [default to True]

## Example

```python
from valstorm_api.models.status_status_routes_available import StatusStatusRoutesAvailable

# TODO update the JSON string below
json = "{}"
# create an instance of StatusStatusRoutesAvailable from a JSON string
status_status_routes_available_instance = StatusStatusRoutesAvailable.from_json(json)
# print the JSON string representation of the object
print(StatusStatusRoutesAvailable.to_json())

# convert the object into a dict
status_status_routes_available_dict = status_status_routes_available_instance.to_dict()
# create an instance of StatusStatusRoutesAvailable from a dict
status_status_routes_available_from_dict = StatusStatusRoutesAvailable.from_dict(status_status_routes_available_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



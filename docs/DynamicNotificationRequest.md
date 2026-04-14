# DynamicNotificationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | 
**body** | **str** |  | 
**type** | **str** |  | [optional] [default to 'dynamic']
**user_id** | **str** |  | [optional] 
**data** | **Dict[str, object]** |  | [optional] 
**save** | **bool** |  | [optional] [default to True]
**notify** | **bool** |  | [optional] [default to True]
**push_to_mobile** | **bool** |  | [optional] [default to False]
**record_id** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.dynamic_notification_request import DynamicNotificationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DynamicNotificationRequest from a JSON string
dynamic_notification_request_instance = DynamicNotificationRequest.from_json(json)
# print the JSON string representation of the object
print(DynamicNotificationRequest.to_json())

# convert the object into a dict
dynamic_notification_request_dict = dynamic_notification_request_instance.to_dict()
# create an instance of DynamicNotificationRequest from a dict
dynamic_notification_request_from_dict = DynamicNotificationRequest.from_dict(dynamic_notification_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



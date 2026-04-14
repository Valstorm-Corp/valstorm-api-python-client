# CalendarSyncRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**calendars** | **List[str]** |  | 
**time_max** | **str** |  | [optional] [default to '2026-12-31T23:59:59Z']
**time_min** | **str** |  | [optional] [default to '2023-01-01T00:00:00Z']

## Example

```python
from valstorm_api.models.calendar_sync_request import CalendarSyncRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CalendarSyncRequest from a JSON string
calendar_sync_request_instance = CalendarSyncRequest.from_json(json)
# print the JSON string representation of the object
print(CalendarSyncRequest.to_json())

# convert the object into a dict
calendar_sync_request_dict = calendar_sync_request_instance.to_dict()
# create an instance of CalendarSyncRequest from a dict
calendar_sync_request_from_dict = CalendarSyncRequest.from_dict(calendar_sync_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



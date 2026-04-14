# ExportRecordsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | 

## Example

```python
from valstorm_api.models.export_records_request import ExportRecordsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ExportRecordsRequest from a JSON string
export_records_request_instance = ExportRecordsRequest.from_json(json)
# print the JSON string representation of the object
print(ExportRecordsRequest.to_json())

# convert the object into a dict
export_records_request_dict = export_records_request_instance.to_dict()
# create an instance of ExportRecordsRequest from a dict
export_records_request_from_dict = ExportRecordsRequest.from_dict(export_records_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



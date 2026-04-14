# FrontendAnalyticsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | 
**chart_type** | **str** |  | 
**var_field** | [**List[ModelField]**](ModelField.md) |  | [optional] 
**x** | [**List[AxisField]**](AxisField.md) |  | [optional] 
**y** | [**List[AxisField]**](AxisField.md) |  | [optional] 
**aggregate** | **str** |  | [optional] 
**summarize_by** | **str** |  | [optional] 
**group_by_date_time** | **str** |  | [optional] 
**dashboard_id** | **str** |  | [optional] 
**component_id** | **str** |  | [optional] 
**object_id** | **str** |  | [optional] 
**item** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.frontend_analytics_request import FrontendAnalyticsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FrontendAnalyticsRequest from a JSON string
frontend_analytics_request_instance = FrontendAnalyticsRequest.from_json(json)
# print the JSON string representation of the object
print(FrontendAnalyticsRequest.to_json())

# convert the object into a dict
frontend_analytics_request_dict = frontend_analytics_request_instance.to_dict()
# create an instance of FrontendAnalyticsRequest from a dict
frontend_analytics_request_from_dict = FrontendAnalyticsRequest.from_dict(frontend_analytics_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



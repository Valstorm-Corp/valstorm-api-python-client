# SalesforceNavigateToRecord


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**record_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**valstorm_id__c** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.salesforce_navigate_to_record import SalesforceNavigateToRecord

# TODO update the JSON string below
json = "{}"
# create an instance of SalesforceNavigateToRecord from a JSON string
salesforce_navigate_to_record_instance = SalesforceNavigateToRecord.from_json(json)
# print the JSON string representation of the object
print(SalesforceNavigateToRecord.to_json())

# convert the object into a dict
salesforce_navigate_to_record_dict = salesforce_navigate_to_record_instance.to_dict()
# create an instance of SalesforceNavigateToRecord from a dict
salesforce_navigate_to_record_from_dict = SalesforceNavigateToRecord.from_dict(salesforce_navigate_to_record_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



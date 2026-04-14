# CheckAvailability


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**scheduled** | **bool** |  | [optional] [default to False]

## Example

```python
from valstorm_api.models.check_availability import CheckAvailability

# TODO update the JSON string below
json = "{}"
# create an instance of CheckAvailability from a JSON string
check_availability_instance = CheckAvailability.from_json(json)
# print the JSON string representation of the object
print(CheckAvailability.to_json())

# convert the object into a dict
check_availability_dict = check_availability_instance.to_dict()
# create an instance of CheckAvailability from a dict
check_availability_from_dict = CheckAvailability.from_dict(check_availability_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



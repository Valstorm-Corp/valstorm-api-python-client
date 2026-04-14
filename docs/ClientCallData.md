# ClientCallData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to** | **str** |  | 
**from_number** | **str** |  | 
**conference_id** | **str** |  | [optional] 
**user** | **str** |  | 
**start_conference_on_enter** | **bool** |  | [optional] 
**end_conference_on_exit** | **bool** |  | [optional] [default to True]
**call_sid** | **str** |  | 
**transfer** | **str** |  | [optional] [default to 'Warm']

## Example

```python
from valstorm_api.models.client_call_data import ClientCallData

# TODO update the JSON string below
json = "{}"
# create an instance of ClientCallData from a JSON string
client_call_data_instance = ClientCallData.from_json(json)
# print the JSON string representation of the object
print(ClientCallData.to_json())

# convert the object into a dict
client_call_data_dict = client_call_data_instance.to_dict()
# create an instance of ClientCallData from a dict
client_call_data_from_dict = ClientCallData.from_dict(client_call_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



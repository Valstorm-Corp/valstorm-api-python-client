# PhoneAddressConfig


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | [**PhoneAddressType**](PhoneAddressType.md) |  | 
**address** | **str** |  | 
**friendly_name** | **str** |  | [optional] 
**auto_creation_enabled** | **bool** |  | [optional] [default to False]
**auto_creation_type** | **str** |  | [optional] 
**auto_creation_conversation_service_sid** | **str** |  | [optional] 
**auto_creation_webhook_url** | **str** |  | [optional] 
**auto_creation_webhook_method** | **str** |  | [optional] 
**auto_creation_webhook_filters** | **List[str]** |  | [optional] 

## Example

```python
from valstorm_api.models.phone_address_config import PhoneAddressConfig

# TODO update the JSON string below
json = "{}"
# create an instance of PhoneAddressConfig from a JSON string
phone_address_config_instance = PhoneAddressConfig.from_json(json)
# print the JSON string representation of the object
print(PhoneAddressConfig.to_json())

# convert the object into a dict
phone_address_config_dict = phone_address_config_instance.to_dict()
# create an instance of PhoneAddressConfig from a dict
phone_address_config_from_dict = PhoneAddressConfig.from_dict(phone_address_config_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



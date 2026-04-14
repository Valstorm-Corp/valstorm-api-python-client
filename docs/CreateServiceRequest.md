# CreateServiceRequest

Schema for creating a Twilio Conversational Intelligence Service. Corresponds to the 'Request body parameters' in the Twilio documentation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**unique_name** | **str** |  | 
**friendly_name** | **str** |  | [optional] 
**auto_transcribe** | **bool** |  | [optional] 
**data_logging** | **bool** |  | [optional] 
**language_code** | **str** |  | [optional] 
**auto_redaction** | **bool** |  | [optional] 
**media_redaction** | **bool** |  | [optional] 
**webhook_url** | **str** |  | [optional] 
**webhook_http_method** | **str** |  | [optional] 
**encryption_credential_sid** | **str** |  | [optional] 

## Example

```python
from valstorm_api.models.create_service_request import CreateServiceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateServiceRequest from a JSON string
create_service_request_instance = CreateServiceRequest.from_json(json)
# print the JSON string representation of the object
print(CreateServiceRequest.to_json())

# convert the object into a dict
create_service_request_dict = create_service_request_instance.to_dict()
# create an instance of CreateServiceRequest from a dict
create_service_request_from_dict = CreateServiceRequest.from_dict(create_service_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



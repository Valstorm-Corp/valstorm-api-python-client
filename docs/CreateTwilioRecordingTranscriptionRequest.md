# CreateTwilioRecordingTranscriptionRequest

Schema for creating a Twilio Recording Transcription.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recording_sid** | **str** |  | 
**service_sid** | **str** |  | 

## Example

```python
from valstorm_api.models.create_twilio_recording_transcription_request import CreateTwilioRecordingTranscriptionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTwilioRecordingTranscriptionRequest from a JSON string
create_twilio_recording_transcription_request_instance = CreateTwilioRecordingTranscriptionRequest.from_json(json)
# print the JSON string representation of the object
print(CreateTwilioRecordingTranscriptionRequest.to_json())

# convert the object into a dict
create_twilio_recording_transcription_request_dict = create_twilio_recording_transcription_request_instance.to_dict()
# create an instance of CreateTwilioRecordingTranscriptionRequest from a dict
create_twilio_recording_transcription_request_from_dict = CreateTwilioRecordingTranscriptionRequest.from_dict(create_twilio_recording_transcription_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# MongoQueryRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**collection** | **str** | The target collection name (e.g., &#39;contact&#39;) | 
**pipeline** | **List[Optional[Dict[str, object]]]** | The raw MongoDB aggregation pipeline | 

## Example

```python
from valstorm_api.models.mongo_query_request import MongoQueryRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MongoQueryRequest from a JSON string
mongo_query_request_instance = MongoQueryRequest.from_json(json)
# print the JSON string representation of the object
print(MongoQueryRequest.to_json())

# convert the object into a dict
mongo_query_request_dict = mongo_query_request_instance.to_dict()
# create an instance of MongoQueryRequest from a dict
mongo_query_request_from_dict = MongoQueryRequest.from_dict(mongo_query_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



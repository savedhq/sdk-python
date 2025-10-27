# ClientStorageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**workspace_id** | **str** |  | [optional] 
**provider** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from saved.models.client_storage_response import ClientStorageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ClientStorageResponse from a JSON string
client_storage_response_instance = ClientStorageResponse.from_json(json)
# print the JSON string representation of the object
print(ClientStorageResponse.to_json())

# convert the object into a dict
client_storage_response_dict = client_storage_response_instance.to_dict()
# create an instance of ClientStorageResponse from a dict
client_storage_response_from_dict = ClientStorageResponse.from_dict(client_storage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



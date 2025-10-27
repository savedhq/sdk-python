# StorageListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**limit** | **int** |  | [optional] 
**total** | **int** |  | [optional] 
**items** | [**List[ListStorages200ResponseAllOfItemsInner]**](ListStorages200ResponseAllOfItemsInner.md) |  | [optional] 

## Example

```python
from saved.models.storage_list_response import StorageListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of StorageListResponse from a JSON string
storage_list_response_instance = StorageListResponse.from_json(json)
# print the JSON string representation of the object
print(StorageListResponse.to_json())

# convert the object into a dict
storage_list_response_dict = storage_list_response_instance.to_dict()
# create an instance of StorageListResponse from a dict
storage_list_response_from_dict = StorageListResponse.from_dict(storage_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



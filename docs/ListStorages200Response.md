# ListStorages200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**limit** | **int** |  | [optional] 
**total** | **int** |  | [optional] 
**items** | [**List[ListStorages200ResponseAllOfItemsInner]**](ListStorages200ResponseAllOfItemsInner.md) |  | [optional] 

## Example

```python
from saved.models.list_storages200_response import ListStorages200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListStorages200Response from a JSON string
list_storages200_response_instance = ListStorages200Response.from_json(json)
# print the JSON string representation of the object
print(ListStorages200Response.to_json())

# convert the object into a dict
list_storages200_response_dict = list_storages200_response_instance.to_dict()
# create an instance of ListStorages200Response from a dict
list_storages200_response_from_dict = ListStorages200Response.from_dict(list_storages200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



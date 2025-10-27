# ListAutoBackup200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**limit** | **int** |  | [optional] 
**total** | **int** |  | [optional] 
**items** | [**List[ListAutoBackup200ResponseAllOfItemsInner]**](ListAutoBackup200ResponseAllOfItemsInner.md) |  | [optional] 

## Example

```python
from saved.models.list_auto_backup200_response import ListAutoBackup200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListAutoBackup200Response from a JSON string
list_auto_backup200_response_instance = ListAutoBackup200Response.from_json(json)
# print the JSON string representation of the object
print(ListAutoBackup200Response.to_json())

# convert the object into a dict
list_auto_backup200_response_dict = list_auto_backup200_response_instance.to_dict()
# create an instance of ListAutoBackup200Response from a dict
list_auto_backup200_response_from_dict = ListAutoBackup200Response.from_dict(list_auto_backup200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# BackupListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**limit** | **int** |  | [optional] 
**total** | **int** |  | [optional] 
**items** | [**List[ListBackups200ResponseAllOfItemsInner]**](ListBackups200ResponseAllOfItemsInner.md) |  | [optional] 

## Example

```python
from saved.models.backup_list_response import BackupListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackupListResponse from a JSON string
backup_list_response_instance = BackupListResponse.from_json(json)
# print the JSON string representation of the object
print(BackupListResponse.to_json())

# convert the object into a dict
backup_list_response_dict = backup_list_response_instance.to_dict()
# create an instance of BackupListResponse from a dict
backup_list_response_from_dict = BackupListResponse.from_dict(backup_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



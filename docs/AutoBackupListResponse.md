# AutoBackupListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**limit** | **int** |  | [optional] 
**total** | **int** |  | [optional] 
**items** | [**List[ListAutoBackup200ResponseAllOfItemsInner]**](ListAutoBackup200ResponseAllOfItemsInner.md) |  | [optional] 

## Example

```python
from saved.models.auto_backup_list_response import AutoBackupListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AutoBackupListResponse from a JSON string
auto_backup_list_response_instance = AutoBackupListResponse.from_json(json)
# print the JSON string representation of the object
print(AutoBackupListResponse.to_json())

# convert the object into a dict
auto_backup_list_response_dict = auto_backup_list_response_instance.to_dict()
# create an instance of AutoBackupListResponse from a dict
auto_backup_list_response_from_dict = AutoBackupListResponse.from_dict(auto_backup_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



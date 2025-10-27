# AutoBackupResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**vault_id** | **str** |  | [optional] 
**workspace_id** | **str** |  | [optional] 
**type** | **str** | Type of backup execution - &#39;worker&#39; for cloud-managed, &#39;agent&#39; for self-hosted | [optional] 
**provider** | **str** | Backup provider type (currently supports HTTP, extensible for future providers) | [optional] 
**agent_id** | **str** | Only present when type is &#39;agent&#39; | [optional] 
**zone** | **str** | Only present when type is &#39;worker&#39; | [optional] 
**schedule** | **str** | Cron expression | [optional] 
**temporal_schedule_id** | **str** | Temporal workflow schedule ID | [optional] 

## Example

```python
from saved.models.auto_backup_response import AutoBackupResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AutoBackupResponse from a JSON string
auto_backup_response_instance = AutoBackupResponse.from_json(json)
# print the JSON string representation of the object
print(AutoBackupResponse.to_json())

# convert the object into a dict
auto_backup_response_dict = auto_backup_response_instance.to_dict()
# create an instance of AutoBackupResponse from a dict
auto_backup_response_from_dict = AutoBackupResponse.from_dict(auto_backup_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



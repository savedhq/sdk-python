# UpdateAutoBackupRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Type of backup execution - &#39;worker&#39; for cloud-managed, &#39;agent&#39; for self-hosted | [optional] 
**provider** | **str** | Backup provider type (currently supports HTTP, extensible for future providers) | [optional] 
**config** | **object** | Provider-specific backup job configuration | [optional] 
**agent_id** | **str** | Required when type is &#39;agent&#39; | [optional] 
**zone** | **str** | Required when type is &#39;worker&#39; | [optional] 
**schedule** | **str** | Cron expression for scheduled execution | [optional] 

## Example

```python
from saved.models.update_auto_backup_request import UpdateAutoBackupRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateAutoBackupRequest from a JSON string
update_auto_backup_request_instance = UpdateAutoBackupRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateAutoBackupRequest.to_json())

# convert the object into a dict
update_auto_backup_request_dict = update_auto_backup_request_instance.to_dict()
# create an instance of UpdateAutoBackupRequest from a dict
update_auto_backup_request_from_dict = UpdateAutoBackupRequest.from_dict(update_auto_backup_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



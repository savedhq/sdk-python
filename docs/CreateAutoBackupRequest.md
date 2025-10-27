# CreateAutoBackupRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Type of backup execution - &#39;worker&#39; for cloud-managed, &#39;agent&#39; for self-hosted | 
**provider** | **str** | Backup provider type (currently supports HTTP, extensible for future providers) | 
**config** | **object** | Provider-specific backup job configuration. Required for worker jobs, optional for agent jobs (config provided in agent YAML) | [optional] 
**agent_id** | **str** | Required when type is &#39;agent&#39; | [optional] 
**zone** | **str** | Required when type is &#39;worker&#39; (e.g., us-east-1, us-west-2) | [optional] 
**schedule** | **str** | Cron expression for scheduled execution (e.g., \&quot;0 2 * * *\&quot; for daily at 2 AM) | 

## Example

```python
from saved.models.create_auto_backup_request import CreateAutoBackupRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAutoBackupRequest from a JSON string
create_auto_backup_request_instance = CreateAutoBackupRequest.from_json(json)
# print the JSON string representation of the object
print(CreateAutoBackupRequest.to_json())

# convert the object into a dict
create_auto_backup_request_dict = create_auto_backup_request_instance.to_dict()
# create an instance of CreateAutoBackupRequest from a dict
create_auto_backup_request_from_dict = CreateAutoBackupRequest.from_dict(create_auto_backup_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



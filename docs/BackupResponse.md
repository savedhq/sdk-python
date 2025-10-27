# BackupResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**workspace_id** | **str** |  | [optional] 
**vault_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**tags** | **List[str]** | List of tags | [optional] 
**checksum** | **str** | SHA256 hash of the backup file | [optional] 
**size** | **int** | Size of the backup in bytes | [optional] 
**content_type** | **str** | MIME type of the file | [optional] 
**status** | **str** | Current status of the backup | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**confirmed** | **bool** | Whether the backup upload has been confirmed | [optional] 
**verified** | **bool** | Whether the backup has been verified | [optional] 
**presigned_url** | **str** | S3 presigned URL for backup upload/download | [optional] 
**presigned_url_expires_at** | **datetime** | When the presigned URL expires | [optional] 
**workflow_id** | **str** | Temporal workflow ID | [optional] 

## Example

```python
from saved.models.backup_response import BackupResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackupResponse from a JSON string
backup_response_instance = BackupResponse.from_json(json)
# print the JSON string representation of the object
print(BackupResponse.to_json())

# convert the object into a dict
backup_response_dict = backup_response_instance.to_dict()
# create an instance of BackupResponse from a dict
backup_response_from_dict = BackupResponse.from_dict(backup_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



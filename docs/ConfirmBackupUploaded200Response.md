# ConfirmBackupUploaded200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**workspace_id** | **str** |  | [optional] 
**project_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] 
**checksum** | **str** |  | [optional] 
**size** | **int** |  | [optional] 
**content_type** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**confirmed** | **bool** |  | [optional] 
**verified** | **bool** |  | [optional] 
**workflow_id** | **str** |  | [optional] 

## Example

```python
from saved.models.confirm_backup_uploaded200_response import ConfirmBackupUploaded200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ConfirmBackupUploaded200Response from a JSON string
confirm_backup_uploaded200_response_instance = ConfirmBackupUploaded200Response.from_json(json)
# print the JSON string representation of the object
print(ConfirmBackupUploaded200Response.to_json())

# convert the object into a dict
confirm_backup_uploaded200_response_dict = confirm_backup_uploaded200_response_instance.to_dict()
# create an instance of ConfirmBackupUploaded200Response from a dict
confirm_backup_uploaded200_response_from_dict = ConfirmBackupUploaded200Response.from_dict(confirm_backup_uploaded200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



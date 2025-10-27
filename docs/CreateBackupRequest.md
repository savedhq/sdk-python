# CreateBackupRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** | Backup description | [optional] 
**tags** | **List[str]** | List of tags for categorization | [optional] 
**metadata** | **Dict[str, str]** | Additional key-value metadata | [optional] 

## Example

```python
from saved.models.create_backup_request import CreateBackupRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateBackupRequest from a JSON string
create_backup_request_instance = CreateBackupRequest.from_json(json)
# print the JSON string representation of the object
print(CreateBackupRequest.to_json())

# convert the object into a dict
create_backup_request_dict = create_backup_request_instance.to_dict()
# create an instance of CreateBackupRequest from a dict
create_backup_request_from_dict = CreateBackupRequest.from_dict(create_backup_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CreateBackup


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** | Backup description | [optional] 
**tags** | **List[str]** | List of tags for categorization | [optional] 
**metadata** | **Dict[str, str]** | Additional key-value metadata | [optional] 

## Example

```python
from saved.models.create_backup import CreateBackup

# TODO update the JSON string below
json = "{}"
# create an instance of CreateBackup from a JSON string
create_backup_instance = CreateBackup.from_json(json)
# print the JSON string representation of the object
print(CreateBackup.to_json())

# convert the object into a dict
create_backup_dict = create_backup_instance.to_dict()
# create an instance of CreateBackup from a dict
create_backup_from_dict = CreateBackup.from_dict(create_backup_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



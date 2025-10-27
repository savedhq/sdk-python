# ListAutoBackupExecutions200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**executions** | [**List[ListAutoBackupExecutions200ResponseExecutionsInner]**](ListAutoBackupExecutions200ResponseExecutionsInner.md) |  | [optional] 

## Example

```python
from saved.models.list_auto_backup_executions200_response import ListAutoBackupExecutions200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListAutoBackupExecutions200Response from a JSON string
list_auto_backup_executions200_response_instance = ListAutoBackupExecutions200Response.from_json(json)
# print the JSON string representation of the object
print(ListAutoBackupExecutions200Response.to_json())

# convert the object into a dict
list_auto_backup_executions200_response_dict = list_auto_backup_executions200_response_instance.to_dict()
# create an instance of ListAutoBackupExecutions200Response from a dict
list_auto_backup_executions200_response_from_dict = ListAutoBackupExecutions200Response.from_dict(list_auto_backup_executions200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



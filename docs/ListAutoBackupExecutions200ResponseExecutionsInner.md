# ListAutoBackupExecutions200ResponseExecutionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workflow_id** | **str** | Temporal workflow ID | [optional] 
**run_id** | **str** | Temporal run ID | [optional] 
**status** | **str** | Execution status (e.g., Running, Completed, Failed) | [optional] 
**start_time** | **datetime** |  | [optional] 
**close_time** | **datetime** |  | [optional] 
**execution_time** | **int** | Execution duration in milliseconds | [optional] 

## Example

```python
from saved.models.list_auto_backup_executions200_response_executions_inner import ListAutoBackupExecutions200ResponseExecutionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListAutoBackupExecutions200ResponseExecutionsInner from a JSON string
list_auto_backup_executions200_response_executions_inner_instance = ListAutoBackupExecutions200ResponseExecutionsInner.from_json(json)
# print the JSON string representation of the object
print(ListAutoBackupExecutions200ResponseExecutionsInner.to_json())

# convert the object into a dict
list_auto_backup_executions200_response_executions_inner_dict = list_auto_backup_executions200_response_executions_inner_instance.to_dict()
# create an instance of ListAutoBackupExecutions200ResponseExecutionsInner from a dict
list_auto_backup_executions200_response_executions_inner_from_dict = ListAutoBackupExecutions200ResponseExecutionsInner.from_dict(list_auto_backup_executions200_response_executions_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



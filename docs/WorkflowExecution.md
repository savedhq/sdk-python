# WorkflowExecution


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
from saved.models.workflow_execution import WorkflowExecution

# TODO update the JSON string below
json = "{}"
# create an instance of WorkflowExecution from a JSON string
workflow_execution_instance = WorkflowExecution.from_json(json)
# print the JSON string representation of the object
print(WorkflowExecution.to_json())

# convert the object into a dict
workflow_execution_dict = workflow_execution_instance.to_dict()
# create an instance of WorkflowExecution from a dict
workflow_execution_from_dict = WorkflowExecution.from_dict(workflow_execution_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# WorkflowExecutionHistoryResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**events** | [**List[GetAutoBackupHistoryDetails200ResponseEventsInner]**](GetAutoBackupHistoryDetails200ResponseEventsInner.md) |  | [optional] 

## Example

```python
from saved.models.workflow_execution_history_response import WorkflowExecutionHistoryResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WorkflowExecutionHistoryResponse from a JSON string
workflow_execution_history_response_instance = WorkflowExecutionHistoryResponse.from_json(json)
# print the JSON string representation of the object
print(WorkflowExecutionHistoryResponse.to_json())

# convert the object into a dict
workflow_execution_history_response_dict = workflow_execution_history_response_instance.to_dict()
# create an instance of WorkflowExecutionHistoryResponse from a dict
workflow_execution_history_response_from_dict = WorkflowExecutionHistoryResponse.from_dict(workflow_execution_history_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



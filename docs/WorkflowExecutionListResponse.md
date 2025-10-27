# WorkflowExecutionListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**executions** | [**List[ListAutoBackupExecutions200ResponseExecutionsInner]**](ListAutoBackupExecutions200ResponseExecutionsInner.md) |  | [optional] 

## Example

```python
from saved.models.workflow_execution_list_response import WorkflowExecutionListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WorkflowExecutionListResponse from a JSON string
workflow_execution_list_response_instance = WorkflowExecutionListResponse.from_json(json)
# print the JSON string representation of the object
print(WorkflowExecutionListResponse.to_json())

# convert the object into a dict
workflow_execution_list_response_dict = workflow_execution_list_response_instance.to_dict()
# create an instance of WorkflowExecutionListResponse from a dict
workflow_execution_list_response_from_dict = WorkflowExecutionListResponse.from_dict(workflow_execution_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



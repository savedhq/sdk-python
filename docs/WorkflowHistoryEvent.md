# WorkflowHistoryEvent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_id** | **int** |  | [optional] 
**event_time** | **datetime** |  | [optional] 
**event_type** | **str** |  | [optional] 
**details** | **Dict[str, object]** | Event-specific details | [optional] 

## Example

```python
from saved.models.workflow_history_event import WorkflowHistoryEvent

# TODO update the JSON string below
json = "{}"
# create an instance of WorkflowHistoryEvent from a JSON string
workflow_history_event_instance = WorkflowHistoryEvent.from_json(json)
# print the JSON string representation of the object
print(WorkflowHistoryEvent.to_json())

# convert the object into a dict
workflow_history_event_dict = workflow_history_event_instance.to_dict()
# create an instance of WorkflowHistoryEvent from a dict
workflow_history_event_from_dict = WorkflowHistoryEvent.from_dict(workflow_history_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



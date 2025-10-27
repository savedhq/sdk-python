# GetAutoBackupHistoryDetails200ResponseEventsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_id** | **int** |  | [optional] 
**event_time** | **datetime** |  | [optional] 
**event_type** | **str** |  | [optional] 
**details** | **Dict[str, object]** | Event-specific details | [optional] 

## Example

```python
from saved.models.get_auto_backup_history_details200_response_events_inner import GetAutoBackupHistoryDetails200ResponseEventsInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetAutoBackupHistoryDetails200ResponseEventsInner from a JSON string
get_auto_backup_history_details200_response_events_inner_instance = GetAutoBackupHistoryDetails200ResponseEventsInner.from_json(json)
# print the JSON string representation of the object
print(GetAutoBackupHistoryDetails200ResponseEventsInner.to_json())

# convert the object into a dict
get_auto_backup_history_details200_response_events_inner_dict = get_auto_backup_history_details200_response_events_inner_instance.to_dict()
# create an instance of GetAutoBackupHistoryDetails200ResponseEventsInner from a dict
get_auto_backup_history_details200_response_events_inner_from_dict = GetAutoBackupHistoryDetails200ResponseEventsInner.from_dict(get_auto_backup_history_details200_response_events_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



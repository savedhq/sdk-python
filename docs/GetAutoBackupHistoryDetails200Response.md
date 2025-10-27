# GetAutoBackupHistoryDetails200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**events** | [**List[GetAutoBackupHistoryDetails200ResponseEventsInner]**](GetAutoBackupHistoryDetails200ResponseEventsInner.md) |  | [optional] 

## Example

```python
from saved.models.get_auto_backup_history_details200_response import GetAutoBackupHistoryDetails200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetAutoBackupHistoryDetails200Response from a JSON string
get_auto_backup_history_details200_response_instance = GetAutoBackupHistoryDetails200Response.from_json(json)
# print the JSON string representation of the object
print(GetAutoBackupHistoryDetails200Response.to_json())

# convert the object into a dict
get_auto_backup_history_details200_response_dict = get_auto_backup_history_details200_response_instance.to_dict()
# create an instance of GetAutoBackupHistoryDetails200Response from a dict
get_auto_backup_history_details200_response_from_dict = GetAutoBackupHistoryDetails200Response.from_dict(get_auto_backup_history_details200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



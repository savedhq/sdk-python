# UpdateClientSignalJson


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**provider** | **str** |  | [optional] 
**config** | **object** |  | [optional] 

## Example

```python
from saved.models.update_client_signal_json import UpdateClientSignalJson

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateClientSignalJson from a JSON string
update_client_signal_json_instance = UpdateClientSignalJson.from_json(json)
# print the JSON string representation of the object
print(UpdateClientSignalJson.to_json())

# convert the object into a dict
update_client_signal_json_dict = update_client_signal_json_instance.to_dict()
# create an instance of UpdateClientSignalJson from a dict
update_client_signal_json_from_dict = UpdateClientSignalJson.from_dict(update_client_signal_json_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



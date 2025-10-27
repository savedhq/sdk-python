# UpdateSignalRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**provider** | **str** |  | [optional] 
**config** | **object** |  | [optional] 

## Example

```python
from saved.models.update_signal_request import UpdateSignalRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateSignalRequest from a JSON string
update_signal_request_instance = UpdateSignalRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateSignalRequest.to_json())

# convert the object into a dict
update_signal_request_dict = update_signal_request_instance.to_dict()
# create an instance of UpdateSignalRequest from a dict
update_signal_request_from_dict = UpdateSignalRequest.from_dict(update_signal_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



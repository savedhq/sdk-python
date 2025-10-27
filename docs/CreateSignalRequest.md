# CreateSignalRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**provider** | **str** |  | 
**config** | **object** | Provider-specific configuration (email or webhook) | 

## Example

```python
from saved.models.create_signal_request import CreateSignalRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSignalRequest from a JSON string
create_signal_request_instance = CreateSignalRequest.from_json(json)
# print the JSON string representation of the object
print(CreateSignalRequest.to_json())

# convert the object into a dict
create_signal_request_dict = create_signal_request_instance.to_dict()
# create an instance of CreateSignalRequest from a dict
create_signal_request_from_dict = CreateSignalRequest.from_dict(create_signal_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



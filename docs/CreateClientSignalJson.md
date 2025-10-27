# CreateClientSignalJson


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**provider** | **str** |  | 
**config** | **object** | Provider-specific configuration (email or webhook) | 

## Example

```python
from saved.models.create_client_signal_json import CreateClientSignalJson

# TODO update the JSON string below
json = "{}"
# create an instance of CreateClientSignalJson from a JSON string
create_client_signal_json_instance = CreateClientSignalJson.from_json(json)
# print the JSON string representation of the object
print(CreateClientSignalJson.to_json())

# convert the object into a dict
create_client_signal_json_dict = create_client_signal_json_instance.to_dict()
# create an instance of CreateClientSignalJson from a dict
create_client_signal_json_from_dict = CreateClientSignalJson.from_dict(create_client_signal_json_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



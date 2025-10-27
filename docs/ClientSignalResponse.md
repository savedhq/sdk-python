# ClientSignalResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**workspace_id** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**name** | **str** |  | [optional] 
**provider** | **str** |  | [optional] 

## Example

```python
from saved.models.client_signal_response import ClientSignalResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ClientSignalResponse from a JSON string
client_signal_response_instance = ClientSignalResponse.from_json(json)
# print the JSON string representation of the object
print(ClientSignalResponse.to_json())

# convert the object into a dict
client_signal_response_dict = client_signal_response_instance.to_dict()
# create an instance of ClientSignalResponse from a dict
client_signal_response_from_dict = ClientSignalResponse.from_dict(client_signal_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# SignalListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**limit** | **int** |  | [optional] 
**total** | **int** |  | [optional] 
**items** | [**List[ListSignals200ResponseAllOfItemsInner]**](ListSignals200ResponseAllOfItemsInner.md) |  | [optional] 

## Example

```python
from saved.models.signal_list_response import SignalListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SignalListResponse from a JSON string
signal_list_response_instance = SignalListResponse.from_json(json)
# print the JSON string representation of the object
print(SignalListResponse.to_json())

# convert the object into a dict
signal_list_response_dict = signal_list_response_instance.to_dict()
# create an instance of SignalListResponse from a dict
signal_list_response_from_dict = SignalListResponse.from_dict(signal_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



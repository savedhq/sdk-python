# ListSignals200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**limit** | **int** |  | [optional] 
**total** | **int** |  | [optional] 
**items** | [**List[ListSignals200ResponseAllOfItemsInner]**](ListSignals200ResponseAllOfItemsInner.md) |  | [optional] 

## Example

```python
from saved.models.list_signals200_response import ListSignals200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListSignals200Response from a JSON string
list_signals200_response_instance = ListSignals200Response.from_json(json)
# print the JSON string representation of the object
print(ListSignals200Response.to_json())

# convert the object into a dict
list_signals200_response_dict = list_signals200_response_instance.to_dict()
# create an instance of ListSignals200Response from a dict
list_signals200_response_from_dict = ListSignals200Response.from_dict(list_signals200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



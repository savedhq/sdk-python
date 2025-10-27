# ListSignals200ResponseAllOfItemsInner


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
from saved.models.list_signals200_response_all_of_items_inner import ListSignals200ResponseAllOfItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListSignals200ResponseAllOfItemsInner from a JSON string
list_signals200_response_all_of_items_inner_instance = ListSignals200ResponseAllOfItemsInner.from_json(json)
# print the JSON string representation of the object
print(ListSignals200ResponseAllOfItemsInner.to_json())

# convert the object into a dict
list_signals200_response_all_of_items_inner_dict = list_signals200_response_all_of_items_inner_instance.to_dict()
# create an instance of ListSignals200ResponseAllOfItemsInner from a dict
list_signals200_response_all_of_items_inner_from_dict = ListSignals200ResponseAllOfItemsInner.from_dict(list_signals200_response_all_of_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



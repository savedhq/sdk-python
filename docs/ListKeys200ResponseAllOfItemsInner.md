# ListKeys200ResponseAllOfItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**workspace_id** | **str** |  | [optional] 
**finger_print** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from saved.models.list_keys200_response_all_of_items_inner import ListKeys200ResponseAllOfItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListKeys200ResponseAllOfItemsInner from a JSON string
list_keys200_response_all_of_items_inner_instance = ListKeys200ResponseAllOfItemsInner.from_json(json)
# print the JSON string representation of the object
print(ListKeys200ResponseAllOfItemsInner.to_json())

# convert the object into a dict
list_keys200_response_all_of_items_inner_dict = list_keys200_response_all_of_items_inner_instance.to_dict()
# create an instance of ListKeys200ResponseAllOfItemsInner from a dict
list_keys200_response_all_of_items_inner_from_dict = ListKeys200ResponseAllOfItemsInner.from_dict(list_keys200_response_all_of_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ListAgents200ResponseAllOfItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**workspace_id** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_secret** | **str** |  | [optional] 
**scope** | **str** |  | [optional] 
**public_url** | **str** |  | [optional] 

## Example

```python
from saved.models.list_agents200_response_all_of_items_inner import ListAgents200ResponseAllOfItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListAgents200ResponseAllOfItemsInner from a JSON string
list_agents200_response_all_of_items_inner_instance = ListAgents200ResponseAllOfItemsInner.from_json(json)
# print the JSON string representation of the object
print(ListAgents200ResponseAllOfItemsInner.to_json())

# convert the object into a dict
list_agents200_response_all_of_items_inner_dict = list_agents200_response_all_of_items_inner_instance.to_dict()
# create an instance of ListAgents200ResponseAllOfItemsInner from a dict
list_agents200_response_all_of_items_inner_from_dict = ListAgents200ResponseAllOfItemsInner.from_dict(list_agents200_response_all_of_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



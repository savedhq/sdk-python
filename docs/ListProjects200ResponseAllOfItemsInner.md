# ListProjects200ResponseAllOfItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**workspace_id** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**retention_lock_period** | **int** | Duration in nanoseconds | [optional] 
**max_backup_count** | **int** |  | [optional] 
**max_backup_age** | **int** | Duration in nanoseconds | [optional] 
**compression_level** | **int** |  | [optional] 

## Example

```python
from saved.models.list_projects200_response_all_of_items_inner import ListProjects200ResponseAllOfItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListProjects200ResponseAllOfItemsInner from a JSON string
list_projects200_response_all_of_items_inner_instance = ListProjects200ResponseAllOfItemsInner.from_json(json)
# print the JSON string representation of the object
print(ListProjects200ResponseAllOfItemsInner.to_json())

# convert the object into a dict
list_projects200_response_all_of_items_inner_dict = list_projects200_response_all_of_items_inner_instance.to_dict()
# create an instance of ListProjects200ResponseAllOfItemsInner from a dict
list_projects200_response_all_of_items_inner_from_dict = ListProjects200ResponseAllOfItemsInner.from_dict(list_projects200_response_all_of_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



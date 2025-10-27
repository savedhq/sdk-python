# ListKeys200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**limit** | **int** |  | [optional] 
**total** | **int** |  | [optional] 
**items** | [**List[ListKeys200ResponseAllOfItemsInner]**](ListKeys200ResponseAllOfItemsInner.md) |  | [optional] 

## Example

```python
from saved.models.list_keys200_response import ListKeys200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListKeys200Response from a JSON string
list_keys200_response_instance = ListKeys200Response.from_json(json)
# print the JSON string representation of the object
print(ListKeys200Response.to_json())

# convert the object into a dict
list_keys200_response_dict = list_keys200_response_instance.to_dict()
# create an instance of ListKeys200Response from a dict
list_keys200_response_from_dict = ListKeys200Response.from_dict(list_keys200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



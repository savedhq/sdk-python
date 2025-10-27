# AddProjectStorageRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_storage_id** | **str** |  | 

## Example

```python
from saved.models.add_project_storage_request import AddProjectStorageRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AddProjectStorageRequest from a JSON string
add_project_storage_request_instance = AddProjectStorageRequest.from_json(json)
# print the JSON string representation of the object
print(AddProjectStorageRequest.to_json())

# convert the object into a dict
add_project_storage_request_dict = add_project_storage_request_instance.to_dict()
# create an instance of AddProjectStorageRequest from a dict
add_project_storage_request_from_dict = AddProjectStorageRequest.from_dict(add_project_storage_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



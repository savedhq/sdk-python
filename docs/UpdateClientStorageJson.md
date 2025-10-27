# UpdateClientStorageJson


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**provider** | **str** |  | [optional] 
**config** | **object** |  | [optional] 

## Example

```python
from saved.models.update_client_storage_json import UpdateClientStorageJson

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateClientStorageJson from a JSON string
update_client_storage_json_instance = UpdateClientStorageJson.from_json(json)
# print the JSON string representation of the object
print(UpdateClientStorageJson.to_json())

# convert the object into a dict
update_client_storage_json_dict = update_client_storage_json_instance.to_dict()
# create an instance of UpdateClientStorageJson from a dict
update_client_storage_json_from_dict = UpdateClientStorageJson.from_dict(update_client_storage_json_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



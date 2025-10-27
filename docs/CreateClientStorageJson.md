# CreateClientStorageJson


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**provider** | **str** |  | 
**config** | **object** | Provider-specific configuration (S3 or FTP) | 

## Example

```python
from saved.models.create_client_storage_json import CreateClientStorageJson

# TODO update the JSON string below
json = "{}"
# create an instance of CreateClientStorageJson from a JSON string
create_client_storage_json_instance = CreateClientStorageJson.from_json(json)
# print the JSON string representation of the object
print(CreateClientStorageJson.to_json())

# convert the object into a dict
create_client_storage_json_dict = create_client_storage_json_instance.to_dict()
# create an instance of CreateClientStorageJson from a dict
create_client_storage_json_from_dict = CreateClientStorageJson.from_dict(create_client_storage_json_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CreateStorageRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**provider** | **str** |  | 
**config** | **object** | Provider-specific configuration (S3 or FTP) | 

## Example

```python
from saved.models.create_storage_request import CreateStorageRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateStorageRequest from a JSON string
create_storage_request_instance = CreateStorageRequest.from_json(json)
# print the JSON string representation of the object
print(CreateStorageRequest.to_json())

# convert the object into a dict
create_storage_request_dict = create_storage_request_instance.to_dict()
# create an instance of CreateStorageRequest from a dict
create_storage_request_from_dict = CreateStorageRequest.from_dict(create_storage_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



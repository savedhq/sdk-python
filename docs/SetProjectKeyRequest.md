# SetProjectKeyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_encryption_key_id** | **str** |  | 

## Example

```python
from saved.models.set_project_key_request import SetProjectKeyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SetProjectKeyRequest from a JSON string
set_project_key_request_instance = SetProjectKeyRequest.from_json(json)
# print the JSON string representation of the object
print(SetProjectKeyRequest.to_json())

# convert the object into a dict
set_project_key_request_dict = set_project_key_request_instance.to_dict()
# create an instance of SetProjectKeyRequest from a dict
set_project_key_request_from_dict = SetProjectKeyRequest.from_dict(set_project_key_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



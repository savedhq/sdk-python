# ClientEncryptionKeyResponse


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
from saved.models.client_encryption_key_response import ClientEncryptionKeyResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ClientEncryptionKeyResponse from a JSON string
client_encryption_key_response_instance = ClientEncryptionKeyResponse.from_json(json)
# print the JSON string representation of the object
print(ClientEncryptionKeyResponse.to_json())

# convert the object into a dict
client_encryption_key_response_dict = client_encryption_key_response_instance.to_dict()
# create an instance of ClientEncryptionKeyResponse from a dict
client_encryption_key_response_from_dict = ClientEncryptionKeyResponse.from_dict(client_encryption_key_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



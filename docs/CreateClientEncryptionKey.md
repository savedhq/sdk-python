# CreateClientEncryptionKey


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**key** | **str** |  | 
**finger_print** | **str** |  | 

## Example

```python
from saved.models.create_client_encryption_key import CreateClientEncryptionKey

# TODO update the JSON string below
json = "{}"
# create an instance of CreateClientEncryptionKey from a JSON string
create_client_encryption_key_instance = CreateClientEncryptionKey.from_json(json)
# print the JSON string representation of the object
print(CreateClientEncryptionKey.to_json())

# convert the object into a dict
create_client_encryption_key_dict = create_client_encryption_key_instance.to_dict()
# create an instance of CreateClientEncryptionKey from a dict
create_client_encryption_key_from_dict = CreateClientEncryptionKey.from_dict(create_client_encryption_key_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



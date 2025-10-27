# ConfirmBackupUploadedRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Actual filename | 
**size** | **int** | File size in bytes | 
**checksum** | **str** | SHA256 hash of the file | 
**content_type** | **str** | MIME type of the file | 

## Example

```python
from saved.models.confirm_backup_uploaded_request import ConfirmBackupUploadedRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ConfirmBackupUploadedRequest from a JSON string
confirm_backup_uploaded_request_instance = ConfirmBackupUploadedRequest.from_json(json)
# print the JSON string representation of the object
print(ConfirmBackupUploadedRequest.to_json())

# convert the object into a dict
confirm_backup_uploaded_request_dict = confirm_backup_uploaded_request_instance.to_dict()
# create an instance of ConfirmBackupUploadedRequest from a dict
confirm_backup_uploaded_request_from_dict = ConfirmBackupUploadedRequest.from_dict(confirm_backup_uploaded_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



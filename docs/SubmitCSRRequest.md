# SubmitCSRRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**csr** | **str** | PEM-encoded Certificate Signing Request | 

## Example

```python
from saved.models.submit_csr_request import SubmitCSRRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubmitCSRRequest from a JSON string
submit_csr_request_instance = SubmitCSRRequest.from_json(json)
# print the JSON string representation of the object
print(SubmitCSRRequest.to_json())

# convert the object into a dict
submit_csr_request_dict = submit_csr_request_instance.to_dict()
# create an instance of SubmitCSRRequest from a dict
submit_csr_request_from_dict = SubmitCSRRequest.from_dict(submit_csr_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



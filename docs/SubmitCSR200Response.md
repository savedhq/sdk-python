# SubmitCSR200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**certificate** | **str** | PEM-encoded signed certificate | [optional] 
**ca_certificate** | **str** | PEM-encoded CA certificate | [optional] 
**certificate_expiry** | **datetime** | Certificate expiration timestamp | [optional] 

## Example

```python
from saved.models.submit_csr200_response import SubmitCSR200Response

# TODO update the JSON string below
json = "{}"
# create an instance of SubmitCSR200Response from a JSON string
submit_csr200_response_instance = SubmitCSR200Response.from_json(json)
# print the JSON string representation of the object
print(SubmitCSR200Response.to_json())

# convert the object into a dict
submit_csr200_response_dict = submit_csr200_response_instance.to_dict()
# create an instance of SubmitCSR200Response from a dict
submit_csr200_response_from_dict = SubmitCSR200Response.from_dict(submit_csr200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



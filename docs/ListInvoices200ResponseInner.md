# ListInvoices200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**amount_due** | **int** |  | [optional] 
**status** | **str** |  | [optional] 
**created** | **int** |  | [optional] 

## Example

```python
from saved.models.list_invoices200_response_inner import ListInvoices200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListInvoices200ResponseInner from a JSON string
list_invoices200_response_inner_instance = ListInvoices200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(ListInvoices200ResponseInner.to_json())

# convert the object into a dict
list_invoices200_response_inner_dict = list_invoices200_response_inner_instance.to_dict()
# create an instance of ListInvoices200ResponseInner from a dict
list_invoices200_response_inner_from_dict = ListInvoices200ResponseInner.from_dict(list_invoices200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



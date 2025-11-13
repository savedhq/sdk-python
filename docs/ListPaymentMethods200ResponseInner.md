# ListPaymentMethods200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**card** | [**ListPaymentMethods200ResponseInnerCard**](ListPaymentMethods200ResponseInnerCard.md) |  | [optional] 

## Example

```python
from saved.models.list_payment_methods200_response_inner import ListPaymentMethods200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListPaymentMethods200ResponseInner from a JSON string
list_payment_methods200_response_inner_instance = ListPaymentMethods200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(ListPaymentMethods200ResponseInner.to_json())

# convert the object into a dict
list_payment_methods200_response_inner_dict = list_payment_methods200_response_inner_instance.to_dict()
# create an instance of ListPaymentMethods200ResponseInner from a dict
list_payment_methods200_response_inner_from_dict = ListPaymentMethods200ResponseInner.from_dict(list_payment_methods200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



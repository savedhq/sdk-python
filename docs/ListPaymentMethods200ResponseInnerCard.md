# ListPaymentMethods200ResponseInnerCard


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**brand** | **str** |  | [optional] 
**last4** | **str** |  | [optional] 
**exp_month** | **int** |  | [optional] 
**exp_year** | **int** |  | [optional] 

## Example

```python
from saved.models.list_payment_methods200_response_inner_card import ListPaymentMethods200ResponseInnerCard

# TODO update the JSON string below
json = "{}"
# create an instance of ListPaymentMethods200ResponseInnerCard from a JSON string
list_payment_methods200_response_inner_card_instance = ListPaymentMethods200ResponseInnerCard.from_json(json)
# print the JSON string representation of the object
print(ListPaymentMethods200ResponseInnerCard.to_json())

# convert the object into a dict
list_payment_methods200_response_inner_card_dict = list_payment_methods200_response_inner_card_instance.to_dict()
# create an instance of ListPaymentMethods200ResponseInnerCard from a dict
list_payment_methods200_response_inner_card_from_dict = ListPaymentMethods200ResponseInnerCard.from_dict(list_payment_methods200_response_inner_card_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# GetSubscription200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**current_period_start** | **datetime** |  | [optional] 
**current_period_end** | **datetime** |  | [optional] 

## Example

```python
from saved.models.get_subscription200_response import GetSubscription200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetSubscription200Response from a JSON string
get_subscription200_response_instance = GetSubscription200Response.from_json(json)
# print the JSON string representation of the object
print(GetSubscription200Response.to_json())

# convert the object into a dict
get_subscription200_response_dict = get_subscription200_response_instance.to_dict()
# create an instance of GetSubscription200Response from a dict
get_subscription200_response_from_dict = GetSubscription200Response.from_dict(get_subscription200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



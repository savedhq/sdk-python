# GetCurrentUsage200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**storage_gb** | **float** |  | [optional] 
**computation_seconds** | **float** |  | [optional] 
**transfer_gb** | **float** |  | [optional] 
**period_start** | **datetime** |  | [optional] 
**period_end** | **datetime** |  | [optional] 

## Example

```python
from saved.models.get_current_usage200_response import GetCurrentUsage200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetCurrentUsage200Response from a JSON string
get_current_usage200_response_instance = GetCurrentUsage200Response.from_json(json)
# print the JSON string representation of the object
print(GetCurrentUsage200Response.to_json())

# convert the object into a dict
get_current_usage200_response_dict = get_current_usage200_response_instance.to_dict()
# create an instance of GetCurrentUsage200Response from a dict
get_current_usage200_response_from_dict = GetCurrentUsage200Response.from_dict(get_current_usage200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



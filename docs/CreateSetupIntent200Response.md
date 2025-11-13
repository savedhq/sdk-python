# CreateSetupIntent200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_secret** | **str** |  | [optional] 
**id** | **str** |  | [optional] 

## Example

```python
from saved.models.create_setup_intent200_response import CreateSetupIntent200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSetupIntent200Response from a JSON string
create_setup_intent200_response_instance = CreateSetupIntent200Response.from_json(json)
# print the JSON string representation of the object
print(CreateSetupIntent200Response.to_json())

# convert the object into a dict
create_setup_intent200_response_dict = create_setup_intent200_response_instance.to_dict()
# create an instance of CreateSetupIntent200Response from a dict
create_setup_intent200_response_from_dict = CreateSetupIntent200Response.from_dict(create_setup_intent200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



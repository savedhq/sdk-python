# ClientAgentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**workspace_id** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_secret** | **str** |  | [optional] 
**scope** | **str** |  | [optional] 
**public_url** | **str** |  | [optional] 
**status** | **str** | Current status of the agent | [optional] 
**certificate_cn** | **str** | Certificate common name | [optional] 
**certificate_expiry** | **datetime** | Certificate expiration date | [optional] 
**temporal_namespace** | **str** | Temporal namespace for this agent | [optional] 
**temporal_task_queue** | **str** | Temporal task queue name | [optional] 
**temporal_host_port** | **str** | Temporal host and port | [optional] 

## Example

```python
from saved.models.client_agent_response import ClientAgentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ClientAgentResponse from a JSON string
client_agent_response_instance = ClientAgentResponse.from_json(json)
# print the JSON string representation of the object
print(ClientAgentResponse.to_json())

# convert the object into a dict
client_agent_response_dict = client_agent_response_instance.to_dict()
# create an instance of ClientAgentResponse from a dict
client_agent_response_from_dict = ClientAgentResponse.from_dict(client_agent_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



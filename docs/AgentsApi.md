# saved.AgentsApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_agent**](AgentsApi.md#create_agent) | **POST** /workspaces/{workspace_id}/agents | Create agent
[**delete_agent**](AgentsApi.md#delete_agent) | **DELETE** /workspaces/{workspace_id}/agents/{id} | Delete agent
[**get_agent**](AgentsApi.md#get_agent) | **GET** /workspaces/{workspace_id}/agents/{id} | Get agent by ID
[**list_agents**](AgentsApi.md#list_agents) | **GET** /workspaces/{workspace_id}/agents | List agents
[**update_agent**](AgentsApi.md#update_agent) | **PATCH** /workspaces/{workspace_id}/agents/{id} | Update agent


# **create_agent**
> ListAgents200ResponseAllOfItemsInner create_agent(workspace_id, create_workspace_request)

Create agent

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_workspace_request import CreateWorkspaceRequest
from saved.models.list_agents200_response_all_of_items_inner import ListAgents200ResponseAllOfItemsInner
from saved.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8080/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = saved.Configuration(
    host = "http://localhost:8080/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = saved.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with saved.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = saved.AgentsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    create_workspace_request = saved.CreateWorkspaceRequest() # CreateWorkspaceRequest | 

    try:
        # Create agent
        api_response = api_instance.create_agent(workspace_id, create_workspace_request)
        print("The response of AgentsApi->create_agent:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AgentsApi->create_agent: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **create_workspace_request** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md)|  | 

### Return type

[**ListAgents200ResponseAllOfItemsInner**](ListAgents200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Agent created |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_agent**
> delete_agent(workspace_id, id)

Delete agent

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8080/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = saved.Configuration(
    host = "http://localhost:8080/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = saved.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with saved.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = saved.AgentsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    id = 'id_example' # str | 

    try:
        # Delete agent
        api_instance.delete_agent(workspace_id, id)
    except Exception as e:
        print("Exception when calling AgentsApi->delete_agent: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Agent deleted |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_agent**
> ListAgents200ResponseAllOfItemsInner get_agent(workspace_id, id)

Get agent by ID

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_agents200_response_all_of_items_inner import ListAgents200ResponseAllOfItemsInner
from saved.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8080/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = saved.Configuration(
    host = "http://localhost:8080/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = saved.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with saved.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = saved.AgentsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    id = 'id_example' # str | 

    try:
        # Get agent by ID
        api_response = api_instance.get_agent(workspace_id, id)
        print("The response of AgentsApi->get_agent:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AgentsApi->get_agent: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **id** | **str**|  | 

### Return type

[**ListAgents200ResponseAllOfItemsInner**](ListAgents200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Agent details |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_agents**
> ListAgents200Response list_agents(workspace_id, page=page, limit=limit)

List agents

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_agents200_response import ListAgents200Response
from saved.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8080/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = saved.Configuration(
    host = "http://localhost:8080/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = saved.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with saved.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = saved.AgentsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List agents
        api_response = api_instance.list_agents(workspace_id, page=page, limit=limit)
        print("The response of AgentsApi->list_agents:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AgentsApi->list_agents: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 10]

### Return type

[**ListAgents200Response**](ListAgents200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of agents |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_agent**
> ListAgents200ResponseAllOfItemsInner update_agent(workspace_id, id, create_workspace_request)

Update agent

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_workspace_request import CreateWorkspaceRequest
from saved.models.list_agents200_response_all_of_items_inner import ListAgents200ResponseAllOfItemsInner
from saved.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8080/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = saved.Configuration(
    host = "http://localhost:8080/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = saved.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with saved.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = saved.AgentsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    id = 'id_example' # str | 
    create_workspace_request = saved.CreateWorkspaceRequest() # CreateWorkspaceRequest | 

    try:
        # Update agent
        api_response = api_instance.update_agent(workspace_id, id, create_workspace_request)
        print("The response of AgentsApi->update_agent:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AgentsApi->update_agent: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **id** | **str**|  | 
 **create_workspace_request** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md)|  | 

### Return type

[**ListAgents200ResponseAllOfItemsInner**](ListAgents200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Agent updated |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


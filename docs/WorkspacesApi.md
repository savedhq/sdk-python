# saved.WorkspacesApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_workspace**](WorkspacesApi.md#create_workspace) | **POST** /workspaces | Create workspace
[**delete_workspace**](WorkspacesApi.md#delete_workspace) | **DELETE** /workspaces/{workspace_id} | Delete workspace
[**get_workspace**](WorkspacesApi.md#get_workspace) | **GET** /workspaces/{workspace_id} | Get workspace by ID
[**list_workspaces**](WorkspacesApi.md#list_workspaces) | **GET** /workspaces | List workspaces
[**update_workspace**](WorkspacesApi.md#update_workspace) | **PATCH** /workspaces/{workspace_id} | Update workspace


# **create_workspace**
> ListWorkspaces200ResponseAllOfItemsInner create_workspace(create_workspace_request)

Create workspace

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_workspace_request import CreateWorkspaceRequest
from saved.models.list_workspaces200_response_all_of_items_inner import ListWorkspaces200ResponseAllOfItemsInner
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
    api_instance = saved.WorkspacesApi(api_client)
    create_workspace_request = saved.CreateWorkspaceRequest() # CreateWorkspaceRequest | 

    try:
        # Create workspace
        api_response = api_instance.create_workspace(create_workspace_request)
        print("The response of WorkspacesApi->create_workspace:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->create_workspace: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_workspace_request** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md)|  | 

### Return type

[**ListWorkspaces200ResponseAllOfItemsInner**](ListWorkspaces200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Workspace created |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_workspace**
> delete_workspace(workspace_id)

Delete workspace

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
    api_instance = saved.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 

    try:
        # Delete workspace
        api_instance.delete_workspace(workspace_id)
    except Exception as e:
        print("Exception when calling WorkspacesApi->delete_workspace: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 

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
**204** | Workspace deleted |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_workspace**
> ListWorkspaces200ResponseAllOfItemsInner get_workspace(workspace_id)

Get workspace by ID

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_workspaces200_response_all_of_items_inner import ListWorkspaces200ResponseAllOfItemsInner
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
    api_instance = saved.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 

    try:
        # Get workspace by ID
        api_response = api_instance.get_workspace(workspace_id)
        print("The response of WorkspacesApi->get_workspace:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->get_workspace: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 

### Return type

[**ListWorkspaces200ResponseAllOfItemsInner**](ListWorkspaces200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Workspace details |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_workspaces**
> ListWorkspaces200Response list_workspaces(page=page, limit=limit)

List workspaces

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_workspaces200_response import ListWorkspaces200Response
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
    api_instance = saved.WorkspacesApi(api_client)
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List workspaces
        api_response = api_instance.list_workspaces(page=page, limit=limit)
        print("The response of WorkspacesApi->list_workspaces:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->list_workspaces: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 10]

### Return type

[**ListWorkspaces200Response**](ListWorkspaces200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of workspaces |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_workspace**
> ListWorkspaces200ResponseAllOfItemsInner update_workspace(workspace_id, create_workspace_request)

Update workspace

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_workspace_request import CreateWorkspaceRequest
from saved.models.list_workspaces200_response_all_of_items_inner import ListWorkspaces200ResponseAllOfItemsInner
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
    api_instance = saved.WorkspacesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    create_workspace_request = saved.CreateWorkspaceRequest() # CreateWorkspaceRequest | 

    try:
        # Update workspace
        api_response = api_instance.update_workspace(workspace_id, create_workspace_request)
        print("The response of WorkspacesApi->update_workspace:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkspacesApi->update_workspace: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **create_workspace_request** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md)|  | 

### Return type

[**ListWorkspaces200ResponseAllOfItemsInner**](ListWorkspaces200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Workspace updated |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


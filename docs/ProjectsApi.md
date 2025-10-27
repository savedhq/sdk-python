# saved.ProjectsApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_project_signal**](ProjectsApi.md#add_project_signal) | **POST** /workspaces/{workspace_id}/projects/{project_id}/signals | Add signal to vault
[**add_project_storage**](ProjectsApi.md#add_project_storage) | **POST** /workspaces/{workspace_id}/projects/{project_id}/storages | Add storage to vault
[**create_project**](ProjectsApi.md#create_project) | **POST** /workspaces/{workspace_id}/projects | Create vault
[**delete_project**](ProjectsApi.md#delete_project) | **DELETE** /workspaces/{workspace_id}/projects/{project_id} | Delete vault
[**delete_project_key**](ProjectsApi.md#delete_project_key) | **DELETE** /workspaces/{workspace_id}/projects/{project_id}/key | Delete vault encryption key
[**delete_project_signal**](ProjectsApi.md#delete_project_signal) | **DELETE** /workspaces/{workspace_id}/projects/{project_id}/signals/{signal_id} | Remove signal from vault
[**delete_project_storage**](ProjectsApi.md#delete_project_storage) | **DELETE** /workspaces/{workspace_id}/projects/{project_id}/storages/{storage_id} | Remove storage from vault
[**get_project**](ProjectsApi.md#get_project) | **GET** /workspaces/{workspace_id}/projects/{project_id} | Get vault by ID
[**get_project_key**](ProjectsApi.md#get_project_key) | **GET** /workspaces/{workspace_id}/projects/{project_id}/key | Get vault encryption key
[**list_project_signals**](ProjectsApi.md#list_project_signals) | **GET** /workspaces/{workspace_id}/projects/{project_id}/signals | List vault signals
[**list_project_storages**](ProjectsApi.md#list_project_storages) | **GET** /workspaces/{workspace_id}/projects/{project_id}/storages | List vault storages
[**list_projects**](ProjectsApi.md#list_projects) | **GET** /workspaces/{workspace_id}/projects | List vaults
[**set_project_key**](ProjectsApi.md#set_project_key) | **PUT** /workspaces/{workspace_id}/projects/{project_id}/key | Set vault encryption key
[**update_project**](ProjectsApi.md#update_project) | **PATCH** /workspaces/{workspace_id}/projects/{project_id} | Update vault


# **add_project_signal**
> ListSignals200ResponseAllOfItemsInner add_project_signal(workspace_id, project_id, add_project_signal_request)

Add signal to vault

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.add_project_signal_request import AddProjectSignalRequest
from saved.models.list_signals200_response_all_of_items_inner import ListSignals200ResponseAllOfItemsInner
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    add_project_signal_request = saved.AddProjectSignalRequest() # AddProjectSignalRequest | 

    try:
        # Add signal to vault
        api_response = api_instance.add_project_signal(workspace_id, project_id, add_project_signal_request)
        print("The response of ProjectsApi->add_project_signal:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->add_project_signal: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **add_project_signal_request** | [**AddProjectSignalRequest**](AddProjectSignalRequest.md)|  | 

### Return type

[**ListSignals200ResponseAllOfItemsInner**](ListSignals200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Signal added to vault |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **add_project_storage**
> ListStorages200ResponseAllOfItemsInner add_project_storage(workspace_id, project_id, add_project_storage_request)

Add storage to vault

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.add_project_storage_request import AddProjectStorageRequest
from saved.models.list_storages200_response_all_of_items_inner import ListStorages200ResponseAllOfItemsInner
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    add_project_storage_request = saved.AddProjectStorageRequest() # AddProjectStorageRequest | 

    try:
        # Add storage to vault
        api_response = api_instance.add_project_storage(workspace_id, project_id, add_project_storage_request)
        print("The response of ProjectsApi->add_project_storage:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->add_project_storage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **add_project_storage_request** | [**AddProjectStorageRequest**](AddProjectStorageRequest.md)|  | 

### Return type

[**ListStorages200ResponseAllOfItemsInner**](ListStorages200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Storage added to vault |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_project**
> ListProjects200ResponseAllOfItemsInner create_project(workspace_id, create_project_request)

Create vault

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_project_request import CreateProjectRequest
from saved.models.list_projects200_response_all_of_items_inner import ListProjects200ResponseAllOfItemsInner
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    create_project_request = saved.CreateProjectRequest() # CreateProjectRequest | 

    try:
        # Create vault
        api_response = api_instance.create_project(workspace_id, create_project_request)
        print("The response of ProjectsApi->create_project:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->create_project: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **create_project_request** | [**CreateProjectRequest**](CreateProjectRequest.md)|  | 

### Return type

[**ListProjects200ResponseAllOfItemsInner**](ListProjects200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Project created |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_project**
> delete_project(workspace_id, project_id)

Delete vault

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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 

    try:
        # Delete vault
        api_instance.delete_project(workspace_id, project_id)
    except Exception as e:
        print("Exception when calling ProjectsApi->delete_project: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 

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
**204** | Project deleted |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_project_key**
> delete_project_key(workspace_id, project_id)

Delete vault encryption key

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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 

    try:
        # Delete vault encryption key
        api_instance.delete_project_key(workspace_id, project_id)
    except Exception as e:
        print("Exception when calling ProjectsApi->delete_project_key: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 

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
**204** | Project key deleted |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_project_signal**
> delete_project_signal(workspace_id, project_id, signal_id)

Remove signal from vault

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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    signal_id = 'signal_id_example' # str | 

    try:
        # Remove signal from vault
        api_instance.delete_project_signal(workspace_id, project_id, signal_id)
    except Exception as e:
        print("Exception when calling ProjectsApi->delete_project_signal: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **signal_id** | **str**|  | 

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
**204** | Signal removed from vault |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_project_storage**
> delete_project_storage(workspace_id, project_id, storage_id)

Remove storage from vault

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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    storage_id = 'storage_id_example' # str | 

    try:
        # Remove storage from vault
        api_instance.delete_project_storage(workspace_id, project_id, storage_id)
    except Exception as e:
        print("Exception when calling ProjectsApi->delete_project_storage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **storage_id** | **str**|  | 

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
**204** | Storage removed from vault |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_project**
> ListProjects200ResponseAllOfItemsInner get_project(workspace_id, project_id)

Get vault by ID

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_projects200_response_all_of_items_inner import ListProjects200ResponseAllOfItemsInner
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 

    try:
        # Get vault by ID
        api_response = api_instance.get_project(workspace_id, project_id)
        print("The response of ProjectsApi->get_project:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->get_project: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 

### Return type

[**ListProjects200ResponseAllOfItemsInner**](ListProjects200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Project details |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_project_key**
> ListKeys200ResponseAllOfItemsInner get_project_key(workspace_id, project_id)

Get vault encryption key

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_keys200_response_all_of_items_inner import ListKeys200ResponseAllOfItemsInner
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 

    try:
        # Get vault encryption key
        api_response = api_instance.get_project_key(workspace_id, project_id)
        print("The response of ProjectsApi->get_project_key:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->get_project_key: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 

### Return type

[**ListKeys200ResponseAllOfItemsInner**](ListKeys200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Project key details |  -  |
**204** | No key set for this vault |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_project_signals**
> ListSignals200Response list_project_signals(workspace_id, project_id, page=page, limit=limit)

List vault signals

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_signals200_response import ListSignals200Response
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List vault signals
        api_response = api_instance.list_project_signals(workspace_id, project_id, page=page, limit=limit)
        print("The response of ProjectsApi->list_project_signals:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->list_project_signals: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 10]

### Return type

[**ListSignals200Response**](ListSignals200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of vault signals |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_project_storages**
> ListStorages200Response list_project_storages(workspace_id, project_id, page=page, limit=limit)

List vault storages

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_storages200_response import ListStorages200Response
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List vault storages
        api_response = api_instance.list_project_storages(workspace_id, project_id, page=page, limit=limit)
        print("The response of ProjectsApi->list_project_storages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->list_project_storages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 10]

### Return type

[**ListStorages200Response**](ListStorages200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of vault storages |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_projects**
> ListProjects200Response list_projects(workspace_id, page=page, limit=limit)

List vaults

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_projects200_response import ListProjects200Response
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List vaults
        api_response = api_instance.list_projects(workspace_id, page=page, limit=limit)
        print("The response of ProjectsApi->list_projects:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->list_projects: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 10]

### Return type

[**ListProjects200Response**](ListProjects200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of vaults |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_project_key**
> ListKeys200ResponseAllOfItemsInner set_project_key(workspace_id, project_id, set_project_key_request)

Set vault encryption key

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_keys200_response_all_of_items_inner import ListKeys200ResponseAllOfItemsInner
from saved.models.set_project_key_request import SetProjectKeyRequest
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    set_project_key_request = saved.SetProjectKeyRequest() # SetProjectKeyRequest | 

    try:
        # Set vault encryption key
        api_response = api_instance.set_project_key(workspace_id, project_id, set_project_key_request)
        print("The response of ProjectsApi->set_project_key:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->set_project_key: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **set_project_key_request** | [**SetProjectKeyRequest**](SetProjectKeyRequest.md)|  | 

### Return type

[**ListKeys200ResponseAllOfItemsInner**](ListKeys200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Project key set |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_project**
> ListProjects200ResponseAllOfItemsInner update_project(workspace_id, project_id, update_project_request)

Update vault

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_projects200_response_all_of_items_inner import ListProjects200ResponseAllOfItemsInner
from saved.models.update_project_request import UpdateProjectRequest
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
    api_instance = saved.ProjectsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    update_project_request = saved.UpdateProjectRequest() # UpdateProjectRequest | 

    try:
        # Update vault
        api_response = api_instance.update_project(workspace_id, project_id, update_project_request)
        print("The response of ProjectsApi->update_project:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->update_project: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **update_project_request** | [**UpdateProjectRequest**](UpdateProjectRequest.md)|  | 

### Return type

[**ListProjects200ResponseAllOfItemsInner**](ListProjects200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Project updated |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


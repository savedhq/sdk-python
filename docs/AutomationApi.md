# saved.AutomationApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_auto_backup**](AutomationApi.md#create_auto_backup) | **POST** /workspaces/{workspace_id}/projects/{project_id}/auto | Create automated backup
[**delete_auto_backup**](AutomationApi.md#delete_auto_backup) | **DELETE** /workspaces/{workspace_id}/projects/{project_id}/auto/{job_id} | Delete automated backup
[**get_auto_backup**](AutomationApi.md#get_auto_backup) | **GET** /workspaces/{workspace_id}/projects/{project_id}/auto/{job_id} | Get automated backup by ID
[**get_auto_backup_history_details**](AutomationApi.md#get_auto_backup_history_details) | **GET** /workspaces/{workspace_id}/projects/{project_id}/auto/{job_id}/runs/{run_id} | Get workflow execution event history details
[**list_auto_backup**](AutomationApi.md#list_auto_backup) | **GET** /workspaces/{workspace_id}/projects/{project_id}/auto | List all automated backups
[**list_auto_backup_executions**](AutomationApi.md#list_auto_backup_executions) | **GET** /workspaces/{workspace_id}/projects/{project_id}/auto/{job_id}/runs | List automated backup workflow executions
[**update_auto_backup**](AutomationApi.md#update_auto_backup) | **PATCH** /workspaces/{workspace_id}/projects/{project_id}/auto/{job_id} | Update automated backup


# **create_auto_backup**
> ListAutoBackup200ResponseAllOfItemsInner create_auto_backup(workspace_id, project_id, create_auto_backup_request)

Create automated backup

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_auto_backup_request import CreateAutoBackupRequest
from saved.models.list_auto_backup200_response_all_of_items_inner import ListAutoBackup200ResponseAllOfItemsInner
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
    api_instance = saved.AutomationApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    create_auto_backup_request = saved.CreateAutoBackupRequest() # CreateAutoBackupRequest | 

    try:
        # Create automated backup
        api_response = api_instance.create_auto_backup(workspace_id, project_id, create_auto_backup_request)
        print("The response of AutomationApi->create_auto_backup:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->create_auto_backup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **create_auto_backup_request** | [**CreateAutoBackupRequest**](CreateAutoBackupRequest.md)|  | 

### Return type

[**ListAutoBackup200ResponseAllOfItemsInner**](ListAutoBackup200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Automated backup created |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_auto_backup**
> delete_auto_backup(workspace_id, project_id, job_id)

Delete automated backup

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
    api_instance = saved.AutomationApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Delete automated backup
        api_instance.delete_auto_backup(workspace_id, project_id, job_id)
    except Exception as e:
        print("Exception when calling AutomationApi->delete_auto_backup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **job_id** | **str**|  | 

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
**204** | Automated backup deleted |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_auto_backup**
> ListAutoBackup200ResponseAllOfItemsInner get_auto_backup(workspace_id, project_id, job_id)

Get automated backup by ID

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_auto_backup200_response_all_of_items_inner import ListAutoBackup200ResponseAllOfItemsInner
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
    api_instance = saved.AutomationApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # Get automated backup by ID
        api_response = api_instance.get_auto_backup(workspace_id, project_id, job_id)
        print("The response of AutomationApi->get_auto_backup:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->get_auto_backup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **job_id** | **str**|  | 

### Return type

[**ListAutoBackup200ResponseAllOfItemsInner**](ListAutoBackup200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Automated backup details |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_auto_backup_history_details**
> GetAutoBackupHistoryDetails200Response get_auto_backup_history_details(workspace_id, project_id, job_id, run_id)

Get workflow execution event history details

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.get_auto_backup_history_details200_response import GetAutoBackupHistoryDetails200Response
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
    api_instance = saved.AutomationApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    job_id = 'job_id_example' # str | 
    run_id = 'run_id_example' # str | 

    try:
        # Get workflow execution event history details
        api_response = api_instance.get_auto_backup_history_details(workspace_id, project_id, job_id, run_id)
        print("The response of AutomationApi->get_auto_backup_history_details:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->get_auto_backup_history_details: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **job_id** | **str**|  | 
 **run_id** | **str**|  | 

### Return type

[**GetAutoBackupHistoryDetails200Response**](GetAutoBackupHistoryDetails200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Workflow execution event history |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_auto_backup**
> ListAutoBackup200Response list_auto_backup(workspace_id, project_id, page=page, limit=limit)

List all automated backups

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_auto_backup200_response import ListAutoBackup200Response
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
    api_instance = saved.AutomationApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List all automated backups
        api_response = api_instance.list_auto_backup(workspace_id, project_id, page=page, limit=limit)
        print("The response of AutomationApi->list_auto_backup:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->list_auto_backup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 10]

### Return type

[**ListAutoBackup200Response**](ListAutoBackup200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of automated backups (both worker and agent) |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_auto_backup_executions**
> ListAutoBackupExecutions200Response list_auto_backup_executions(workspace_id, project_id, job_id)

List automated backup workflow executions

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_auto_backup_executions200_response import ListAutoBackupExecutions200Response
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
    api_instance = saved.AutomationApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    job_id = 'job_id_example' # str | 

    try:
        # List automated backup workflow executions
        api_response = api_instance.list_auto_backup_executions(workspace_id, project_id, job_id)
        print("The response of AutomationApi->list_auto_backup_executions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->list_auto_backup_executions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **job_id** | **str**|  | 

### Return type

[**ListAutoBackupExecutions200Response**](ListAutoBackupExecutions200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of workflow executions |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_auto_backup**
> ListAutoBackup200ResponseAllOfItemsInner update_auto_backup(workspace_id, project_id, job_id, update_auto_backup_request)

Update automated backup

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_auto_backup200_response_all_of_items_inner import ListAutoBackup200ResponseAllOfItemsInner
from saved.models.update_auto_backup_request import UpdateAutoBackupRequest
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
    api_instance = saved.AutomationApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    job_id = 'job_id_example' # str | 
    update_auto_backup_request = saved.UpdateAutoBackupRequest() # UpdateAutoBackupRequest | 

    try:
        # Update automated backup
        api_response = api_instance.update_auto_backup(workspace_id, project_id, job_id, update_auto_backup_request)
        print("The response of AutomationApi->update_auto_backup:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AutomationApi->update_auto_backup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **job_id** | **str**|  | 
 **update_auto_backup_request** | [**UpdateAutoBackupRequest**](UpdateAutoBackupRequest.md)|  | 

### Return type

[**ListAutoBackup200ResponseAllOfItemsInner**](ListAutoBackup200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Automated backup updated |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


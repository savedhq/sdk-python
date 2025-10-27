# saved.BackupsApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**confirm_backup_uploaded**](BackupsApi.md#confirm_backup_uploaded) | **POST** /workspaces/{workspace_id}/projects/{project_id}/backups/{backup_id}/confirm | Confirm backup uploaded
[**create_backup**](BackupsApi.md#create_backup) | **POST** /workspaces/{workspace_id}/projects/{project_id}/backups | Create backup (request upload)
[**get_backup**](BackupsApi.md#get_backup) | **GET** /workspaces/{workspace_id}/projects/{project_id}/backups/{backup_id} | Get backup by ID
[**list_backups**](BackupsApi.md#list_backups) | **GET** /workspaces/{workspace_id}/projects/{project_id}/backups | List backups
[**request_backup_copy**](BackupsApi.md#request_backup_copy) | **POST** /workspaces/{workspace_id}/projects/{project_id}/backups/{backup_id}/download | Request backup copy for download


# **confirm_backup_uploaded**
> ConfirmBackupUploaded200Response confirm_backup_uploaded(workspace_id, project_id, backup_id, confirm_backup_uploaded_request)

Confirm backup uploaded

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.confirm_backup_uploaded200_response import ConfirmBackupUploaded200Response
from saved.models.confirm_backup_uploaded_request import ConfirmBackupUploadedRequest
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
    api_instance = saved.BackupsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    backup_id = 'backup_id_example' # str | 
    confirm_backup_uploaded_request = saved.ConfirmBackupUploadedRequest() # ConfirmBackupUploadedRequest | 

    try:
        # Confirm backup uploaded
        api_response = api_instance.confirm_backup_uploaded(workspace_id, project_id, backup_id, confirm_backup_uploaded_request)
        print("The response of BackupsApi->confirm_backup_uploaded:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackupsApi->confirm_backup_uploaded: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **backup_id** | **str**|  | 
 **confirm_backup_uploaded_request** | [**ConfirmBackupUploadedRequest**](ConfirmBackupUploadedRequest.md)|  | 

### Return type

[**ConfirmBackupUploaded200Response**](ConfirmBackupUploaded200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Backup confirmed |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_backup**
> ListBackups200ResponseAllOfItemsInner create_backup(workspace_id, project_id, create_backup_request)

Create backup (request upload)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_backup_request import CreateBackupRequest
from saved.models.list_backups200_response_all_of_items_inner import ListBackups200ResponseAllOfItemsInner
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
    api_instance = saved.BackupsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    create_backup_request = saved.CreateBackupRequest() # CreateBackupRequest | 

    try:
        # Create backup (request upload)
        api_response = api_instance.create_backup(workspace_id, project_id, create_backup_request)
        print("The response of BackupsApi->create_backup:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackupsApi->create_backup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **create_backup_request** | [**CreateBackupRequest**](CreateBackupRequest.md)|  | 

### Return type

[**ListBackups200ResponseAllOfItemsInner**](ListBackups200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Backup created |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_backup**
> ListBackups200ResponseAllOfItemsInner get_backup(workspace_id, project_id, backup_id)

Get backup by ID

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_backups200_response_all_of_items_inner import ListBackups200ResponseAllOfItemsInner
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
    api_instance = saved.BackupsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    backup_id = 'backup_id_example' # str | 

    try:
        # Get backup by ID
        api_response = api_instance.get_backup(workspace_id, project_id, backup_id)
        print("The response of BackupsApi->get_backup:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackupsApi->get_backup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **backup_id** | **str**|  | 

### Return type

[**ListBackups200ResponseAllOfItemsInner**](ListBackups200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Backup details |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_backups**
> ListBackups200Response list_backups(workspace_id, project_id, page=page, limit=limit)

List backups

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_backups200_response import ListBackups200Response
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
    api_instance = saved.BackupsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List backups
        api_response = api_instance.list_backups(workspace_id, project_id, page=page, limit=limit)
        print("The response of BackupsApi->list_backups:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackupsApi->list_backups: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 10]

### Return type

[**ListBackups200Response**](ListBackups200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of backups |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **request_backup_copy**
> request_backup_copy(workspace_id, project_id, backup_id)

Request backup copy for download

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
    api_instance = saved.BackupsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    project_id = 'project_id_example' # str | 
    backup_id = 'backup_id_example' # str | 

    try:
        # Request backup copy for download
        api_instance.request_backup_copy(workspace_id, project_id, backup_id)
    except Exception as e:
        print("Exception when calling BackupsApi->request_backup_copy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **project_id** | **str**|  | 
 **backup_id** | **str**|  | 

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
**200** | Backup copy requested |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


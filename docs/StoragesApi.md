# saved.StoragesApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_storage**](StoragesApi.md#create_storage) | **POST** /workspaces/{workspace_id}/storages | Create storage
[**delete_storage**](StoragesApi.md#delete_storage) | **DELETE** /workspaces/{workspace_id}/storages/{storage_id} | Delete storage
[**get_storage**](StoragesApi.md#get_storage) | **GET** /workspaces/{workspace_id}/storages/{storage_id} | Get storage by ID
[**list_storages**](StoragesApi.md#list_storages) | **GET** /workspaces/{workspace_id}/storages | List storages
[**update_storage**](StoragesApi.md#update_storage) | **PATCH** /workspaces/{workspace_id}/storages/{storage_id} | Update storage


# **create_storage**
> ListStorages200ResponseAllOfItemsInner create_storage(workspace_id, create_storage_request)

Create storage

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_storage_request import CreateStorageRequest
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
    api_instance = saved.StoragesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    create_storage_request = saved.CreateStorageRequest() # CreateStorageRequest | 

    try:
        # Create storage
        api_response = api_instance.create_storage(workspace_id, create_storage_request)
        print("The response of StoragesApi->create_storage:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StoragesApi->create_storage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **create_storage_request** | [**CreateStorageRequest**](CreateStorageRequest.md)|  | 

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
**201** | Storage created |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_storage**
> delete_storage(workspace_id, storage_id)

Delete storage

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
    api_instance = saved.StoragesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    storage_id = 'storage_id_example' # str | 

    try:
        # Delete storage
        api_instance.delete_storage(workspace_id, storage_id)
    except Exception as e:
        print("Exception when calling StoragesApi->delete_storage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
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
**204** | Storage deleted |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_storage**
> ListStorages200ResponseAllOfItemsInner get_storage(workspace_id, storage_id)

Get storage by ID

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
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
    api_instance = saved.StoragesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    storage_id = 'storage_id_example' # str | 

    try:
        # Get storage by ID
        api_response = api_instance.get_storage(workspace_id, storage_id)
        print("The response of StoragesApi->get_storage:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StoragesApi->get_storage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **storage_id** | **str**|  | 

### Return type

[**ListStorages200ResponseAllOfItemsInner**](ListStorages200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Storage details |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_storages**
> ListStorages200Response list_storages(workspace_id, page=page, limit=limit)

List storages

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
    api_instance = saved.StoragesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List storages
        api_response = api_instance.list_storages(workspace_id, page=page, limit=limit)
        print("The response of StoragesApi->list_storages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StoragesApi->list_storages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
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
**200** | List of storages |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_storage**
> ListStorages200ResponseAllOfItemsInner update_storage(workspace_id, storage_id, update_storage_request)

Update storage

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_storages200_response_all_of_items_inner import ListStorages200ResponseAllOfItemsInner
from saved.models.update_storage_request import UpdateStorageRequest
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
    api_instance = saved.StoragesApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    storage_id = 'storage_id_example' # str | 
    update_storage_request = saved.UpdateStorageRequest() # UpdateStorageRequest | 

    try:
        # Update storage
        api_response = api_instance.update_storage(workspace_id, storage_id, update_storage_request)
        print("The response of StoragesApi->update_storage:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StoragesApi->update_storage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **storage_id** | **str**|  | 
 **update_storage_request** | [**UpdateStorageRequest**](UpdateStorageRequest.md)|  | 

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
**200** | Storage updated |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


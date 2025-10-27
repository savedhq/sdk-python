# saved.KeysApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_key**](KeysApi.md#create_key) | **POST** /workspaces/{workspace_id}/keys | Create encryption key
[**delete_key**](KeysApi.md#delete_key) | **DELETE** /workspaces/{workspace_id}/keys/{key_id} | Delete encryption key
[**get_key**](KeysApi.md#get_key) | **GET** /workspaces/{workspace_id}/keys/{key_id} | Get encryption key by ID
[**list_keys**](KeysApi.md#list_keys) | **GET** /workspaces/{workspace_id}/keys | List encryption keys
[**update_key**](KeysApi.md#update_key) | **PATCH** /workspaces/{workspace_id}/keys/{key_id} | Update encryption key


# **create_key**
> ListKeys200ResponseAllOfItemsInner create_key(workspace_id, create_key_request)

Create encryption key

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_key_request import CreateKeyRequest
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
    api_instance = saved.KeysApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    create_key_request = saved.CreateKeyRequest() # CreateKeyRequest | 

    try:
        # Create encryption key
        api_response = api_instance.create_key(workspace_id, create_key_request)
        print("The response of KeysApi->create_key:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeysApi->create_key: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **create_key_request** | [**CreateKeyRequest**](CreateKeyRequest.md)|  | 

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
**200** | Key created |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_key**
> delete_key(workspace_id, key_id)

Delete encryption key

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
    api_instance = saved.KeysApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    key_id = 'key_id_example' # str | 

    try:
        # Delete encryption key
        api_instance.delete_key(workspace_id, key_id)
    except Exception as e:
        print("Exception when calling KeysApi->delete_key: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **key_id** | **str**|  | 

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
**204** | Key deleted |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_key**
> ListKeys200ResponseAllOfItemsInner get_key(workspace_id, key_id)

Get encryption key by ID

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
    api_instance = saved.KeysApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    key_id = 'key_id_example' # str | 

    try:
        # Get encryption key by ID
        api_response = api_instance.get_key(workspace_id, key_id)
        print("The response of KeysApi->get_key:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeysApi->get_key: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **key_id** | **str**|  | 

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
**200** | Key details |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_keys**
> ListKeys200Response list_keys(workspace_id, page=page, limit=limit)

List encryption keys

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_keys200_response import ListKeys200Response
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
    api_instance = saved.KeysApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List encryption keys
        api_response = api_instance.list_keys(workspace_id, page=page, limit=limit)
        print("The response of KeysApi->list_keys:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeysApi->list_keys: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 10]

### Return type

[**ListKeys200Response**](ListKeys200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of encryption keys |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_key**
> ListKeys200ResponseAllOfItemsInner update_key(workspace_id, key_id, create_workspace_request)

Update encryption key

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_workspace_request import CreateWorkspaceRequest
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
    api_instance = saved.KeysApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    key_id = 'key_id_example' # str | 
    create_workspace_request = saved.CreateWorkspaceRequest() # CreateWorkspaceRequest | 

    try:
        # Update encryption key
        api_response = api_instance.update_key(workspace_id, key_id, create_workspace_request)
        print("The response of KeysApi->update_key:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeysApi->update_key: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **key_id** | **str**|  | 
 **create_workspace_request** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md)|  | 

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
**200** | Key updated |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


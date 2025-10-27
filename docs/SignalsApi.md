# saved.SignalsApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_signal**](SignalsApi.md#create_signal) | **POST** /workspaces/{workspace_id}/signals | Create signal
[**delete_signal**](SignalsApi.md#delete_signal) | **DELETE** /workspaces/{workspace_id}/signals/{signal_id} | Delete signal
[**get_signal**](SignalsApi.md#get_signal) | **GET** /workspaces/{workspace_id}/signals/{signal_id} | Get signal by ID
[**list_signals**](SignalsApi.md#list_signals) | **GET** /workspaces/{workspace_id}/signals | List signals
[**update_signal**](SignalsApi.md#update_signal) | **PATCH** /workspaces/{workspace_id}/signals/{signal_id} | Update signal


# **create_signal**
> ListSignals200ResponseAllOfItemsInner create_signal(workspace_id, create_signal_request)

Create signal

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_signal_request import CreateSignalRequest
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
    api_instance = saved.SignalsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    create_signal_request = saved.CreateSignalRequest() # CreateSignalRequest | 

    try:
        # Create signal
        api_response = api_instance.create_signal(workspace_id, create_signal_request)
        print("The response of SignalsApi->create_signal:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SignalsApi->create_signal: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **create_signal_request** | [**CreateSignalRequest**](CreateSignalRequest.md)|  | 

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
**201** | Signal created |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_signal**
> delete_signal(workspace_id, signal_id)

Delete signal

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
    api_instance = saved.SignalsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    signal_id = 'signal_id_example' # str | 

    try:
        # Delete signal
        api_instance.delete_signal(workspace_id, signal_id)
    except Exception as e:
        print("Exception when calling SignalsApi->delete_signal: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
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
**204** | Signal deleted |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_signal**
> ListSignals200ResponseAllOfItemsInner get_signal(workspace_id, signal_id)

Get signal by ID

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
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
    api_instance = saved.SignalsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    signal_id = 'signal_id_example' # str | 

    try:
        # Get signal by ID
        api_response = api_instance.get_signal(workspace_id, signal_id)
        print("The response of SignalsApi->get_signal:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SignalsApi->get_signal: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **signal_id** | **str**|  | 

### Return type

[**ListSignals200ResponseAllOfItemsInner**](ListSignals200ResponseAllOfItemsInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Signal details |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_signals**
> ListSignals200Response list_signals(workspace_id, page=page, limit=limit)

List signals

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
    api_instance = saved.SignalsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    page = 1 # int |  (optional) (default to 1)
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List signals
        api_response = api_instance.list_signals(workspace_id, page=page, limit=limit)
        print("The response of SignalsApi->list_signals:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SignalsApi->list_signals: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
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
**200** | List of signals |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_signal**
> ListSignals200ResponseAllOfItemsInner update_signal(workspace_id, signal_id, update_signal_request)

Update signal

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_signals200_response_all_of_items_inner import ListSignals200ResponseAllOfItemsInner
from saved.models.update_signal_request import UpdateSignalRequest
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
    api_instance = saved.SignalsApi(api_client)
    workspace_id = 'workspace_id_example' # str | 
    signal_id = 'signal_id_example' # str | 
    update_signal_request = saved.UpdateSignalRequest() # UpdateSignalRequest | 

    try:
        # Update signal
        api_response = api_instance.update_signal(workspace_id, signal_id, update_signal_request)
        print("The response of SignalsApi->update_signal:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SignalsApi->update_signal: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspace_id** | **str**|  | 
 **signal_id** | **str**|  | 
 **update_signal_request** | [**UpdateSignalRequest**](UpdateSignalRequest.md)|  | 

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
**200** | Signal updated |  -  |
**400** | Bad request - validation error |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


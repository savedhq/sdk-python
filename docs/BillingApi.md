# saved.BillingApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_subscription**](BillingApi.md#cancel_subscription) | **DELETE** /workspaces/{id}/billing/subscription | Cancel subscription
[**create_portal_session**](BillingApi.md#create_portal_session) | **POST** /workspaces/{id}/billing/portal-session | Create Stripe customer portal session
[**create_setup_intent**](BillingApi.md#create_setup_intent) | **POST** /workspaces/{id}/billing/setup-intent | Create setup intent for payment method
[**get_current_usage**](BillingApi.md#get_current_usage) | **GET** /workspaces/{id}/billing/usage/current | Get current billing period usage
[**get_subscription**](BillingApi.md#get_subscription) | **GET** /workspaces/{id}/billing/subscription | Get subscription information
[**list_invoices**](BillingApi.md#list_invoices) | **GET** /workspaces/{id}/billing/invoices | List invoices
[**list_payment_methods**](BillingApi.md#list_payment_methods) | **GET** /workspaces/{id}/billing/payment-methods | List payment methods
[**remove_payment_method**](BillingApi.md#remove_payment_method) | **DELETE** /workspaces/{id}/billing/payment-methods/{pm_id} | Remove payment method
[**set_default_payment_method**](BillingApi.md#set_default_payment_method) | **POST** /workspaces/{id}/billing/payment-methods/{pm_id}/default | Set default payment method


# **cancel_subscription**
> ListWorkspaces401Response cancel_subscription(id)

Cancel subscription

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_workspaces401_response import ListWorkspaces401Response
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
    api_instance = saved.BillingApi(api_client)
    id = 'id_example' # str | 

    try:
        # Cancel subscription
        api_response = api_instance.cancel_subscription(id)
        print("The response of BillingApi->cancel_subscription:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->cancel_subscription: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**ListWorkspaces401Response**](ListWorkspaces401Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Subscription canceled |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_portal_session**
> CreatePortalSession200Response create_portal_session(id, create_portal_session_request)

Create Stripe customer portal session

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_portal_session200_response import CreatePortalSession200Response
from saved.models.create_portal_session_request import CreatePortalSessionRequest
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
    api_instance = saved.BillingApi(api_client)
    id = 'id_example' # str | 
    create_portal_session_request = saved.CreatePortalSessionRequest() # CreatePortalSessionRequest | 

    try:
        # Create Stripe customer portal session
        api_response = api_instance.create_portal_session(id, create_portal_session_request)
        print("The response of BillingApi->create_portal_session:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->create_portal_session: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **create_portal_session_request** | [**CreatePortalSessionRequest**](CreatePortalSessionRequest.md)|  | 

### Return type

[**CreatePortalSession200Response**](CreatePortalSession200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Portal session created |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_setup_intent**
> CreateSetupIntent200Response create_setup_intent(id)

Create setup intent for payment method

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.create_setup_intent200_response import CreateSetupIntent200Response
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
    api_instance = saved.BillingApi(api_client)
    id = 'id_example' # str | 

    try:
        # Create setup intent for payment method
        api_response = api_instance.create_setup_intent(id)
        print("The response of BillingApi->create_setup_intent:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->create_setup_intent: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**CreateSetupIntent200Response**](CreateSetupIntent200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Setup intent created |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_current_usage**
> GetCurrentUsage200Response get_current_usage(id)

Get current billing period usage

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.get_current_usage200_response import GetCurrentUsage200Response
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
    api_instance = saved.BillingApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get current billing period usage
        api_response = api_instance.get_current_usage(id)
        print("The response of BillingApi->get_current_usage:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_current_usage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**GetCurrentUsage200Response**](GetCurrentUsage200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Current usage details |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |
**403** | User not authorized for workspace billing |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_subscription**
> GetSubscription200Response get_subscription(id)

Get subscription information

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.get_subscription200_response import GetSubscription200Response
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
    api_instance = saved.BillingApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get subscription information
        api_response = api_instance.get_subscription(id)
        print("The response of BillingApi->get_subscription:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_subscription: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**GetSubscription200Response**](GetSubscription200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Subscription details |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_invoices**
> List[ListInvoices200ResponseInner] list_invoices(id, limit=limit)

List invoices

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_invoices200_response_inner import ListInvoices200ResponseInner
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
    api_instance = saved.BillingApi(api_client)
    id = 'id_example' # str | 
    limit = 10 # int |  (optional) (default to 10)

    try:
        # List invoices
        api_response = api_instance.list_invoices(id, limit=limit)
        print("The response of BillingApi->list_invoices:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->list_invoices: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **limit** | **int**|  | [optional] [default to 10]

### Return type

[**List[ListInvoices200ResponseInner]**](ListInvoices200ResponseInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of invoices |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_payment_methods**
> List[ListPaymentMethods200ResponseInner] list_payment_methods(id)

List payment methods

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_payment_methods200_response_inner import ListPaymentMethods200ResponseInner
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
    api_instance = saved.BillingApi(api_client)
    id = 'id_example' # str | 

    try:
        # List payment methods
        api_response = api_instance.list_payment_methods(id)
        print("The response of BillingApi->list_payment_methods:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->list_payment_methods: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**List[ListPaymentMethods200ResponseInner]**](ListPaymentMethods200ResponseInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of payment methods |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **remove_payment_method**
> ListWorkspaces401Response remove_payment_method(id, pm_id)

Remove payment method

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_workspaces401_response import ListWorkspaces401Response
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
    api_instance = saved.BillingApi(api_client)
    id = 'id_example' # str | 
    pm_id = 'pm_id_example' # str | 

    try:
        # Remove payment method
        api_response = api_instance.remove_payment_method(id, pm_id)
        print("The response of BillingApi->remove_payment_method:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->remove_payment_method: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **pm_id** | **str**|  | 

### Return type

[**ListWorkspaces401Response**](ListWorkspaces401Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Payment method removed |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_default_payment_method**
> ListWorkspaces401Response set_default_payment_method(id, pm_id)

Set default payment method

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import saved
from saved.models.list_workspaces401_response import ListWorkspaces401Response
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
    api_instance = saved.BillingApi(api_client)
    id = 'id_example' # str | 
    pm_id = 'pm_id_example' # str | 

    try:
        # Set default payment method
        api_response = api_instance.set_default_payment_method(id, pm_id)
        print("The response of BillingApi->set_default_payment_method:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->set_default_payment_method: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **pm_id** | **str**|  | 

### Return type

[**ListWorkspaces401Response**](ListWorkspaces401Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default payment method updated |  -  |
**401** | Unauthorized - invalid or missing authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


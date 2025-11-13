# saved.WebhooksApi

All URIs are relative to *http://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**handle_stripe_webhook**](WebhooksApi.md#handle_stripe_webhook) | **POST** /webhooks/stripe | Stripe webhook handler


# **handle_stripe_webhook**
> handle_stripe_webhook(body)

Stripe webhook handler

### Example


```python
import saved
from saved.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8080/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = saved.Configuration(
    host = "http://localhost:8080/v1"
)


# Enter a context with an instance of the API client
with saved.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = saved.WebhooksApi(api_client)
    body = None # object | 

    try:
        # Stripe webhook handler
        api_instance.handle_stripe_webhook(body)
    except Exception as e:
        print("Exception when calling WebhooksApi->handle_stripe_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Webhook processed |  -  |
**400** | Invalid webhook signature |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# seerr.OverrideruleApi

All URIs are relative to *http://localhost:5055/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_overriderule**](OverrideruleApi.md#create_overriderule) | **POST** /overrideRule | Create override rule
[**delete_overriderule**](OverrideruleApi.md#delete_overriderule) | **DELETE** /overrideRule/{ruleId} | Delete override rule by ID
[**list_overriderule**](OverrideruleApi.md#list_overriderule) | **GET** /overrideRule | Get override rules
[**update_overriderule**](OverrideruleApi.md#update_overriderule) | **PUT** /overrideRule/{ruleId} | Update override rule


# **create_overriderule**
> List[OverrideRule] create_overriderule()

Create override rule

Creates a new Override Rule from the request body.

### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
from seerr.models.override_rule import OverrideRule
from seerr.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5055/api/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = seerr.Configuration(
    host = "http://localhost:5055/api/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: apiKey
configuration.api_key['apiKey'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['apiKey'] = 'Bearer'

# Configure API key authorization: cookieAuth
configuration.api_key['cookieAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['cookieAuth'] = 'Bearer'

# Enter a context with an instance of the API client
with seerr.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = seerr.OverrideruleApi(api_client)

    try:
        # Create override rule
        api_response = api_instance.create_overriderule()
        print("The response of OverrideruleApi->create_overriderule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OverrideruleApi->create_overriderule: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[OverrideRule]**](OverrideRule.md)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**2XX** | Values were successfully created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_overriderule**
> OverrideRule delete_overriderule(rule_id)

Delete override rule by ID

Deletes the override rule with the provided ruleId.

### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
from seerr.models.override_rule import OverrideRule
from seerr.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5055/api/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = seerr.Configuration(
    host = "http://localhost:5055/api/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: apiKey
configuration.api_key['apiKey'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['apiKey'] = 'Bearer'

# Configure API key authorization: cookieAuth
configuration.api_key['cookieAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['cookieAuth'] = 'Bearer'

# Enter a context with an instance of the API client
with seerr.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = seerr.OverrideruleApi(api_client)
    rule_id = 3.4 # float | 

    try:
        # Delete override rule by ID
        api_response = api_instance.delete_overriderule(rule_id)
        print("The response of OverrideruleApi->delete_overriderule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OverrideruleApi->delete_overriderule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **float**|  | 

### Return type

[**OverrideRule**](OverrideRule.md)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**2XX** | Override rule successfully deleted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_overriderule**
> List[OverrideRule] list_overriderule()

Get override rules

Returns a list of all override rules with their conditions and settings

### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
from seerr.models.override_rule import OverrideRule
from seerr.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5055/api/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = seerr.Configuration(
    host = "http://localhost:5055/api/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: apiKey
configuration.api_key['apiKey'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['apiKey'] = 'Bearer'

# Configure API key authorization: cookieAuth
configuration.api_key['cookieAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['cookieAuth'] = 'Bearer'

# Enter a context with an instance of the API client
with seerr.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = seerr.OverrideruleApi(api_client)

    try:
        # Get override rules
        api_response = api_instance.list_overriderule()
        print("The response of OverrideruleApi->list_overriderule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OverrideruleApi->list_overriderule: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[OverrideRule]**](OverrideRule.md)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**2XX** | Override rules returned |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_overriderule**
> List[OverrideRule] update_overriderule(rule_id)

Update override rule

Updates an Override Rule from the request body.

### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
from seerr.models.override_rule import OverrideRule
from seerr.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5055/api/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = seerr.Configuration(
    host = "http://localhost:5055/api/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: apiKey
configuration.api_key['apiKey'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['apiKey'] = 'Bearer'

# Configure API key authorization: cookieAuth
configuration.api_key['cookieAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['cookieAuth'] = 'Bearer'

# Enter a context with an instance of the API client
with seerr.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = seerr.OverrideruleApi(api_client)
    rule_id = 3.4 # float | 

    try:
        # Update override rule
        api_response = api_instance.update_overriderule(rule_id)
        print("The response of OverrideruleApi->update_overriderule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OverrideruleApi->update_overriderule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **float**|  | 

### Return type

[**List[OverrideRule]**](OverrideRule.md)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**2XX** | Values were successfully updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


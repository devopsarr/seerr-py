# seerr.WatchlistApi

All URIs are relative to *http://localhost:5055/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_watchlist**](WatchlistApi.md#create_watchlist) | **POST** /watchlist | Add media to watchlist
[**delete_watchlist**](WatchlistApi.md#delete_watchlist) | **DELETE** /watchlist/{tmdbId} | Delete watchlist item


# **create_watchlist**
> Watchlist create_watchlist(watchlist)

Add media to watchlist

### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
from seerr.models.watchlist import Watchlist
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
    api_instance = seerr.WatchlistApi(api_client)
    watchlist = seerr.Watchlist() # Watchlist | 

    try:
        # Add media to watchlist
        api_response = api_instance.create_watchlist(watchlist)
        print("The response of WatchlistApi->create_watchlist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WatchlistApi->create_watchlist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **watchlist** | [**Watchlist**](Watchlist.md)|  | 

### Return type

[**Watchlist**](Watchlist.md)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**2XX** | Watchlist data returned |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_watchlist**
> delete_watchlist(tmdb_id, media_type)

Delete watchlist item

Removes a watchlist item.

### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
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
    api_instance = seerr.WatchlistApi(api_client)
    tmdb_id = '1' # str | tmdbId ID
    media_type = 'media_type_example' # str | 

    try:
        # Delete watchlist item
        api_instance.delete_watchlist(tmdb_id, media_type)
    except Exception as e:
        print("Exception when calling WatchlistApi->delete_watchlist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tmdb_id** | **str**| tmdbId ID | 
 **media_type** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Succesfully removed watchlist item |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


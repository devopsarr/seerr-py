# seerr.BlocklistApi

All URIs are relative to *http://localhost:5055/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_blacklist**](BlocklistApi.md#create_blacklist) | **POST** /blacklist | Add media to blocklist
[**create_blocklist**](BlocklistApi.md#create_blocklist) | **POST** /blocklist | Add media to blocklist
[**create_blocklist_collection_by_collection_id**](BlocklistApi.md#create_blocklist_collection_by_collection_id) | **POST** /blocklist/collection/{collectionId} | Add collection to blocklist
[**delete_blacklist**](BlocklistApi.md#delete_blacklist) | **DELETE** /blacklist/{tmdbId} | Remove media from blocklist
[**delete_blocklist**](BlocklistApi.md#delete_blocklist) | **DELETE** /blocklist/{tmdbId} | Remove media from blocklist
[**delete_blocklist_collection**](BlocklistApi.md#delete_blocklist_collection) | **DELETE** /blocklist/collection/{collectionId} | Remove collection from blocklist
[**get_blacklist**](BlocklistApi.md#get_blacklist) | **GET** /blacklist | Returns blocklisted items
[**get_blacklist_by_tmdb_id**](BlocklistApi.md#get_blacklist_by_tmdb_id) | **GET** /blacklist/{tmdbId} | Get media from blocklist
[**get_blocklist**](BlocklistApi.md#get_blocklist) | **GET** /blocklist | Returns blocklisted items
[**get_blocklist_by_tmdb_id**](BlocklistApi.md#get_blocklist_by_tmdb_id) | **GET** /blocklist/{tmdbId} | Get media from blocklist


# **create_blacklist**
> create_blacklist(blocklist)

Add media to blocklist

**DEPRECATED**: Use `/blocklist` instead. This endpoint will be deprecated soon.


### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
from seerr.models.blocklist import Blocklist
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
    api_instance = seerr.BlocklistApi(api_client)
    blocklist = seerr.Blocklist() # Blocklist | 

    try:
        # Add media to blocklist
        api_instance.create_blacklist(blocklist)
    except Exception as e:
        print("Exception when calling BlocklistApi->create_blacklist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **blocklist** | [**Blocklist**](Blocklist.md)|  | 

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Item succesfully blocklisted |  -  |
**412** | Item has already been blocklisted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_blocklist**
> create_blocklist(blocklist)

Add media to blocklist

### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
from seerr.models.blocklist import Blocklist
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
    api_instance = seerr.BlocklistApi(api_client)
    blocklist = seerr.Blocklist() # Blocklist | 

    try:
        # Add media to blocklist
        api_instance.create_blocklist(blocklist)
    except Exception as e:
        print("Exception when calling BlocklistApi->create_blocklist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **blocklist** | [**Blocklist**](Blocklist.md)|  | 

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Item succesfully blocklisted |  -  |
**412** | Item has already been blocklisted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_blocklist_collection_by_collection_id**
> create_blocklist_collection_by_collection_id(collection_id, body=body)

Add collection to blocklist

Adds all movies in a collection to the blocklist

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
    api_instance = seerr.BlocklistApi(api_client)
    collection_id = '1424991' # str | Collection ID
    body = None # object |  (optional)

    try:
        # Add collection to blocklist
        api_instance.create_blocklist_collection_by_collection_id(collection_id, body=body)
    except Exception as e:
        print("Exception when calling BlocklistApi->create_blocklist_collection_by_collection_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **collection_id** | **str**| Collection ID | 
 **body** | **object**|  | [optional] 

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successfully added collection to blocklist |  -  |
**500** | Error adding collection to blocklist |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_blacklist**
> delete_blacklist(tmdb_id, media_type)

Remove media from blocklist

**DEPRECATED**: Use `/blocklist/{tmdbId}` instead. This endpoint will be deprecated soon.


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
    api_instance = seerr.BlocklistApi(api_client)
    tmdb_id = '1' # str | tmdbId ID
    media_type = 'media_type_example' # str | 

    try:
        # Remove media from blocklist
        api_instance.delete_blacklist(tmdb_id, media_type)
    except Exception as e:
        print("Exception when calling BlocklistApi->delete_blacklist: %s\n" % e)
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
**204** | Succesfully removed media item |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_blocklist**
> delete_blocklist(tmdb_id, media_type)

Remove media from blocklist

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
    api_instance = seerr.BlocklistApi(api_client)
    tmdb_id = '1' # str | tmdbId ID
    media_type = 'media_type_example' # str | 

    try:
        # Remove media from blocklist
        api_instance.delete_blocklist(tmdb_id, media_type)
    except Exception as e:
        print("Exception when calling BlocklistApi->delete_blocklist: %s\n" % e)
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
**204** | Succesfully removed media item |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_blocklist_collection**
> delete_blocklist_collection(collection_id)

Remove collection from blocklist

Removes all movies in a collection from the blocklist

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
    api_instance = seerr.BlocklistApi(api_client)
    collection_id = '1424991' # str | Collection ID

    try:
        # Remove collection from blocklist
        api_instance.delete_blocklist_collection(collection_id)
    except Exception as e:
        print("Exception when calling BlocklistApi->delete_blocklist_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **collection_id** | **str**| Collection ID | 

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
**204** | Successfully removed collection from blocklist |  -  |
**500** | Error removing collection from blocklist |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_blacklist**
> GetBlocklist2XXResponse get_blacklist(take=take, skip=skip, search=search, filter=filter)

Returns blocklisted items

**DEPRECATED**: Use `/blocklist` instead. This endpoint will be deprecated soon.


### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
from seerr.models.get_blocklist2_xx_response import GetBlocklist2XXResponse
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
    api_instance = seerr.BlocklistApi(api_client)
    take = 25 # float |  (optional)
    skip = 0 # float |  (optional)
    search = 'dune' # str |  (optional)
    filter = manual # str |  (optional) (default to manual)

    try:
        # Returns blocklisted items
        api_response = api_instance.get_blacklist(take=take, skip=skip, search=search, filter=filter)
        print("The response of BlocklistApi->get_blacklist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BlocklistApi->get_blacklist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **take** | **float**|  | [optional] 
 **skip** | **float**|  | [optional] 
 **search** | **str**|  | [optional] 
 **filter** | **str**|  | [optional] [default to manual]

### Return type

[**GetBlocklist2XXResponse**](GetBlocklist2XXResponse.md)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**2XX** | Blocklisted items returned |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_blacklist_by_tmdb_id**
> get_blacklist_by_tmdb_id(tmdb_id, media_type)

Get media from blocklist

**DEPRECATED**: Use `/blocklist/{tmdbId}` instead. This endpoint will be deprecated soon.


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
    api_instance = seerr.BlocklistApi(api_client)
    tmdb_id = '1' # str | tmdbId ID
    media_type = 'media_type_example' # str | 

    try:
        # Get media from blocklist
        api_instance.get_blacklist_by_tmdb_id(tmdb_id, media_type)
    except Exception as e:
        print("Exception when calling BlocklistApi->get_blacklist_by_tmdb_id: %s\n" % e)
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
**2XX** | Blocklist details in JSON |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_blocklist**
> GetBlocklist2XXResponse get_blocklist(take=take, skip=skip, search=search, filter=filter)

Returns blocklisted items

Returns list of all blocklisted media

### Example

* Api Key Authentication (apiKey):
* Api Key Authentication (cookieAuth):

```python
import seerr
from seerr.models.get_blocklist2_xx_response import GetBlocklist2XXResponse
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
    api_instance = seerr.BlocklistApi(api_client)
    take = 25 # float |  (optional)
    skip = 0 # float |  (optional)
    search = 'dune' # str |  (optional)
    filter = manual # str |  (optional) (default to manual)

    try:
        # Returns blocklisted items
        api_response = api_instance.get_blocklist(take=take, skip=skip, search=search, filter=filter)
        print("The response of BlocklistApi->get_blocklist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BlocklistApi->get_blocklist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **take** | **float**|  | [optional] 
 **skip** | **float**|  | [optional] 
 **search** | **str**|  | [optional] 
 **filter** | **str**|  | [optional] [default to manual]

### Return type

[**GetBlocklist2XXResponse**](GetBlocklist2XXResponse.md)

### Authorization

[apiKey](../README.md#apiKey), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**2XX** | Blocklisted items returned |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_blocklist_by_tmdb_id**
> get_blocklist_by_tmdb_id(tmdb_id, media_type)

Get media from blocklist

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
    api_instance = seerr.BlocklistApi(api_client)
    tmdb_id = '1' # str | tmdbId ID
    media_type = 'media_type_example' # str | 

    try:
        # Get media from blocklist
        api_instance.get_blocklist_by_tmdb_id(tmdb_id, media_type)
    except Exception as e:
        print("Exception when calling BlocklistApi->get_blocklist_by_tmdb_id: %s\n" % e)
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
**2XX** | Blocklist details in JSON |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


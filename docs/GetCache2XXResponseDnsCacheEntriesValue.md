# GetCache2XXResponseDnsCacheEntriesValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**addresses** | [**GetCache2XXResponseDnsCacheEntriesValueAddresses**](GetCache2XXResponseDnsCacheEntriesValueAddresses.md) |  | [optional] 
**active_address** | **str** |  | [optional] 
**family** | **float** |  | [optional] 
**age** | **float** |  | [optional] 
**ttl** | **float** |  | [optional] 
**network_errors** | **float** |  | [optional] 
**hits** | **float** |  | [optional] 
**misses** | **float** |  | [optional] 

## Example

```python
from seerr.models.get_cache2_xx_response_dns_cache_entries_value import GetCache2XXResponseDnsCacheEntriesValue

# TODO update the JSON string below
json = "{}"
# create an instance of GetCache2XXResponseDnsCacheEntriesValue from a JSON string
get_cache2_xx_response_dns_cache_entries_value_instance = GetCache2XXResponseDnsCacheEntriesValue.from_json(json)
# print the JSON string representation of the object
print(GetCache2XXResponseDnsCacheEntriesValue.to_json())

# convert the object into a dict
get_cache2_xx_response_dns_cache_entries_value_dict = get_cache2_xx_response_dns_cache_entries_value_instance.to_dict()
# create an instance of GetCache2XXResponseDnsCacheEntriesValue from a dict
get_cache2_xx_response_dns_cache_entries_value_from_dict = GetCache2XXResponseDnsCacheEntriesValue.from_dict(get_cache2_xx_response_dns_cache_entries_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



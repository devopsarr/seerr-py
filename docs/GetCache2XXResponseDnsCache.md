# GetCache2XXResponseDnsCache


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**stats** | [**GetCache2XXResponseDnsCacheStats**](GetCache2XXResponseDnsCacheStats.md) |  | [optional] 
**entries** | [**Dict[str, GetCache2XXResponseDnsCacheEntriesValue]**](GetCache2XXResponseDnsCacheEntriesValue.md) |  | [optional] 

## Example

```python
from seerr.models.get_cache2_xx_response_dns_cache import GetCache2XXResponseDnsCache

# TODO update the JSON string below
json = "{}"
# create an instance of GetCache2XXResponseDnsCache from a JSON string
get_cache2_xx_response_dns_cache_instance = GetCache2XXResponseDnsCache.from_json(json)
# print the JSON string representation of the object
print(GetCache2XXResponseDnsCache.to_json())

# convert the object into a dict
get_cache2_xx_response_dns_cache_dict = get_cache2_xx_response_dns_cache_instance.to_dict()
# create an instance of GetCache2XXResponseDnsCache from a dict
get_cache2_xx_response_dns_cache_from_dict = GetCache2XXResponseDnsCache.from_dict(get_cache2_xx_response_dns_cache_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



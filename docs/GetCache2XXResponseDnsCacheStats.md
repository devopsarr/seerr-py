# GetCache2XXResponseDnsCacheStats


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**size** | **float** |  | [optional] 
**max_size** | **float** |  | [optional] 
**hits** | **float** |  | [optional] 
**misses** | **float** |  | [optional] 
**failures** | **float** |  | [optional] 
**ipv4_fallbacks** | **float** |  | [optional] 
**hit_rate** | **float** |  | [optional] 

## Example

```python
from seerr.models.get_cache2_xx_response_dns_cache_stats import GetCache2XXResponseDnsCacheStats

# TODO update the JSON string below
json = "{}"
# create an instance of GetCache2XXResponseDnsCacheStats from a JSON string
get_cache2_xx_response_dns_cache_stats_instance = GetCache2XXResponseDnsCacheStats.from_json(json)
# print the JSON string representation of the object
print(GetCache2XXResponseDnsCacheStats.to_json())

# convert the object into a dict
get_cache2_xx_response_dns_cache_stats_dict = get_cache2_xx_response_dns_cache_stats_instance.to_dict()
# create an instance of GetCache2XXResponseDnsCacheStats from a dict
get_cache2_xx_response_dns_cache_stats_from_dict = GetCache2XXResponseDnsCacheStats.from_dict(get_cache2_xx_response_dns_cache_stats_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



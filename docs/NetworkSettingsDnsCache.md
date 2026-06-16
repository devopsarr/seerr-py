# NetworkSettingsDnsCache


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**force_min_ttl** | **float** |  | [optional] 
**force_max_ttl** | **float** |  | [optional] 

## Example

```python
from seerr.models.network_settings_dns_cache import NetworkSettingsDnsCache

# TODO update the JSON string below
json = "{}"
# create an instance of NetworkSettingsDnsCache from a JSON string
network_settings_dns_cache_instance = NetworkSettingsDnsCache.from_json(json)
# print the JSON string representation of the object
print(NetworkSettingsDnsCache.to_json())

# convert the object into a dict
network_settings_dns_cache_dict = network_settings_dns_cache_instance.to_dict()
# create an instance of NetworkSettingsDnsCache from a dict
network_settings_dns_cache_from_dict = NetworkSettingsDnsCache.from_dict(network_settings_dns_cache_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



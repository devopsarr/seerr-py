# NetworkSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**csrf_protection** | **bool** |  | [optional] 
**force_ipv4_first** | **bool** |  | [optional] 
**trust_proxy** | **bool** |  | [optional] 
**proxy** | [**NetworkSettingsProxy**](NetworkSettingsProxy.md) |  | [optional] 
**dns_cache** | [**NetworkSettingsDnsCache**](NetworkSettingsDnsCache.md) |  | [optional] 

## Example

```python
from seerr.models.network_settings import NetworkSettings

# TODO update the JSON string below
json = "{}"
# create an instance of NetworkSettings from a JSON string
network_settings_instance = NetworkSettings.from_json(json)
# print the JSON string representation of the object
print(NetworkSettings.to_json())

# convert the object into a dict
network_settings_dict = network_settings_instance.to_dict()
# create an instance of NetworkSettings from a dict
network_settings_from_dict = NetworkSettings.from_dict(network_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



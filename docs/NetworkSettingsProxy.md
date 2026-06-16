# NetworkSettingsProxy


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**hostname** | **str** |  | [optional] 
**port** | **float** |  | [optional] 
**use_ssl** | **bool** |  | [optional] 
**user** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**bypass_filter** | **str** |  | [optional] 
**bypass_local_addresses** | **bool** |  | [optional] 

## Example

```python
from seerr.models.network_settings_proxy import NetworkSettingsProxy

# TODO update the JSON string below
json = "{}"
# create an instance of NetworkSettingsProxy from a JSON string
network_settings_proxy_instance = NetworkSettingsProxy.from_json(json)
# print the JSON string representation of the object
print(NetworkSettingsProxy.to_json())

# convert the object into a dict
network_settings_proxy_dict = network_settings_proxy_instance.to_dict()
# create an instance of NetworkSettingsProxy from a dict
network_settings_proxy_from_dict = NetworkSettingsProxy.from_dict(network_settings_proxy_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



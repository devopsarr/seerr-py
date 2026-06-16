# JellyfinSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] [readonly] 
**hostname** | **str** |  | [optional] 
**external_hostname** | **str** |  | [optional] 
**jellyfin_forgot_password_url** | **str** |  | [optional] 
**admin_user** | **str** |  | [optional] 
**admin_pass** | **str** |  | [optional] 
**libraries** | [**List[JellyfinLibrary]**](JellyfinLibrary.md) |  | [optional] [readonly] 
**server_id** | **str** |  | [optional] [readonly] 

## Example

```python
from seerr.models.jellyfin_settings import JellyfinSettings

# TODO update the JSON string below
json = "{}"
# create an instance of JellyfinSettings from a JSON string
jellyfin_settings_instance = JellyfinSettings.from_json(json)
# print the JSON string representation of the object
print(JellyfinSettings.to_json())

# convert the object into a dict
jellyfin_settings_dict = jellyfin_settings_instance.to_dict()
# create an instance of JellyfinSettings from a dict
jellyfin_settings_from_dict = JellyfinSettings.from_dict(jellyfin_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



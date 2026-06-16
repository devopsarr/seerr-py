# NtfySettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**types** | **float** |  | [optional] 
**options** | [**NtfySettingsOptions**](NtfySettingsOptions.md) |  | [optional] 

## Example

```python
from seerr.models.ntfy_settings import NtfySettings

# TODO update the JSON string below
json = "{}"
# create an instance of NtfySettings from a JSON string
ntfy_settings_instance = NtfySettings.from_json(json)
# print the JSON string representation of the object
print(NtfySettings.to_json())

# convert the object into a dict
ntfy_settings_dict = ntfy_settings_instance.to_dict()
# create an instance of NtfySettings from a dict
ntfy_settings_from_dict = NtfySettings.from_dict(ntfy_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# NtfySettingsOptions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | [optional] 
**topic** | **str** |  | [optional] 
**auth_method_username_password** | **bool** |  | [optional] 
**username** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**auth_method_token** | **bool** |  | [optional] 
**token** | **str** |  | [optional] 
**priority** | **float** |  | [optional] 
**locale** | **str** |  | [optional] 

## Example

```python
from seerr.models.ntfy_settings_options import NtfySettingsOptions

# TODO update the JSON string below
json = "{}"
# create an instance of NtfySettingsOptions from a JSON string
ntfy_settings_options_instance = NtfySettingsOptions.from_json(json)
# print the JSON string representation of the object
print(NtfySettingsOptions.to_json())

# convert the object into a dict
ntfy_settings_options_dict = ntfy_settings_options_instance.to_dict()
# create an instance of NtfySettingsOptions from a dict
ntfy_settings_options_from_dict = NtfySettingsOptions.from_dict(ntfy_settings_options_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



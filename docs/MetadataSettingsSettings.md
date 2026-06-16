# MetadataSettingsSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tv** | **str** |  | [optional] 
**anime** | **str** |  | [optional] 

## Example

```python
from seerr.models.metadata_settings_settings import MetadataSettingsSettings

# TODO update the JSON string below
json = "{}"
# create an instance of MetadataSettingsSettings from a JSON string
metadata_settings_settings_instance = MetadataSettingsSettings.from_json(json)
# print the JSON string representation of the object
print(MetadataSettingsSettings.to_json())

# convert the object into a dict
metadata_settings_settings_dict = metadata_settings_settings_instance.to_dict()
# create an instance of MetadataSettingsSettings from a dict
metadata_settings_settings_from_dict = MetadataSettingsSettings.from_dict(metadata_settings_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



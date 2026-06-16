# MetadataSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**settings** | [**MetadataSettingsSettings**](MetadataSettingsSettings.md) |  | [optional] 

## Example

```python
from seerr.models.metadata_settings import MetadataSettings

# TODO update the JSON string below
json = "{}"
# create an instance of MetadataSettings from a JSON string
metadata_settings_instance = MetadataSettings.from_json(json)
# print the JSON string representation of the object
print(MetadataSettings.to_json())

# convert the object into a dict
metadata_settings_dict = metadata_settings_instance.to_dict()
# create an instance of MetadataSettings from a dict
metadata_settings_from_dict = MetadataSettings.from_dict(metadata_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



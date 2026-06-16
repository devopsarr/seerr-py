# JellyfinLibrary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**enabled** | **bool** |  | 

## Example

```python
from seerr.models.jellyfin_library import JellyfinLibrary

# TODO update the JSON string below
json = "{}"
# create an instance of JellyfinLibrary from a JSON string
jellyfin_library_instance = JellyfinLibrary.from_json(json)
# print the JSON string representation of the object
print(JellyfinLibrary.to_json())

# convert the object into a dict
jellyfin_library_dict = jellyfin_library_instance.to_dict()
# create an instance of JellyfinLibrary from a dict
jellyfin_library_from_dict = JellyfinLibrary.from_dict(jellyfin_library_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



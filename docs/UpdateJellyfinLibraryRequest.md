# UpdateJellyfinLibraryRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | 

## Example

```python
from seerr.models.update_jellyfin_library_request import UpdateJellyfinLibraryRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateJellyfinLibraryRequest from a JSON string
update_jellyfin_library_request_instance = UpdateJellyfinLibraryRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateJellyfinLibraryRequest.to_json())

# convert the object into a dict
update_jellyfin_library_request_dict = update_jellyfin_library_request_instance.to_dict()
# create an instance of UpdateJellyfinLibraryRequest from a dict
update_jellyfin_library_request_from_dict = UpdateJellyfinLibraryRequest.from_dict(update_jellyfin_library_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



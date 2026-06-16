# CreateUserImportFromJellyfinRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**jellyfin_user_ids** | **List[str]** |  | [optional] 

## Example

```python
from seerr.models.create_user_import_from_jellyfin_request import CreateUserImportFromJellyfinRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateUserImportFromJellyfinRequest from a JSON string
create_user_import_from_jellyfin_request_instance = CreateUserImportFromJellyfinRequest.from_json(json)
# print the JSON string representation of the object
print(CreateUserImportFromJellyfinRequest.to_json())

# convert the object into a dict
create_user_import_from_jellyfin_request_dict = create_user_import_from_jellyfin_request_instance.to_dict()
# create an instance of CreateUserImportFromJellyfinRequest from a dict
create_user_import_from_jellyfin_request_from_dict = CreateUserImportFromJellyfinRequest.from_dict(create_user_import_from_jellyfin_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



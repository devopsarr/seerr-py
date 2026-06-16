# CreateJellyfinSyncRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cancel** | **bool** |  | [optional] 
**start** | **bool** |  | [optional] 

## Example

```python
from seerr.models.create_jellyfin_sync_request import CreateJellyfinSyncRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateJellyfinSyncRequest from a JSON string
create_jellyfin_sync_request_instance = CreateJellyfinSyncRequest.from_json(json)
# print the JSON string representation of the object
print(CreateJellyfinSyncRequest.to_json())

# convert the object into a dict
create_jellyfin_sync_request_dict = create_jellyfin_sync_request_instance.to_dict()
# create an instance of CreateJellyfinSyncRequest from a dict
create_jellyfin_sync_request_from_dict = CreateJellyfinSyncRequest.from_dict(create_jellyfin_sync_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



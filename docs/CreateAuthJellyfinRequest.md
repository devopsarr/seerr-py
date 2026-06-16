# CreateAuthJellyfinRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | 
**password** | **str** |  | 
**hostname** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**server_type** | **float** |  | [optional] 

## Example

```python
from seerr.models.create_auth_jellyfin_request import CreateAuthJellyfinRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAuthJellyfinRequest from a JSON string
create_auth_jellyfin_request_instance = CreateAuthJellyfinRequest.from_json(json)
# print the JSON string representation of the object
print(CreateAuthJellyfinRequest.to_json())

# convert the object into a dict
create_auth_jellyfin_request_dict = create_auth_jellyfin_request_instance.to_dict()
# create an instance of CreateAuthJellyfinRequest from a dict
create_auth_jellyfin_request_from_dict = CreateAuthJellyfinRequest.from_dict(create_auth_jellyfin_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



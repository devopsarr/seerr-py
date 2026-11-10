# CreateOverrideruleAdvancedRequestRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**media_type** | **str** |  | 
**tmdb_id** | **float** |  | 
**is4k** | **bool** |  | [optional] 
**request_id** | **float** |  | [optional] 
**request_user** | **float** |  | [optional] 
**tags** | **List[float]** |  | [optional] 
**service_id** | **float** |  | [optional] 

## Example

```python
from seerr.models.create_overriderule_advanced_request_request import CreateOverrideruleAdvancedRequestRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOverrideruleAdvancedRequestRequest from a JSON string
create_overriderule_advanced_request_request_instance = CreateOverrideruleAdvancedRequestRequest.from_json(json)
# print the JSON string representation of the object
print(CreateOverrideruleAdvancedRequestRequest.to_json())

# convert the object into a dict
create_overriderule_advanced_request_request_dict = create_overriderule_advanced_request_request_instance.to_dict()
# create an instance of CreateOverrideruleAdvancedRequestRequest from a dict
create_overriderule_advanced_request_request_from_dict = CreateOverrideruleAdvancedRequestRequest.from_dict(create_overriderule_advanced_request_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



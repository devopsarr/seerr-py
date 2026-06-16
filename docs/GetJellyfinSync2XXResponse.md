# GetJellyfinSync2XXResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**running** | **bool** |  | [optional] 
**progress** | **float** |  | [optional] 
**total** | **float** |  | [optional] 
**current_library** | [**JellyfinLibrary**](JellyfinLibrary.md) |  | [optional] 
**libraries** | [**List[JellyfinLibrary]**](JellyfinLibrary.md) |  | [optional] 

## Example

```python
from seerr.models.get_jellyfin_sync2_xx_response import GetJellyfinSync2XXResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GetJellyfinSync2XXResponse from a JSON string
get_jellyfin_sync2_xx_response_instance = GetJellyfinSync2XXResponse.from_json(json)
# print the JSON string representation of the object
print(GetJellyfinSync2XXResponse.to_json())

# convert the object into a dict
get_jellyfin_sync2_xx_response_dict = get_jellyfin_sync2_xx_response_instance.to_dict()
# create an instance of GetJellyfinSync2XXResponse from a dict
get_jellyfin_sync2_xx_response_from_dict = GetJellyfinSync2XXResponse.from_dict(get_jellyfin_sync2_xx_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



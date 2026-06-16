# UserSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**locale** | **str** |  | [optional] 
**discover_region** | **str** |  | [optional] 
**streaming_region** | **str** |  | [optional] 
**original_language** | **str** |  | [optional] 
**movie_quota_limit** | **float** | Maximum number of movie requests allowed | [optional] 
**movie_quota_days** | **float** | Time period in days for movie quota | [optional] 
**tv_quota_limit** | **float** | Maximum number of TV requests allowed | [optional] 
**tv_quota_days** | **float** | Time period in days for TV quota | [optional] 
**global_movie_quota_days** | **float** | Global movie quota days setting | [optional] 
**global_movie_quota_limit** | **float** | Global movie quota limit setting | [optional] 
**global_tv_quota_limit** | **float** | Global TV quota limit setting | [optional] 
**global_tv_quota_days** | **float** | Global TV quota days setting | [optional] 
**watchlist_sync_movies** | **bool** | Enable watchlist sync for movies | [optional] 
**watchlist_sync_tv** | **bool** | Enable watchlist sync for TV | [optional] 

## Example

```python
from seerr.models.user_settings import UserSettings

# TODO update the JSON string below
json = "{}"
# create an instance of UserSettings from a JSON string
user_settings_instance = UserSettings.from_json(json)
# print the JSON string representation of the object
print(UserSettings.to_json())

# convert the object into a dict
user_settings_dict = user_settings_instance.to_dict()
# create an instance of UserSettings from a dict
user_settings_from_dict = UserSettings.from_dict(user_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



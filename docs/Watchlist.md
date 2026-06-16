# Watchlist


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**tmdb_id** | **float** |  | [optional] 
**rating_key** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**media** | [**MediaInfo**](MediaInfo.md) |  | [optional] 
**created_at** | **str** |  | [optional] [readonly] 
**updated_at** | **str** |  | [optional] [readonly] 
**requested_by** | [**User**](User.md) |  | [optional] 

## Example

```python
from seerr.models.watchlist import Watchlist

# TODO update the JSON string below
json = "{}"
# create an instance of Watchlist from a JSON string
watchlist_instance = Watchlist.from_json(json)
# print the JSON string representation of the object
print(Watchlist.to_json())

# convert the object into a dict
watchlist_dict = watchlist_instance.to_dict()
# create an instance of Watchlist from a dict
watchlist_from_dict = Watchlist.from_dict(watchlist_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



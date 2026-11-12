# WatchlistRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tmdb_id** | **float** |  | 
**media_type** | **str** |  | 
**rating_key** | **str** |  | [optional] 
**title** | **str** |  | [optional] 

## Example

```python
from seerr.models.watchlist_request import WatchlistRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WatchlistRequest from a JSON string
watchlist_request_instance = WatchlistRequest.from_json(json)
# print the JSON string representation of the object
print(WatchlistRequest.to_json())

# convert the object into a dict
watchlist_request_dict = watchlist_request_instance.to_dict()
# create an instance of WatchlistRequest from a dict
watchlist_request_from_dict = WatchlistRequest.from_dict(watchlist_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



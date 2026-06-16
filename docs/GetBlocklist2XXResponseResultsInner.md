# GetBlocklist2XXResponseResultsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | [**User**](User.md) |  | [optional] 
**created_at** | **str** |  | [optional] 
**id** | **float** |  | [optional] 
**media_type** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**tmdb_id** | **float** |  | [optional] 

## Example

```python
from seerr.models.get_blocklist2_xx_response_results_inner import GetBlocklist2XXResponseResultsInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetBlocklist2XXResponseResultsInner from a JSON string
get_blocklist2_xx_response_results_inner_instance = GetBlocklist2XXResponseResultsInner.from_json(json)
# print the JSON string representation of the object
print(GetBlocklist2XXResponseResultsInner.to_json())

# convert the object into a dict
get_blocklist2_xx_response_results_inner_dict = get_blocklist2_xx_response_results_inner_instance.to_dict()
# create an instance of GetBlocklist2XXResponseResultsInner from a dict
get_blocklist2_xx_response_results_inner_from_dict = GetBlocklist2XXResponseResultsInner.from_dict(get_blocklist2_xx_response_results_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



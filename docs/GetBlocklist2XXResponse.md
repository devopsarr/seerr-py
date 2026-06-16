# GetBlocklist2XXResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_info** | [**PageInfo**](PageInfo.md) |  | [optional] 
**results** | [**List[GetBlocklist2XXResponseResultsInner]**](GetBlocklist2XXResponseResultsInner.md) |  | [optional] 

## Example

```python
from seerr.models.get_blocklist2_xx_response import GetBlocklist2XXResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GetBlocklist2XXResponse from a JSON string
get_blocklist2_xx_response_instance = GetBlocklist2XXResponse.from_json(json)
# print the JSON string representation of the object
print(GetBlocklist2XXResponse.to_json())

# convert the object into a dict
get_blocklist2_xx_response_dict = get_blocklist2_xx_response_instance.to_dict()
# create an instance of GetBlocklist2XXResponse from a dict
get_blocklist2_xx_response_from_dict = GetBlocklist2XXResponse.from_dict(get_blocklist2_xx_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



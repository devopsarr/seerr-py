# CertificationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**certifications** | **Dict[str, List[Certification]]** |  | [optional] 

## Example

```python
from seerr.models.certification_response import CertificationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CertificationResponse from a JSON string
certification_response_instance = CertificationResponse.from_json(json)
# print the JSON string representation of the object
print(CertificationResponse.to_json())

# convert the object into a dict
certification_response_dict = certification_response_instance.to_dict()
# create an instance of CertificationResponse from a dict
certification_response_from_dict = CertificationResponse.from_dict(certification_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



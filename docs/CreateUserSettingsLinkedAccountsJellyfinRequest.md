# CreateUserSettingsLinkedAccountsJellyfinRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | [optional] 
**password** | **str** |  | [optional] 

## Example

```python
from seerr.models.create_user_settings_linked_accounts_jellyfin_request import CreateUserSettingsLinkedAccountsJellyfinRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateUserSettingsLinkedAccountsJellyfinRequest from a JSON string
create_user_settings_linked_accounts_jellyfin_request_instance = CreateUserSettingsLinkedAccountsJellyfinRequest.from_json(json)
# print the JSON string representation of the object
print(CreateUserSettingsLinkedAccountsJellyfinRequest.to_json())

# convert the object into a dict
create_user_settings_linked_accounts_jellyfin_request_dict = create_user_settings_linked_accounts_jellyfin_request_instance.to_dict()
# create an instance of CreateUserSettingsLinkedAccountsJellyfinRequest from a dict
create_user_settings_linked_accounts_jellyfin_request_from_dict = CreateUserSettingsLinkedAccountsJellyfinRequest.from_dict(create_user_settings_linked_accounts_jellyfin_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



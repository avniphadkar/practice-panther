# Matter

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] 
**account_ref** | [**\Swagger\Client\Model\AccountReference**](AccountReference.md) |  | [optional] 
**number** | **int** | This is the matter number. If Auto-Numbering is turned on you can leave this field blank and PracticePanther will automatically assign the next available number | [optional] 
**display_name** | **string** | This is the display name for the matter. It is set automatically based on the user settings in the UI This is the display name for the matter. It is set automatically based on the user settings in the UI | [optional] 
**name** | **string** | This is the name of the matter, for example John vs. Jane | 
**notes** | **string** | Matter notes, can be either plain text or HTML | [optional] 
**open_date** | [**\DateTime**](\DateTime.md) |  | [optional] 
**close_date** | [**\DateTime**](\DateTime.md) |  | [optional] 
**statute_of_limitation_date** | [**\DateTime**](\DateTime.md) |  | [optional] 
**tags** | **string[]** |  | [optional] 
**status** | **string** | Determines if this matter is open, closed or pending. | 
**assigned_to_users** | [**\Swagger\Client\Model\UserReference[]**](UserReference.md) | At least one user must be assigned to this matter. You can get the current user using get at /users/me | [optional] 
**custom_field_values** | [**\Swagger\Client\Model\CustomFieldValue[]**](CustomFieldValue.md) | This is a list of custom field values related to this matter | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | updated_at can be used to sync matters with PracticePanther. updated_at can be used to sync matters with PracticePanther. | [optional] 
**updated_at** | [**\DateTime**](\DateTime.md) | updated_at can be used to sync matters with PracticePanther. updated_at can be used to sync matters with PracticePanther. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



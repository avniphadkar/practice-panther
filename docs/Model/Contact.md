# Contact

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] 
**account_ref** | [**\Swagger\Client\Model\AccountReference**](AccountReference.md) |  | [optional] 
**is_primary_contact** | **bool** | This will be set to true if this contact is a primary contact for the account This will be set to true if this contact is a primary contact for the account | [optional] 
**display_name** | **string** | This is the display name for the contact. It is read-only and set automatically based on the user settings in the UI This is the display name for the contact. It is read-only and set automatically based on the user settings in the UI | [optional] 
**first_name** | **string** |  | [optional] 
**last_name** | **string** |  | [optional] 
**phone_mobile** | **string** | This will be used to send text message reminders and notifications to this contact | [optional] 
**phone_home** | **string** |  | [optional] 
**phone_fax** | **string** |  | [optional] 
**phone_work** | **string** |  | [optional] 
**email** | **string** | Must be a valid email address | [optional] 
**notes** | **string** | Can be either plain text or HTML. | [optional] 
**custom_field_values** | [**\Swagger\Client\Model\CustomFieldValue[]**](CustomFieldValue.md) | This is a list of custom field values related to this contact | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Account

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] 
**display_name** | **string** | This is the display name for the contact. It is set automatically based on the user settings in the UI This is the display name for the contact. It is set automatically based on the user settings in the UI | [optional] 
**number** | **int** | This is the account number. If Auto-Numbering is turned on you can leave this field blank and PracticePanther will automatically assign the next available number | [optional] 
**company_name** | **string** | Should be set only if this account represents a company | [optional] 
**address_street_1** | **string** |  | [optional] 
**address_street_2** | **string** |  | [optional] 
**address_city** | **string** |  | [optional] 
**address_state** | **string** |  | [optional] 
**address_country** | **string** |  | [optional] 
**address_zip_code** | **string** |  | [optional] 
**tags** | **string[]** |  | [optional] 
**company_custom_field_values** | [**\Swagger\Client\Model\CustomFieldValue[]**](CustomFieldValue.md) | This is a list of custom field values related to this company. Can only be used if company_name is set for this account | [optional] 
**assigned_to_users** | [**\Swagger\Client\Model\UserReference[]**](UserReference.md) | At least one user must be assigned to this matter. You can get the current user using get at /users/me | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | updated_at can be used to sync contacts with PracticePanther. updated_at can be used to sync contacts with PracticePanther. | [optional] 
**updated_at** | [**\DateTime**](\DateTime.md) | updated_at can be used to sync contacts with PracticePanther. updated_at can be used to sync contacts with PracticePanther. | [optional] 
**notes** | **string** | These are company notes and can only be used if company_name is set for this account | [optional] 
**primary_contact** | [**\Swagger\Client\Model\Contact**](Contact.md) | This is the primary contact for this account | [optional] 
**other_contacts** | [**\Swagger\Client\Model\Contact[]**](Contact.md) | If this account is a company, this will include any additional contacts other than the primary contact, if any | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



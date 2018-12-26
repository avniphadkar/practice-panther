# CustomFieldValue

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**custom_field_ref** | [**\Swagger\Client\Model\CustomFieldRef**](CustomFieldRef.md) | This is a reference to the custom field we are setting this value for. | 
**value_boolean** | **bool** | Used only if CustomField.Type &#x3D;&#x3D; Checkbox | [optional] 
**contact_ref** | [**\Swagger\Client\Model\ContactReference**](ContactReference.md) | Used only if CustomField.Type &#x3D;&#x3D; Contact | [optional] 
**value_date_time** | [**\DateTime**](\DateTime.md) | Used only if CustomField.Type &#x3D;&#x3D; Date || CustomField.Type &#x3D;&#x3D; DateTime | [optional] 
**value_number** | **double** | Used only if CustomField.Type &#x3D;&#x3D; Number || CustomField.Type &#x3D;&#x3D; Currency | [optional] 
**value_string** | **string** | Used only if CustomField.Type &#x3D;&#x3D; TextEditor || CustomField.Type &#x3D;&#x3D; DropDownList | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



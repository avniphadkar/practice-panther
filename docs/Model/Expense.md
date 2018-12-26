# Expense

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] 
**is_billable** | **bool** | If set to billable, it will be automatically queued to be added to the next invoice. If this is set to false, it will show in PracticePanther as not billable | [optional] 
**is_billed** | **bool** | If set to billed, it will not be added to future invoices and will be marked as \&quot;billed\&quot; in PracticePanther | [optional] 
**date** | [**\DateTime**](\DateTime.md) | This is the date for this expense and will be visible to the client if this expense is billable. The date field can be used to run reports on expenses in PracticePanther. | [optional] 
**amount** | **double** |  | 
**description** | **string** | This is the description which will be visible on the invoice | [optional] 
**private_notes** | **string** | These are private notes that are visible to PracticePanther users but will not be added to the invoice | [optional] 
**account_ref** | [**\Swagger\Client\Model\AccountReference**](AccountReference.md) |  | 
**matter_ref** | [**\Swagger\Client\Model\MatterReference**](MatterReference.md) |  | 
**billed_by_user_ref** | [**\Swagger\Client\Model\UserReference**](UserReference.md) | The user who billed this time entry, this field is optional. If you want to get the current user information you can use GET /users/me | [optional] 
**expense_category_ref** | [**\Swagger\Client\Model\ExpenseCategory**](ExpenseCategory.md) | This field is optional. If set will add an expense category for this expense. | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) |  | [optional] 
**updated_at** | [**\DateTime**](\DateTime.md) |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



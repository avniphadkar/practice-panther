# TimeEntry

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] 
**is_billable** | **bool** | If set to billable, it will be automatically queued to be added to the next invoice. If this is set to false, it will show in PracticePanther as not billable | [optional] 
**is_billed** | **bool** | If set to billed, it will not be added to future invoices and will be marked as \&quot;billed\&quot; in PracticePanther | [optional] 
**date** | [**\DateTime**](\DateTime.md) | This is the date for this time entry and will be visible to the client if this time entry is billable. The date field can be used to run reports on time entries in PracticePanther. | 
**hours** | **double** | The number of hours worked on this time entry. For example, an hour and a half will be added as 1.5, fifteen minutes will be added as 0.25. | 
**rate** | **double** | This is the hourly rate for this time entry. Will be used together with hours to calculate the total billable for this time entry. If you leave this field blank, PracticePanther will automatically add the default hourly rate for the user and matter | [optional] 
**description** | **string** | This is the description which will be visible to the client on the invoice | [optional] 
**private_notes** | **string** | These are private notes that are visible to PracticePanther users but will not be added to the invoice | [optional] 
**account_ref** | [**\Swagger\Client\Model\AccountReference**](AccountReference.md) |  | 
**matter_ref** | [**\Swagger\Client\Model\MatterReference**](MatterReference.md) |  | 
**billed_by_user_ref** | [**\Swagger\Client\Model\UserReference**](UserReference.md) | The user who billed this time entry, this field is required. If you want to get the current user information you can use GET /users/me | 
**item_ref** | [**\Swagger\Client\Model\ItemReference**](ItemReference.md) | This is a reference to the item related to this time entry, This is field is not required, to get all available items you can GET /items | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | This field can be used to sync time entries with PracticePanther. This field can be used to sync time entries with PracticePanther. | [optional] 
**updated_at** | [**\DateTime**](\DateTime.md) | This field can be used to sync time entries with PracticePanther. This field can be used to sync time entries with PracticePanther. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



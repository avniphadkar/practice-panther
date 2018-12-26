# Invoice

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_ref** | [**\Swagger\Client\Model\AccountReference**](AccountReference.md) |  | [optional] 
**matter_ref** | [**\Swagger\Client\Model\MatterReference**](MatterReference.md) |  | [optional] 
**id** | **string** |  | [optional] 
**issue_date** | [**\DateTime**](\DateTime.md) | This is the issue date for the invoice. ie. the date this invoice was created | [optional] 
**due_date** | [**\DateTime**](\DateTime.md) | This is the due date for the invoice. If due_date is in the past and amount_due &amp;gt; 0, then this invoice is overdue. | [optional] 
**items_time_entries** | [**\Swagger\Client\Model\InvoiceLineItem[]**](InvoiceLineItem.md) |  | [optional] 
**items_expenses** | [**\Swagger\Client\Model\InvoiceLineItem[]**](InvoiceLineItem.md) |  | [optional] 
**items_flat_fees** | [**\Swagger\Client\Model\InvoiceLineItem[]**](InvoiceLineItem.md) |  | [optional] 
**subtotal** | **double** |  | [optional] 
**tax** | **double** |  | [optional] 
**discount** | **double** |  | [optional] 
**total** | **double** |  | [optional] 
**total_paid** | **double** |  | [optional] 
**total_outstanding** | **double** |  | [optional] 
**invoice_type** | **string** | Determines if this is a sale invoice, refund or credit note. | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | This field can be used to sync invoices with PracticePanther. This field can be used to sync invoices with PracticePanther. | [optional] 
**updated_at** | [**\DateTime**](\DateTime.md) | This field can be used to sync invoices with PracticePanther. This field can be used to sync invoices with PracticePanther. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



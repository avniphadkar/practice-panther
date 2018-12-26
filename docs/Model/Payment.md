# Payment

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] 
**account_ref** | [**\Swagger\Client\Model\AccountReference**](AccountReference.md) |  | 
**matter_ref** | [**\Swagger\Client\Model\MatterReference**](MatterReference.md) | If this is a payment that can be used for this account by all matters related to this account, you can leave this field empty. If this can be used only for a specific matter, you can set the matter reference here | [optional] 
**number** | **int** | This is the payment number. Leave this blank to have PracticePanther automatically set the next available number | [optional] 
**date** | [**\DateTime**](\DateTime.md) | The date field can be used to run reports on payments in PracticePanther. | 
**total_amount** | **double** | This is the amount of this payment | 
**unapplied_amount** | **double** | This is the amount of the payment that has not yet been applied on any invoices | [optional] 
**notes** | **string** |  | [optional] 
**bank_account** | [**\Swagger\Client\Model\BankAccount**](BankAccount.md) | This field is a reference to the bank account this payment is related to. You can use bank_account.type to determing if this is a Trust or Operating payment. | 
**created_at** | [**\DateTime**](\DateTime.md) | This field can be used to sync payments with PracticePanther. This field can be used to sync payments with PracticePanther. | [optional] 
**updated_at** | [**\DateTime**](\DateTime.md) | This field can be used to sync payments with PracticePanther. This field can be used to sync payments with PracticePanther. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



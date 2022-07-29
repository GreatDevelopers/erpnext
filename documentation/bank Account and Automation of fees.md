## To create a bank account which holds all the records of collection of fees from the students

For creating new Fee collection head Create a new Account. Add account name-> Select Company name-> Currency type. Select Balance type (Debit or Credit), Select Parent account type (Income account or Expenses account). After Creating head verify it in Company Cost center, while creating new Fee slip under Accounting Section select income account in which you want to add new fees.

## How a child company will be able to create a new account without creating it in the  parent or in another child company

1. First go to the company list and select the company for which you want to create the new account.
2. Under the selected company, first go to Account Settings then click on option "Allow account creation against child company".
3. Then we have to repeat the previous steps of creating a new account under the 'Chart of Accounts' section.
4. After creating a new account we also have another option to make a new account as a default bank account  by setting the new account name as 'Default Bank Account'.

## Sending Messages to specific Students using ERPNext

- Creating New Email Group Add Subscribers to whom we want to send emails.
- We can them in a bluk by writing their emails.
- After adding subscriber Create New newsletter in which we have to add email group which is created.
- Then add Subject and Message also we have option to test this message by sending to only one specific user.
- Save the newsletter we have another option schedule sending mail automatically.  

## Automation of Fee Creation of the Students

First we nedd to customize the doctype and check the autorepat box in the doctype

- go to doctype list 
- search for doctype name
- allow autorepeat checkbox in the doctype 

 Then follow the following steps

- Go to Home > Settings > Automation > Auto Repeat > New.
- Select the Reference Document Type, like Journal Entry or Sales Invoice, etc.
- Select the Reference Document. This is the individual document that you want to repeat.
- Set the Start Date and End Date (optional). If End Date is not specified, recurring documents will be created, unless the Auto Repeat is disabled.
- Set the Frequency for creating repeatable documents (Daily, Weekly, Monthly, Quarterly, Half-yearly, Yearly).
- Save

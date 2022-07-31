## Notifications in erpnext:- 



## Setting Up An Alert 

To set up a Notification:
    1. Select the Document Type you want to watch changes on. 
    2. Define what events you want to watch under Send Alert On. Events are: 
        1. New: When a new document of the selected type is made. 
        2. Save/Submit/Cancel: When a document of the selected type is saved, submitted, or canceled. 
        3. Days Before/Days After: Trigger this alert a few days before or after the Reference Date. To set the days, set Days Before or After. This can be useful in reminding you of upcoming due dates or reminding you to follow up on certain leads of quotations. 
        4. Value Change: When a particular value in the selected type changes. 
        5. Method: Sends notification when a specific method is triggered. Eg: before_insert. 
        6. Custom: Send a notification to an Email Account selected. 
    3. Set additional Conditions if required. 
    4. Set the recipients of this alert. The recipient could either be a field of the document or a list of fixed Email Addresses. 
    5. Compose the message. 
    6. Save. 

## 1.1 Setting a Subject 

You can retrieve the data for a particular field by using doc.[field_name]. To use it in your subject/message, you have to surround it with {% raw %}{{ }}{% endraw %}. These are called Jinja tags. For example, to get the name of a document, you use {% raw %}{{ doc.name }}{% endraw %}. The following example sends an email on saving a Task with the Subject, "TASK#### has been created"

## 1.2 Setting Conditions 

Notifications allow you to set conditions according to the field data in your documents. For example, if you want to receive an Email if a Lead has been saved as "Interested" as it's status, you put doc.status == "Interested" in the conditions textbox. You can also set more complex conditions by combining them with the operator and or or.

The above example will send a Notification when a Task is saved with the status "Open" and the "Expected End Date" for the Task is the date on or before the date on which it was saved on.
1.3 Setting a Message 
You can use both Jinja Tags ({% raw %}{{ doc.[field_name] }}{% endraw %}) and HTML tags in the message textbox.
1.4 Setting a Value after the Alert is Set 
Sometimes to make sure that the Notification is not sent multiple times, you can define a custom property (via Customize Form) like "Notification Sent" and then set this property after the alert is sent by setting the Set Property After Alert field.
Then you can use that as a condition in the Condition rules to ensure emails are not sent multiple times.


## Workflow:-

1. Go to the Workflow list, click on New.
2. Enter a name for the Workflow and select the DocType on which to be applied. 
3. Enter the different states of the Workflow. Enter Doc Status for them, select which field to update from the Update Field column, enter what the value will be updated to under Update Value.
4. The Workflow States can have different colors according to the state. Eg: Green for success. Document statuses: Saved = 0, Submitted = 1, Cancelled = 2.
5.  Enter the Transition Rules.
      
 
## DOCUMENTATION FOR ROLE-WISE PERMISSIONS:-

There are two methods for giving role-wise permissions :-
1. Front-End
2. Via .csv file

## FRONT-END:- 

1. Login with Administrator, Go to User list. Click on the user to whom you want to give/restrict the permission.
2. Under the “Allow Modules”. Check the boxes of those module whose permissions you want to give to that particular user. Then click on “Save”.

## Via CSV FILE:-

1. Login with Administrator, Go to Data Import list then click on “Add Data Import”.
2. Add “User” as Document type and “Insert New Records” as import type then click on “Save” button.
3. Then check all the fields and click on download template.
4. Open the downloaded file and enter required data.
5. In the downloaded file, under the row named as “Block Modules” add the modules that should not be visible to particular user. Then save it.
6. Then go to the data import, click on “Add Data Import”.
7. Add “User” as Document type and “Insert New Records” as import type and save it.
8. Then click on “Attach” under import file and attach the arranged file.
9. Click on “Start Importing” and wait until it completes importing. Then click on “Save”.








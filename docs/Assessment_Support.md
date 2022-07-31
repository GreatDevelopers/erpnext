# Documentation of Assessment module

First We have to create Assessment Criteria. Assessment Criteria is the parameter based on which you assess the Student.

For example, if the assessment was conducted for English or another subject, then we can evaluate students in English on various criteria like Writing, assessment(viva), Attendance etc.
Assessment criteria can be used while scheduling assessment plans for student groups and courses.
Then next , We have to create Assessment group tree (hierarchy for examination conducted in school) for one batch i.e 2021-2022
Steps to create Assessment criteria:-

1. First go to the Assessment criteria. Click on New Assessment Criteria.
2. Then give the name of assessment Criteria and assessment group.

## Assessment plan

Next Create Assessment plan which is scheduled to conduct the examination/assessment of a particular course for a group of students in an on-going academic term. For creating Assessment plan the prerequisite is a grading scale, so we need to create a grading scale for it.
To access the Assessment Plan, go to
Home > Education > Assessment > Assessment Plan
Steps to Create Assessment Plan:-

1. Go to the Assessment Plan list and click on New.
2. Select the Student Group for which you want to conduct the assessment.
3. Select the Course for which you are conducting the assessment.
4. Select the Assessment Group under which the assessment is being conducted.
5. Once you select the course, the Grading Scale would automatically be updated for the assessment.
6. Save

## Grading Scale

Grading Scale defines the threshold for the different grades obtained by the students, based on their scores in the assessment. For example , I have created a grading scale of Students obtaining a score of 100%  would be graded as O, students obtaining a score of 80% and below would be graded A- and so on.
After creating an Assessment plan for course 'English-4/A/MST -1'. Then there is the Assessment Result.

## Assessment Result

Assessment Result is log of marks/grades earned by the student for specific Assessment. Basically we can use the Assessment Result Tool for creating a log of marks of multiple students at the same time . It is based on Assessment plan.

## Assessment Result Tool

The Assessment Result Tool helps you enter marks earned by the Students for specific course. In this tool, based on the Assessment Plan, all the Students will be fetched into the Assessment Result Tool.
Also, Columns for Assessment Criteria will be where marks earned can be entered for each Student.
As you go on entering marks for a Student, and switch to the next student, in the backend, the Student Result record will be auto-created for that Student.
 

# Documentation of Support Module

## Issue
An Issue is an incoming query from a Customer, usually via email or from the Contact section of your website. 
In erpnext , Issue is an incoming query from a Customer. Issue can be created in two ways:-
The first is through the web portal and the other one is when a customer or student emails you on a support address. For example, a company or college has a support address(supportexample@gmail.com). When a customer or student sends an issue on this mail. Then the issue will be created automatically.
We have to set up email for this. First go to email account -> Append To  'issue'.
To access the Issue list, go to:
Home > Support > Issues > Issue

**How to Create Issue**

Issues are automatically created if you use the append to feature in E
You can also create an Issue manually, to do that:

1. Go to the Issue list, click on New.
2. Enter the Subject, Raised By, and a description of the Issue.
 
## Issue Type
  
Issue Type is useful for tagging and classifying Issues.
Classifying Issues helps in assigning the concerned team members to specific Issues. Examples of Issue Types can be: 'Functional', 'Technical', 'Hardware', etc. So engineers can be assigned to technical or hardware issues and consultants would be assigned to address functional issues.
To access the Issue Type list, go to:
Home > Support > Issues > Issue Type
To create an Issue Type, click on New and enter a name for the type. A description can be added.
 
## Issue Priority
  
Issue Priority indicates the urgency of solving an Issue
Users can create priorities like "Low", "Medium", "High", "Critical", etc. Issue Priority will be used while creating the Service Level Agreement.
To access the Issue Priority list, go to:
Home > Support > Issues > Issue Priority
To create an Issue Priority, click on New and enter a name for the type. A description can be added.

# Service Level Agreement

A service level agreement (SLA) is a contract between a service provider (either internal or external) and the end user on the level of service expected from the service provider.
To access the Service Level Agreement list, go to:
Home > Support > Service Level Agreement > Service Level Agreement
 
 
**How to Create a Service Level Agreement**

1. Go to the Service Level Agreement list, click on New.
2. Enter a name for the Service Level.
3. Select an Employee group, that will handle a particular Service Level.
4. Set a Holiday List. Service Level Agreement won't be applied in the days mentioned in the Holiday List.
5. 'Enable' determines if a Service Level Agreement is enabled or disabled.
6. Ticking 'Default Service Level Agreement' will apply this SLA to a customer if they don't have a particular SLA assigned to them.
7. Entity Type: Service Level Agreements can be assigned to a Customer/Customer Group/Territory enabling you to apply Service Level Agreement based on these factors.
8. Entity: Select the specific Customer/Customer Group/Territory.
9. Start / End Date: Defines the validity of the agreement.
10. Priorities: You can set multiple Issue Priorities and their Time to Respond and Resolve (in hours and mins).
11. Save
 




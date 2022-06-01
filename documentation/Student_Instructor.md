# Documentation for adding Students, enrolling them in Programs and creating users of all students.

**Following are steps to insert students manually through csv file.**


## For Student Applicants:-

1. First, Go to the Student Applicant. Then click on import then Add Data Import. Then the New Data Import form will open. Here, add the doctype "Student Applicant" in the Document Type field, and select "Insert New Record" in Import Type. Then save it.
2. Then download the template with required fields like First name, Middle name, Last name, Program, Application Status etc. Application Status of all students should be "Approved". Otherwise we have to Approve all manually.
3. Create the csv file of all students according to the fields in the downloaded template. Then Attach csv file in "Import File". Then click on "Save" then "Start Import".
4. Here, if you find any error in fields then you can export the failed error logs, change it and upload it again.
5. Now all students will be visible in the Student Applicant List.


## For Enrolling Students in Programs:-

1. If you have already set the "Default Email" then go to step 3. Otherwise, In Settings, click on "Education Settings". Then the Education Setting page will open.
2. Then enable the option "Skip User creation for new Student".
3. In Tools, Click on Program Enrollment Tool, the new form will open.
4. Select "Student Applicant" in the field "Get Students From" and Select Program in which you want to enroll students. Select Academic Year and Academic Term.
5. Then click on "Get Students". Here, you will get all students from this Program.
6. Click on the "Enroll Students" button.
7. Repeat these steps for all Programs.
8. In Admission, click on Program Enrollment. Then all students will be visible here with status "Draft". You have to submit all then they will be in Submitted status and they automatically get enrolled in courses.


## For creating Users of Students:-

1. First, go to Student Applicants. Click on Import, then Add Data Import.
2. Then the New Data Import form will open. Here, add the doctype "Student Applicant" in the Document Type field, and select "Update Existing Record" in Import Type. Then save it.
3. Then, click on "Download Template". Select "All Records" in Export Type. Select the First Name, Middle Name, Last Name, Student Email Address and download the template.
4. Then the csv file of all students will be downloaded. In this, add the field "Set New Password" and create passwords of all students.
5. Add column "Role (Roles Assigned)" and write "Student" for all students.
6. Then go to the User list, click on import then Add Data Import. Then the New Data Import form will open. Here, add the doctype "User" in the Document Type field, and select "Insert New Record" in Import Type. Then save it.
7. Then attach the file, click on "Save" and then "Start Import".
8. All students will become users with Student role.


              
# Documentation of creating Users, Employee and Instructors.

## For Creating Users:- 

1. First, go to User, click on Import then Add Data Import.
2. Then the New Data Import form will open. Here, add the doctype "User" in the Document Type field, and select "New Data Record" in Import Type. Then save it.
3. Then download template with required fields like First name, Middle name, Last name, Email, Set New Password, Role (Roles Assigned) etc.
4. The csv file will be downloaded. Add the data of instructors in this file. Role (Roles Assigned) should be "Instructor" for all instructors.
5. Then attach the file, click on "Save" and then "Start Import". Then all users will be visible in the User List.

## For Creating Employees:-

1. First, go to User, click on Import then Add Data Import.
2. Then Download the template of All Records with First Name, Middle Name, Last Name, ID etc. Because we need the Id of users to link with Employees.
3. Then go to HR, click on "Employee".
4. In Employee, click on Import then Add Data Import. Then Download the template with required fields like Company, Date of Joining, Date of Birth etc.
5. Then add the data in the downloaded csv file and attach the file.
6. Click on Save then "Start Import". Then employees will be visible in the Employee List.


## For Creating Instructors:-

1. First, go to Instructor, then click on Import then Add Data Import.
2. Then Download template with required fields like Instructor name, Employee, Instructor Log etc. Then in the downloaded csv file, add data of instructors, in the "Employee" column, add Employee ID of respective instructor from Employee List.
3. You can add Programs and courses of Instructors in this file.
4. Then attach the file, click on save then "Start Import".
5. Then all the Instructors will be visible in the Instructor List.


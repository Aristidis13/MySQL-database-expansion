# MYSQL_project

This is a project that is about relational MySQL Database handling.
A Database about an erecruitment system is given, and you have to add more tables and appropriate information to them.
Also queries have to be constructed that extract information from the tables.
Specifically, there are two types of users that interact with the database.A recruiter and a candidate.

# The 3 tables are:
- `interview` a table that will provide the opportunity to add comments about an interview and the personality of a job applicant to the recruiter. 
- `sectors` a table that is recursive and contains sectors for for every company. For example if a company is an IT company it can furtherly be specified as
a web development company and even a more specific sector.
- `changes` this is a history table that contains will automatically store information if a change happens in the database.
Specifically it will contain the username of the user that made the change, the time that the change occured,the success or failure of this update the type of the change
('UPDATE','DELETE','INSERT') and the name of the table that the change occured.

The files that are showed are these:
- db.txt : The database that I was given by my professor
- createAnInsert.txt : A file that contains the create statements for my project and the insertion of data to the interview table for extracting results.
- changes_triggers.txt : This is the file that contains all of the triggers that are required to update the changes table (TOTAL of 12 triggers that cover all of the combinations). 
- preventTrigger.txt : This is a trigger that prevents the deletion of an application if the submission_date has passed. This ensures some integrity to the system and the recruiter will not be able to favor any candidate in favor of another
- test Queries.txt : This is a file that contains testing of the triggers above.
- S_P.txt : This is the implementation of a stored procedure, that accepts as input a job position id and returns two tables one with the ranking of every canddate that applied for the 
job and the number of his interviews for this particular job. Additionally if the there are candidates that are excluded from the final desision due to personality or another reason are presented in asecond table along with the reason they were disqualified. 
- Selects.txt : This file contains all the SELECT queries that my professor wanted. Pick what you want and ask the database.

To run the files first copy-paste the db_txt file in the MySQL workbench.
After that run the createAnInsert.txt to extend the database.
Then run the changes_triggers.txt and the preventTrigger.txt.
Then run the S_P.txt and the Selects (if you want more info about this dummy database)

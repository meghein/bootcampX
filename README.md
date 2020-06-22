We've received our first round of queries that need to be written for BootcampX. It's now time to start writing the SQL Queries.

Setup
Create a new directory in BootcampX called 1_queries.

Remember to create a new file for each individual query.

Tips
Remember to try writing the query, even if you don't know exactly how it should be written.
Build your queries incrementally and run them against the database as many times as you want.
Reference the weekend material if you need help remembering how to do something.
Requirements
Students in Cohort
Get the names of all of the students from a single cohort.

Select their id and name.
Order them by their name in alphabetical order.
Since this query needs to work with any specific cohort, just use any number for the cohort_id.
Expected Result:

id |       name        
----+-------------------
  1 | Armand Hilll
 13 | Brian Jones
 16 | Carmel Grant
 14 | Clint Cremin
 17 | Colten Gutkowski
...
(18 rows)
Your Answer
Type in your answer here and Compass will let you reveal our answer below. Compass will auto-save your answer as you type. Once you click Toggle Answer below, your answer cannot be changed.
Total Students in Cohorts
The admissions department wants to know the total number of students from any number of cohorts combined.

Select the total number of students who were in the first 3 cohorts.

Expected Result:

 count 
-------
    48
(1 row)
Your Answer
Type in your answer here and Compass will let you reveal our answer below. Compass will auto-save your answer as you type. Once you click Toggle Answer below, your answer cannot be changed.
Contact Details
We need to make sure that we can contact students through a phone number or through email. If student's don't have a phone number or email associated with their account, we'll need to message them on slack to update their details.

Get all of the students that don't have an email or phone number.

Get their name, id, and cohort_id.
Expected Result:

       name       | id  
------------------+-----
 Aurore Yundt     | 160
 Cory Toy         | 161
 Kurt Turcotte    | 163
 Elda McClure     | 164
 Luisa Sipes      | 168
...
(17 rows)
Your Answer
Type in your answer here and Compass will let you reveal our answer below. Compass will auto-save your answer as you type. Once you click Toggle Answer below, your answer cannot be changed.
Non Gmail Students
Recently we've been having trouble emailing students without a gmail account. To make sure that we can reliably contact all students, we'll need to make sure that student's without a gmail account have a phone number.

Get all of the students without a gmail.com or phone number.

Get their name, email, id, and cohort_id.
Expected Result:

      name       | id  |           email           | cohort_id 
-----------------+-----+---------------------------+-----------
 Javonte Ward    | 178 | jessie_howell@hotmail.com |        12
 Jessika Jenkins | 187 | stephanie.koss@kevon.io   |        12
 Jerrold Rohan   | 189 | wehner.twila@hotmail.com  |        12
(3 rows)
Your Answer
Type in your answer here and Compass will let you reveal our answer below. Compass will auto-save your answer as you type. Once you click Toggle Answer below, your answer cannot be changed.
Currently Enrolled Students
A student's end date will be NULL when they are currently enrolled in Bootcamp.

Get all of the students currently enrolled.

Get their name, id, and cohort_id.
Order them by cohort_id.
Expected Result:

        name         | id  | cohort_id 
---------------------+-----+-----------
 Deon Hahn           | 151 |        11
 Sean Bartell        | 152 |        11
 Sarai Flatley       | 153 |        11
 Billie Mitchell     | 154 |        11
 Vance Kihn          | 155 |        11
...
(42 rows)
Your Answer
Type in your answer here and Compass will let you reveal our answer below. Compass will auto-save your answer as you type. Once you click Toggle Answer below, your answer cannot be changed.
Github Activity
Once a student graduates, the career services department needs to keep track of their activity on Github. If a graduate has not linked their Github account, we need to contact them to do so.

Get all graduates without a linked Github account.

Get their name, email, and phone.
Expected Result:

       name        |             email             |    phone     
-------------------+-------------------------------+--------------
 Herminia Smitham  | sawayn.sarina@yahoo.com       | 778-251-5094
 Jacinthe Kautzer  | litzy_fay@hilpert.net         | 075-883-5570
 Bernardo Turcotte | margarita.anderson@paolo.name | 814-473-6929
 Eloisa Quigley    | schmidt.ansel@gmail.com       | 276-965-2022
 Tiana Altenwerth  | zelda.stanton@yahoo.com       | 448-872-0954
 Hailie Kutch      | zora.corkery@goldner.net      | 249-763-9998
(6 rows)
Your Answer
Type in your answer here and Compass will let you reveal our answer below. Compass will auto-save your answer as you type. Once you click Toggle Answer below, your answer cannot be changed.
Submit Assignment
Once you've completed all of the queries, it's time to push your work and mark this activity as completed.

Commit and push your code, then post a link to the 1_queries directory on Github.
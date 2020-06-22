For the BootcampX project, we will need to write many queries. In this exercise, we will go over the process that should be used when writing each query.

Requirements
In future exercises, we will receive a list of requirements that we will have to write queries for. Each query will be written in it's own .sql file. Before starting a new exercise, create a new directory that all of the query files can be stored in.

Because each query will be inside its own file, we can write all of the SQL code in our text editor. We will then execute the query against our database using \i filename.sql from within our psql session.

We will now go over an example requirement and write the query for it. Before we start writing queries, let's create a new directory for this exercise.

Create a new directory in BootcampX called 0_selects

Example Requirement
We need a list of all of the students that haven't added their Github username to their account yet, so that we can tell them to add it.

Your task is to get all students without a Github username.

Select their id, name, email, and cohort_id.
Order them by cohort_id.
Expected Result:

 id  |       name        |             email              | cohort_id 
-----+-------------------+--------------------------------+-----------
  99 | Herminia Smitham  | sawayn.sarina@yahoo.com        |         7
 102 | Jacinthe Kautzer  | litzy_fay@hilpert.net          |         7
 111 | Bernardo Turcotte | margarita.anderson@paolo.name  |         8
 123 | Eloisa Quigley    | schmidt.ansel@gmail.com        |         9
 128 | Tiana Altenwerth  | zelda.stanton@yahoo.com        |         9
...
(20 rows)
Results will be truncated in order to save space on the screen. In this example, there are 20 rows and these are the first 5.

Steps
Create a New SQL File
Before doing anything, start by creating a new .sql inside the 0_selects. Name the file whatever you like, but adding a number at the beginning can help organize. A good name for this requirement might be 1_students_without_github.sql.

Create a new file inside the 0_selects named 1_students_without_github.sql.

Write The Query
Open the file in your text editor and start writing the query. The query for this requirement can be found below. Try writing it yourself before looking at the answer.

Add the following SQL to your SQL file.

Format your SQL code correctly to make it more readable.

Use a separate line for each clause.
Uppercase each reserved SQL keyword.
Execute The Query
As you're writing the query, you should be incrementally executing it in the database to make sure it's working correctly. There is no penalty for executing queries so execute as many times as you like.

Execute the SQL file.

Make sure you're in a psql session.
Execute psql from, the BootcampX directory.
Make sure you're using the bootcampx database \c bootcampx
Execute the query with the following command:
\i 0_selects/1_students_without_github.sql
Check The Answer
The expected result will be posted with the requirement. Make sure to compare your answer with the expected result to make sure it's correct.

Conclusion
In this exercise we walked through the process of completing a single query for BootcampX. In the following exercises, there will be many queries to complete, use this process for each of them.


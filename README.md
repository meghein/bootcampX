# The Entities
## The main entities for this application will be:

students
cohorts
assignments
assignment_submissions
teachers
assistance_requests
We're going to start off simple and just focus on the queries for two entities: students and cohorts.

A cohort will have the following attributes:

id: A unique identifier
name: The name of the cohort
start_date: The cohorts' start date
end_date: The cohorts' end date
A student will have the following attributes:

id: A unique identifier
name: The full name of the student
email: The students' email address
phone: The students' phone number
github: The students' github profile url
start_date: The students' start date of the Bootcamp
end_date: The students' end date of the Bootcamp
cohort_id: The id of the cohort that the student is enrolled in

### We can model these entities in an Entity Relation Diagram (ERD):
- We will get much more into creating ERDs and Database Design in the next couple of days. For now, we will be mainly focusing on querying the database.

# Create a Database
Using the ERD, we can create tables for the database; but before we do that, we need a database.

Start a new psql session.

From within the bootcampx directory, enter psql into terminal.

Create a database called bootcampx

-- Create the database
CREATE DATABASE bootcampx;
-- Start using the database
\c bootcampx;
You will have to enter \c bootcampx every time you enter a new psql session to make sure that you're using the correct database.

# Tables
Now that we have a database, we can create the tables for our student and cohort entities.

Write the CREATE TABLE statements for the students and a cohorts tables.

Create a folder called migrations within the BootcampX folder.
Inside migrations, create a new file called students_cohorts.sql
Take a moment to try writing the CREATE TABLE statements yourself for students and cohorts. Use the ERD to help.
Once you've given it a try, toggle the code block below to reveal our version of the code.
Make sure the code in your students_cohorts.sql file is identical to the code below.
Add the tables to the database.

From your psql session, type \i migrations/students_cohorts.sql
Now enter \dt into your psql session to make sure the two tables have been created.
Student and Cohort Data
Take a look at all of the data in the students and cohorts tables.

In psql, enter the following commands:

SELECT * FROM students;
SELECT * FROM cohorts;
We haven't added any data yet, so both tables contain 0 rows. Let's change that. We're going to need to add some fake data to test our queries against.

Once the database is in production, it will contain lots of data, hundreds or maybe thousands of rows in each table, so we'll need to test our queries on a large set of data. This means we'll need hundreds of fake students to test with.

Don't worry though, we're not going to write hundreds of INSERT statements; instead, we'll have some software generate a whole bunch of fake data. In fact, the project manager has already done this for us and uploaded the .sql files.

Students http://bit.ly/2Z0fN4t
Cohorts http://bit.ly/300nIQy
Download the .sql files with the fake data in them.

Create a folder named seeds inside the BootcampX folder.
Download both of the .sql files using wget.
wget http://bit.ly/2Z0fN4t -O seeds/students.sql

wget http://bit.ly/300nIQy -O seeds/cohorts.sql
We now have two files in the seeds directory, cohorts.sql and students.sql.

Open the students.sql file and take a look at the data. Just rows and rows of fake student data. Let's add this data to the tables.

Run the cohorts.sql and students.sql files against the bootcampx database.

Inside the psql session, run the following commands:

\i seeds/cohorts.sql
\i seeds/students.sql
This will result in a bunch of INSERT 0 1 appearing in the terminal window. Now try running the following command:

SELECT count(*) FROM students;
We've got 192 students to query against.

Submit Code
For the BootcampX project, we will be tracking everything in a single git repo.

Create a git repo for BootcampX.

Initialize a new git repo in the BootcampX folder git init.
Commit all of the current code.
Create a new repo on Github for the project.
Push your project to Github.
Submit a link to the project in this assignment.

Conclusion
In this activity we setup the BootcampX database, added two tables, and seeded those tables with a bunch of fake data. With all of this setup, we can now start writing queries for BootcampX.
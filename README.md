Download Link: https://assignmentchef.com/product/solved-cs532-homework-4
<br>
<ol>

 <li>Write relational algebra expressions to answer the following query statements based on the tables used in Project 1. It is okay to answer a query in multiple steps. You need to make sure that your relational algebra expressions are reasonably optimized as we discussed in class, i.e., conditions involving a single table should be specified on that table directly and Cartesian products should be replaced by joins whenever possible.</li>

</ol>

<ul>

 <li>For each TA from the CS department, find his/her B#, first name and birth date.</li>

 <li> For each class that has a PhD student TA, find its classid, dept_code and course# as well as the TA’s first name and email.</li>

 <li>Find the B# and first name of each MS student who did not take any course.</li>

 <li>Find the classid, dept_code and course# of each class that has been taken by all juniors.</li>

</ul>

<ol start="2">

 <li> Consider the two tables Courses and Classes used in Project 1. Test the following with real SQL statements in your Oracle account and report the result of each test case (including the SQL statements used).</li>

</ol>

<ul>

 <li>Try to drop table Courses using “drop table courses;”. Report what happened.</li>

 <li>Try to drop table Courses using “drop table courses cascade constraints;”). Did the table Courses get dropped? Did any tuples from table Classes get deleted?</li>

 <li>Following the statement in (b), analyze what happened to the foreign key (dept_code, course#) in Classes that references the primary key of Courses? Use SQL statement(s) and the results to explain your answer.</li>

</ul>

<ol start="3">

 <li> The Referential Integrity Constraint says that any value under a foreign key must either be a null value or a value matching a value under the corresponding primary (candidate) key. When a foreign key FK in table R1 has two attributes (A, B), there are two possible ways to define the meaning of a null value: (i) both A and B have null values, i.e., (null, null) and (ii) at least one of the values under A and B is a null value, i.e., (null, b), (a, null) or (null, null), where a and b are non-null values. In Project 1, the foreign key (dept_code, course#) in table Classes has two attributes that reference the primary key of table Courses. Use the two tables and design experiments in Oracle to answer the following questions. Report your queries for each experiment.</li>

</ol>

<ul>

 <li>Which of the above two meanings, i.e., (i) and (ii), is adopted by Oracle? Note that for this experiment, the schema for table Classes needs to be modified to allow null values for both dept_code and class# (just remove “not null” for them</li>

</ul>

<ul>

 <li>Is it possible to insert a tuple in table Classes such that its values under (dept_code, course#) have one null value (say under dept_code) and a non-null value (say under course#) and the non-value does not match any value under course# in table Courses?                                                                                 1</li>

</ul>

<ol start="4">

 <li> Create a simple view CSCourses on table Courses from Project 1 in your Oracle account. CSCourses logically contains only CS courses from Courses.</li>

</ol>

<ul>

 <li>Try to insert a tuple into, delete a tuple from, and update a value of Courses through CSCourses.</li>

 <li>Try to insert a new math course into Course via CSCourses. Note that this new course does not logically belong to CSCourses. Report whether you succeeded.</li>

</ul>




Save your work in one or more spool files and hand in the files.






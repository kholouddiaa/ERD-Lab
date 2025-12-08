\# ERD Lab – Company Projects \& Employees



This repository contains ERD diagrams and exercises for modeling a company database.



---



\## Case 1 – Company Database



A big company has decided to store information about its projects and employees in a database.  

You have been hired as a \*\*database designer\*\* to prepare an \*\*E-R diagram\*\* according to the following description:



\### 1. Employees

\- The company has a number of employees.

\- Each employee has the following attributes:

&nbsp; - `SSN`

&nbsp; - `BirthDate`

&nbsp; - `Gender`

&nbsp; - `FName`

&nbsp; - `LName`

&nbsp; - `Address`

&nbsp; - `Salary`

\- Each employee \*\*works on several projects\*\*.

\- Each employee \*\*must work in exactly one department\*\*.

\- Each employee has \*\*a number of working hours\*\* in each project.



\### 2. Departments

\- The company has a set of departments.

\- Each department has:

&nbsp; - `DName`

&nbsp; - `DNUM` (unique identifier)

&nbsp; - `Locations`

\- Each department has \*\*one employee assigned as a manager\*\*, and each manager has a \*\*HiringDate\*\*.

\- Each department:

&nbsp; - \*\*May have employees\*\*

&nbsp; - \*\*Has a set of projects\*\*

&nbsp; - Each project must be \*\*assigned to exactly one department\*\*



\### 3. Projects

\- Each project has the following attributes:

&nbsp; - `PName`

&nbsp; - `PNumber` (identifier)

&nbsp; - `Location`

&nbsp; - `City`

\- Employees work on several projects, and each project has several employees  

&nbsp; → This is a \*\*many-to-many relationship\*\* with an attribute:

&nbsp; - `Hours` (employee hours on a project)



\### 4. Dependents

\- Each employee has a set of dependents.

\- Each dependent has:

&nbsp; - `DependentName` (unique per employee)

&nbsp; - `Gender`

&nbsp; - `BirthDate`

\- \*\*Note:\*\* If the employee leaves the company, \*\*dependent information is deleted\*\*.



---



\## ERD Diagrams



\### \*\*Problem 1 – ERD\*\*

!\[Problem 1](./Problem1/erd\_problem1.png)



---



\### \*\*Problem 2 – ERD\*\*

!\[Problem 2](./Problem2/erd\_problem2.png)



---



\### \*\*Problem 3 – ERD\*\*

!\[Problem 3](./Problem3/erd\_problem3.png)



---



\### \*\*Problem 4 – ERD\*\*

!\[Problem 4](./Problem4/erd\_problem4.png)



---



\## Notes

\- Each ERD diagram illustrates entities, relationships, and attributes clearly.

\- Folder organization ensures clean structure and easy navigation.

\- You can expand the repository later with SQL scripts or relational schemas.



---



\### Created with  by Kholoud




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

\- For each department, there is always \*\*one employee assigned to manage\*\* that department.

\- Each manager has a \*\*HiringDate\*\* (date they started managing the department).

\- Each department:

&nbsp; - \*\*May have employees\*\*.

&nbsp; - \*\*Has a set of projects\*\*.

&nbsp; - Each project must be \*\*assigned to exactly one department\*\*.



\### 3. Projects

\- Each project has the following attributes:

&nbsp; - `PName`

&nbsp; - `PNumber` (identifier)

&nbsp; - `Location`

&nbsp; - `City`

\- Employees work on several projects, and each project has several employees  

&nbsp; → this is a \*\*many-to-many relationship\*\* with an attribute:  

&nbsp; - `Hours` (working hours of an employee on a project).



\### 4. Dependents

\- Each employee has a set of dependents.

\- Each dependent has:

&nbsp; - `DependentName` (unique per employee)

&nbsp; - `Gender`

&nbsp; - `BirthDate`

\- \*\*Note:\*\* If the employee leaves the company, there is \*\*no need to store\*\* his/her dependents’ information (i.e. dependent existence depends on employee).



---




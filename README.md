Contents

Problem 1: Musicana (Musicians, Albums, Songs, Instruments)

Problem 2: Real Estate Firm (Sales Offices, Employees, Properties, Owners)

Problem 3: General Hospital (Wards, Patients, Consultants, Nurses, Drugs)

Problem 4: Airlines Database (Airlines, Employees, Aircrafts, Routes, Crew, Transactions)

Problem 1 – Musicana Records (Conceptual Schema)

Musicana records store data about:

Musicians (ID, Name, Address: Street/City, Phone)

Instruments (Unique Name, Musical Key)

Albums (Unique Title, Copyright Date, Album Identifier)

Songs (Unique Title, Author)

Key business rules:

A musician can play multiple instruments, and an instrument can be played by multiple musicians (M:N).

Each album contains multiple songs, and each song must appear on exactly one album.

Each song is performed by one or more musicians, and a musician can perform many songs (M:N).

Each album has exactly one producer (a musician), and a producer can produce many albums (1:N).

Problem 2 – Real Estate Firm (E-R Diagram)

The firm manages:

Sales Offices (Office_Number, Location)

Employees (Employee_ID, Employee_Name)

Properties (Property_ID, Location = Address, City, State, Zip_Code)

Owners (Owner_ID, Owner_Name)

Key business rules:

Each office can have zero or more employees.

Each employee must be assigned to exactly one office.

Each office has exactly one manager (who is an employee), and a manager manages only one office.

Each property must be listed with exactly one office; an office may list zero or more properties.

Each property can have zero or more owners.

Each owner must own one or more properties.

Store PercentOwned for each (Owner, Property).

Problem 3 – General Hospital (E-R Diagram)

The hospital system includes:

Wards (Ward_ID, Name)

Patients (Patient_ID, Name, Date_Of_Birth)

Consultants (Consultant_ID, Name)

Nurses (Number, Name, Address)

Drugs (CodeNumber, RecommendedDosage, BrandNames…)

Key business rules:

Each ward can host many patients, and each patient is hosted by only one ward (1:N).

Each patient has one leading consultant, but may also be examined by other consultants.

Consultants may be assigned/examine zero or more patients.

The system records each time a nurse gives a patient a drug:

Drug + Dosage + DateTime + Patient + Nurse

Each ward is under supervision of one nurse, and a nurse supervises only one ward (1:1).

Each nurse must serve in one ward, and a ward can have many nurses (1:N).

A drug can have more than one brand name.

Problem 4 – Major Airlines Database (E-R Diagram)

The database stores:

Airlines (ID, Name, Address, Contact Person, Telephone Numbers)

Employees (Employee_ID, Name, Address, Birthday (Day/Month/Year), Gender, Position, Qualifications)

Aircrafts (Aircraft_ID, Capacity, Model)

Routes (Route_ID, Origin, Destination, Distance, Classification: Domestic/International)

Transactions (Transaction_ID, Date, Description, Amount)

Key business rules:

Each airline owns multiple aircrafts (1:N).

Aircrafts are assigned to routes (M:N) and record:

NumberOfPassengers, PricePerPassenger, DepartureDateTime, ArrivalDateTime, TravelTime

Each aircraft has its own crew:

Major Pilot, Assistant Pilot, Two Hostesses
(Crew are NOT stored as employees.)

Each crew is assigned to only one aircraft.

The airline records buy/sell transactions (ticket sales, maintenance payments, etc.).

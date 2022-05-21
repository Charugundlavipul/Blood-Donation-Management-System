# Blood-Donation-Management-System

## Main Objective:
A portal for allowing users to donate and receive blood at scheduled date and time which also keeps track of amount of blood of various blood groups stored in the hospitals.
## Features implemented:
### Donate Blood:
-> Schedule appointments to donate blood.
-> Keep track of scheduled donate appointments in “Appointments” drop down menu.
-> Won’t let users with permanent diseases to donate blood.
-> Won’t let users with temporary conditions such as flu, pregnancy etc. to donate blood.
-> Won’t let users to schedule appointments prior to the current date of the computer.
-> Won’t let minors and senior citizens(>65) to donate blood.
### Receive Blood:
-> Schedule appointments to receive blood.
-> Keep track of scheduled receive appointments in “Appointments” drop down menu.
-> Won’t let users to schedule appointments prior to the current date of the computer and 2 days after the current date of the computer (This is done to help users with immediate requirements to receive blood).
-> Max amount of blood that could be received by a recipient is limited to 10 units (Amount required for total transfusion).
-> Giving appointments based on compatibility table attached below if stock isn’t available at a particular hospital program will prompt the user to select other hospitals.
### Appointments:
-> Appointments drop down menu allows users to keep track of scheduled appointments.
### Help:
-> Helps the user to know all the functionalities of the program
### Profile:
-> Allows user to log into their profiles
-> Allows users to update their profile and change details and password.
### Home Page:
-> Displays welcome message to the user depending upon His/her name.
-> Displays information of all the hospitals in a city as well as the stock of various blood group stored in the hospital.
-> Filters the hospitals being displayed based on the city, area and hospital name selected in the combo box.
## Schema of the tables:
### User Table:
-> Stores the information provided by the user during signup
-> “UserId” is the primary key generated automatically by the program
-> The rest of the attributes are taken as input from the user and stored in the table
### Hospitals Table:
-> Stores the information of the hospitals
-> “HosId” is the primary key manually given by the programmer
-> Rest of the attributes were entered by the programmer
### donorappointments Table:
-> Stores the scheduled appointments of the donor
-> “DID” is the primary key generated automatically by the program
->”UserId” is the foreign key which references the primary key of the User in “User” table
-> Rest of the attributes are taken as input from the user and stored in the table
###  recipientappointments Table:
-> Stores the scheduled appointments of the recipient
-> “RID” is the primary key generated automatically by the program
->”UserId” is the foreign key which references the primary key of the User in “User” table
-> Rest of the attributes are taken as input from the user and stored in the table

# Hospital API

> This api is used for managing the doctors and pateints, doctors can track the patients .

## Technologies Used

1.  Nodejs
2.  Express
3.  MongoDB for database

## Prerequisites

- MongoDB
- Node.js 
- Command Line Tools
- Visual Studio Code
- Postman for testing

## Installation

##### # Get the latest snapshot

`git clone https://github.com/samir-sayyed/hospital-api.git myproject`

##### # Change directory

`cd myproject`

##### # Install NPM dependencies

`npm install`

##### # Then simply start your app

`npm start`

#### # The Server should running at: http://localhost:8000

## How to use 
- For registering doctor use - http://localhost:8000/api/v1/doctors/register
 
  -Enter following details
    1. name
    2. phone
    3. address
    4. speciality
    5. password
    6. confirm_password

- For log in doctor use - http://localhost:8000/api/v1/doctors/login
 
  -Enter following details
    1. name
    2. password

- For registering patients use - http://localhost:8000/api/v1/patients/register
 
  -Enter following details
    1. name
    2. phone
    3. address

- For creating reports for patients use - http://localhost:8000/api/v1/patients/:id/create_report
 
  -Enter following details
    1. doctor
    2. status
    3. date

- For seeing all reports of patients use - http://localhost:8000/api/v1/patients/:id/all_reports

- For all the reports of all the patients filtered by a specific status use  http://localhost:8000/api/v1//reports/:status

## Folder Structure

## Hospital API <br>
├── config <br>
│ --- ├── mongoose.js <br>
│ --- └── passport-jwt-strategy.js <br>
├── controllers <br>
│ --- ├── doctors_controller.js <br>
│ --- ├── patients_controller.js <br>
│ --- └── reports_controller.js <br>
├── models <br>
│ --- ├── doctor.js <br>
│ --- ├── patient.js <br>
│ --- └── report.js <br>
├── routes <br>
│ --- ├── api <br>
│ ----│ -- ├── v1 <br>
│ --- │ -- │ -- ├── doctors.js <br>
│ --- │ -- │ -- ├── index.js <br>
│ --- │ -- │ -- ├── patients.js <br>
│ --- │ -- │ -- └── reports.js <br>
│ ----│ -- └── index.js <br>
│ --- └── index.js <br>
├── server.js <br>
├── package.json <br>
├── package-lock.json <br>
└── readme.md <br>

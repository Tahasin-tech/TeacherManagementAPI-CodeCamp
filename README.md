# Project Overview
## This project contains automated test cases for the Teacher Management APIs.

We have Tested the Authentication :
Login and Saved token (POST) 

We have automated the complete CRUD flow:

Create Teacher (POST)

Get All Teachers (GET)

Get Teachers by teacher ID (GET)

Filtered By Email (GET)

Filtered By Department (GET)

Search Student by Name (GET with query param)

Update Student (PUT)

Delete Student (DELETE)

Conducted Negetive test cases:
Login with wrong credentials (POST)

Access teachers without token (POST)

Get teacher with invalid ID (GET)

Create teacher with missing required field (POST)

The collection is built using Postman test scripts and can be executed using Newman to generate HTML reports.

## Tools Used
- Postman
- Newman
- Node.js
## Project Structure
The collection includes:

1. Authentication (POST)
   - Validates Status Code
   - Stores Token and shows in response
    - Shows Token is not Empty
  
2. Create Teacher (POST)
   - Validates Status Code
   - Checks ID exists in response
   - Validates Response matches sent/request data

3. Get All Teachers (GET)
   - Validates Status Code
   - Validates Response Schema
   - Checks Created Teacher Exists in List

4. Filter Teachers (GET)
   - Validates Department Filter Works Correctly
   - Validates Email Filter Works Correctly

5. Get Teacher by ID (GET)
   - Validates Status Code
   - Validates Returned ID Matches Teacher ID

6. Update Teacher (PUT)
   - Validates Status Code
   - Validates two Fields Updated Correctly

7. Delete Teacher (DELETE)
   - Validates Status Code
   - Validates Deleted Teacher Cannot Be Retrieved
   - GET by ID Returns 404 After Delete(GET)

8. Negative Tests
   - Validates Login with Wrong Credentials (POST)
   - Validates Access Teachers Without Token (POST)
   - Validates Get Teacher with Invalid ID (GET)
   - Validates Create Teacher with Missing Required Field Returns 400 (POST)


## How to run
- Clone the project

- give command ```npm i newman```

- Add env file to the project root

- Finally give command to execute ```npm test```

- Documentation: [[Postman documentation] ](https://documenter.getpostman.com/view/38007041/2sBXcLfxJZ)

- Test Cases: [[Test Cases]](https://docs.google.com/spreadsheets/d/16Jp0eDzK6djGbwgpRYRokJV004H8vTod/edit?usp=sharing&ouid=115080025741069195972&rtpof=true&sd=true)

## HTML Report:

<img width="894" height="901" alt="Screenshot 2026-03-08 144511" src="https://github.com/user-attachments/assets/eee0cd7c-6b9c-4d74-a222-2226f259daf0" />

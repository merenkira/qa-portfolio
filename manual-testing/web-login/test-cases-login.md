# Test Cases – Login Page (Web)

This file contains sample test cases for a typical web login form.

| ID           | Title                                | Preconditions                  | Steps                                                                 | Expected result                                   |
|--------------|--------------------------------------|--------------------------------|-----------------------------------------------------------------------|--------------------------------------------------|
| TC-LOGIN-001 | Login with valid credentials         | User has a registered account | 1. Open the login page<br>2. Enter valid email<br>3. Enter valid password<br>4. Click **Login** | User is logged in and redirected to the Dashboard |
| TC-LOGIN-002 | Login with incorrect password        | User has a registered account | 1. Open the login page<br>2. Enter valid email<br>3. Enter invalid password<br>4. Click **Login** | Error message is shown, user stays on the login page |
| TC-LOGIN-003 | Attempt to login with empty fields   | –                              | 1. Open the login page<br>2. Leave email and password empty<br>3. Click **Login** | Validation messages appear for required fields   |
| TC-LOGIN-004 | Login with invalid email format      | –                              | 1. Open the login page<br>2. Enter invalid email format (e.g. `user@`)<br>3. Enter any password<br>4. Click **Login** | Email field shows validation error                |
| TC-LOGIN-005 | Remember me checkbox functionality   | User has a registered account | 1. Open the login page<br>2. Enter valid email and password<br>3. Check **Remember me**<br>4. Click **Login**<br>5. Close and reopen the browser, return to the site | User stays logged in or email is pre-filled (according to requirements) |

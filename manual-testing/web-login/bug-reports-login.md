# Bug Reports – Demo Login Page

## BUG-LOGIN-001: Login button is not disabled during request

**Severity:** Medium  
**Priority:** High  
**Environment:** Web, Chrome (latest), Demo login page  

**Steps to reproduce:**
1. Open the login page.
2. Enter valid email and valid password.
3. Click **Login** several times quickly.

**Actual result:**  
Multiple requests are sent, the page freezes for a few seconds.

**Expected result:**  
After the first click, the **Login** button becomes disabled until the server responds.

---

## BUG-LOGIN-002: Generic error message for empty password

**Severity:** Low  
**Priority:** Medium  
**Environment:** Web, Chrome (latest), Demo login page  

**Steps to reproduce:**
1. Open the login page.
2. Enter valid email.
3. Leave the password field empty.
4. Click **Login**.

**Actual result:**  
Generic error message is shown: “Invalid email or password”.

**Expected result:**  
Specific validation message is shown: “Password is required”.

---

## BUG-LOGIN-003: Error message not cleared after successful login

**Severity:** Low  
**Priority:** Low  
**Environment:** Web, Chrome (latest), Demo login page  

**Steps to reproduce:**
1. Open the login page.
2. Enter valid email and invalid password.
3. Click **Login** → error message appears.
4. Correct the password and enter a valid password.
5. Click **Login** again.

**Actual result:**  
User is logged in, but the previous error message briefly remains visible or flashes.

**Expected result:**  
Error message is cleared immediately after a successful login attempt.

# E-commerce Application – Test Cases

## 1. User Registration

### TC-001: Register with valid user details

- **Scenario ID:** TS-001
- **Priority:** High
- **Type:** Positive
- **Preconditions:** The user does not have an existing account.
- **Test Data:**
  - Email: newuser@example.com
  - Password: ValidPassword123!
- **Test Steps:**
  1. Open the registration page.
  2. Enter a valid email address.
  3. Enter a valid password.
  4. Complete all other mandatory fields.
  5. Click the Register button.
- **Expected Result:** The account is successfully created and the user receives confirmation.

### TC-002: Register with an already registered email

- **Scenario ID:** TS-002
- **Priority:** High
- **Type:** Negative
- **Preconditions:** An account with the test email already exists.
- **Test Data:** Existing email address.
- **Test Steps:**
  1. Open the registration page.
  2. Enter an email address already associated with an account.
  3. Complete the remaining mandatory fields.
  4. Click the Register button.
- **Expected Result:** Registration is rejected and an appropriate error message is displayed.

### TC-003: Register with missing mandatory fields

- **Scenario ID:** TS-003
- **Priority:** High
- **Type:** Negative
- **Preconditions:** The registration page is accessible.
- **Test Data:** Leave one or more mandatory fields empty.
- **Test Steps:**
  1. Open the registration page.
  2. Leave mandatory fields empty.
  3. Click the Register button.
- **Expected Result:** Registration is rejected and validation messages are displayed.

### TC-004: Register with an invalid email format

- **Scenario ID:** TS-004
- **Priority:** Medium
- **Type:** Negative
- **Preconditions:** The registration page is accessible.
- **Test Data:** invalid-email-format
- **Test Steps:**
  1. Open the registration page.
  2. Enter an invalid email address.
  3. Complete the remaining mandatory fields.
  4. Click the Register button.
- **Expected Result:** The system rejects the invalid email format and displays a validation message.

## 2. User Login

### TC-005: Login with valid credentials

- **Scenario ID:** TS-005
- **Priority:** Critical
- **Type:** Positive
- **Preconditions:** A registered and active user account exists.
- **Test Data:**
  - Email: existinguser@example.com
  - Password: ValidPassword123!
- **Test Steps:**
  1. Open the login page.
  2. Enter the registered email address.
  3. Enter the correct password.
  4. Click the Login button.
- **Expected Result:** The user successfully logs in and is redirected to the appropriate account page.

### TC-006: Login with an incorrect password

- **Scenario ID:** TS-006
- **Priority:** High
- **Type:** Negative
- **Preconditions:** A registered user account exists.
- **Test Data:** Valid email address and incorrect password.
- **Test Steps:**
  1. Open the login page.
  2. Enter a registered email address.
  3. Enter an incorrect password.
  4. Click the Login button.
- **Expected Result:** Login is rejected and an appropriate error message is displayed.

### TC-007: Login with an unregistered email

- **Scenario ID:** TS-007
- **Priority:** High
- **Type:** Negative
- **Preconditions:** The user does not have an account with the test email.
- **Test Data:** unregistered@example.com
- **Test Steps:**
  1. Open the login page.
  2. Enter an unregistered email address.
  3. Enter a password.
  4. Click the Login button.
- **Expected Result:** Login is rejected and an appropriate error message is displayed.

### TC-008: Login with empty credentials

- **Scenario ID:** TS-008
- **Priority:** Medium
- **Type:** Negative
- **Preconditions:** The login page is accessible.
- **Test Data:** Empty email and password fields.
- **Test Steps:**
  1. Open the login page.
  2. Leave both fields empty.
  3. Click the Login button.
- **Expected Result:** Login is rejected and mandatory field validation messages are displayed.
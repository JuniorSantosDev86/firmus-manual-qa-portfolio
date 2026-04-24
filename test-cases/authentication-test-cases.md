# Authentication Test Cases — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Module | Authentication |
| Test Type | Manual Functional Testing |
| Tester | Junior Santos |
| Version | 1.0 |
| Status | In progress |

---

## 2. Module Overview

The authentication module is responsible for controlling user access to the Firmus application.

This test suite validates login behavior, logout behavior, session handling and protected route access from the user's perspective.

The goal is to ensure that authenticated users can access the system correctly and unauthenticated users are prevented from accessing private areas.

---

## 3. Test Scope

This test suite covers:

- Login with valid credentials
- Login with invalid credentials
- Required field validation
- Logout behavior
- Protected route access
- Redirection after login
- Redirection after logout
- Basic session persistence
- Basic authentication error feedback

Out of scope:

- Password recovery
- Multi-factor authentication
- Token inspection
- Backend authentication implementation
- Advanced security testing

---

## 4. Test Cases

---

## TC-AUTH-001 — Login with valid credentials

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-001 |
| Module | Authentication |
| Type | Functional |
| Priority | High |
| Severity if failed | Critical |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is on the login page.
- The user has valid credentials.

### Steps

1. Open the Firmus application.
2. Navigate to the login page.
3. Enter a valid email.
4. Enter a valid password.
5. Click the login button.

### Expected Result

The user should be successfully authenticated and redirected to the main dashboard.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This is a critical smoke test scenario.

---

## TC-AUTH-002 — Login with invalid email

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-002 |
| Module | Authentication |
| Type | Negative / Functional |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is on the login page.

### Steps

1. Open the Firmus application.
2. Navigate to the login page.
3. Enter an invalid or unregistered email.
4. Enter a valid password format.
5. Click the login button.

### Expected Result

The system should not authenticate the user and should display a clear error message.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

The error message should not expose sensitive authentication details.

---

## TC-AUTH-003 — Login with invalid password

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-003 |
| Module | Authentication |
| Type | Negative / Functional |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is on the login page.
- The user has a valid registered email.

### Steps

1. Open the Firmus application.
2. Navigate to the login page.
3. Enter a valid email.
4. Enter an incorrect password.
5. Click the login button.

### Expected Result

The system should not authenticate the user and should display a clear error message.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

The user should remain on the login page.

---

## TC-AUTH-004 — Login with empty email field

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-004 |
| Module | Authentication |
| Type | Negative / Validation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is on the login page.

### Steps

1. Open the Firmus application.
2. Navigate to the login page.
3. Leave the email field empty.
4. Enter a valid password.
5. Click the login button.

### Expected Result

The system should prevent login and indicate that the email field is required.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Validation feedback should be visible and understandable.

---

## TC-AUTH-005 — Login with empty password field

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-005 |
| Module | Authentication |
| Type | Negative / Validation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is on the login page.

### Steps

1. Open the Firmus application.
2. Navigate to the login page.
3. Enter a valid email.
4. Leave the password field empty.
5. Click the login button.

### Expected Result

The system should prevent login and indicate that the password field is required.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Validation feedback should be visible and understandable.

---

## TC-AUTH-006 — Login with both fields empty

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-006 |
| Module | Authentication |
| Type | Negative / Validation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is on the login page.

### Steps

1. Open the Firmus application.
2. Navigate to the login page.
3. Leave the email field empty.
4. Leave the password field empty.
5. Click the login button.

### Expected Result

The system should prevent login and indicate that the required fields must be filled.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Both required fields should provide clear validation feedback.

---

## TC-AUTH-007 — Access protected route without authentication

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-007 |
| Module | Authentication / Protected Routes |
| Type | Functional / Security Basic |
| Priority | High |
| Severity if failed | Critical |
| Status | Not Executed |

### Preconditions

- The user is not authenticated.
- The application is running.

### Steps

1. Open a new browser session or clear the current session.
2. Try to access a protected route directly.
3. Observe the system behavior.

### Expected Result

The system should prevent access to the protected route and redirect the user to the login page.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This is a critical route protection scenario.

---

## TC-AUTH-008 — Access protected route after login

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-008 |
| Module | Authentication / Protected Routes |
| Type | Functional |
| Priority | High |
| Severity if failed | Critical |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user has valid credentials.

### Steps

1. Open the Firmus application.
2. Log in with valid credentials.
3. Navigate to a protected route.
4. Observe the page behavior.

### Expected Result

The authenticated user should be able to access the protected route successfully.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

The protected area should load without redirecting the authenticated user back to login.

---

## TC-AUTH-009 — Logout from authenticated session

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-009 |
| Module | Authentication |
| Type | Functional |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The user is inside a protected area.

### Steps

1. Locate the logout option.
2. Click the logout button or menu item.
3. Observe the system behavior.

### Expected Result

The user should be logged out and redirected to the login page or another public page according to the expected application behavior.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

After logout, the user should not remain inside protected areas.

---

## TC-AUTH-010 — Access protected route after logout

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-010 |
| Module | Authentication / Protected Routes |
| Type | Functional / Security Basic |
| Priority | High |
| Severity if failed | Critical |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user has logged in successfully.
- The user has logged out successfully.

### Steps

1. Log in with valid credentials.
2. Log out from the application.
3. Try to access a protected route again.
4. Observe the system behavior.

### Expected Result

The system should prevent access and redirect the user to the login page or another public route.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This validates whether logout properly ends the authenticated session.

---

## TC-AUTH-011 — Refresh page while authenticated

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-011 |
| Module | Authentication / Session |
| Type | Functional |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The user is inside a protected area.

### Steps

1. Log in with valid credentials.
2. Navigate to a protected page.
3. Refresh the browser page.
4. Observe the system behavior.

### Expected Result

The user should remain authenticated and the protected page should load correctly, unless the application intentionally requires a new login.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the application intentionally expires the session after refresh, this behavior should be documented.

---

## TC-AUTH-012 — Login page visual and usability validation

| Field | Information |
|---|---|
| Test Case ID | TC-AUTH-012 |
| Module | Authentication |
| Type | Usability / Visual |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is on the login page.

### Steps

1. Open the login page.
2. Verify if the email field is visible.
3. Verify if the password field is visible.
4. Verify if the login button is visible.
5. Check if labels, placeholders or instructions are understandable.
6. Check if the layout is readable and visually consistent.

### Expected Result

The login page should be clear, readable and usable, with visible fields and understandable actions.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test supports basic usability validation.

---

## 5. Execution Summary

| Status | Total |
|---|---:|
| Passed | 0 |
| Failed | 0 |
| Blocked | 0 |
| Not Executed | 12 |

---

## 6. Notes for Execution

During execution, the tester should update each test case with:

- Actual result
- Status
- Evidence, when applicable
- Notes, when useful

If a test fails, a bug report should be created in the `bug-reports/` folder using the project bug report template.
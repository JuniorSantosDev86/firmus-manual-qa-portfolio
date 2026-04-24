# Clients Test Cases — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Module | Clients |
| Test Type | Manual Functional Testing |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | In progress |

---

## 2. Module Overview

The Clients module is responsible for displaying and managing client-related information within the Firmus application.

This test suite validates whether the user can access the clients area, view client records, interact with client-related actions and understand empty states or validation messages.

The goal is to ensure that client management flows are clear, reliable and usable from the user's perspective.

---

## 3. Test Scope

This test suite covers:

- Clients page loading
- Client list visibility
- Empty state behavior
- Client creation flow, when available
- Required field validation
- Invalid input validation
- Client details visibility, when available
- Navigation involving client records
- Basic visual consistency
- Basic responsive behavior
- Basic usability of client-related flows

Out of scope:

- Database validation
- Backend client persistence validation
- Bulk import or export
- Advanced segmentation
- Duplicate detection logic, unless visible in the UI
- API testing
- Automated testing

---

## 4. Test Cases

---

## TC-CLI-001 — Clients page loads successfully

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-001 |
| Module | Clients |
| Type | Functional / Smoke |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.

### Steps

1. Log in to the Firmus application.
2. Navigate to the clients area.
3. Observe the page loading behavior.

### Expected Result

The clients page should load successfully without errors, broken layout or unexpected redirects.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This is a smoke test for the clients module.

---

## TC-CLI-002 — Clients list is visible when records exist

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-002 |
| Module | Clients |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one client record exists.

### Steps

1. Access the clients page.
2. Observe the client list area.
3. Verify if client records are displayed.
4. Check if each record shows relevant client information.

### Expected Result

The clients page should display existing client records clearly and in an organized way.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the environment has no client records, this test may be marked as Blocked or Not Applicable.

---

## TC-CLI-003 — Clients empty state is clear when no records exist

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-003 |
| Module | Clients |
| Type | Functional / Empty State |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- No client records are available in the current environment.

### Steps

1. Access the clients page.
2. Observe the client list area.
3. Verify if an empty state message is displayed.
4. Check if the message is clear and helpful.

### Expected Result

The page should display a clear empty state explaining that no clients are available, without appearing broken or incomplete.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the environment always contains sample clients, this test may be marked as Not Applicable.

---

## TC-CLI-004 — Create client action is visible when available

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-004 |
| Module | Clients |
| Type | Functional / Usability |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The clients page is loaded.

### Steps

1. Access the clients page.
2. Look for a button or action to create a new client.
3. Verify if the action is visible and understandable.
4. Click the create client action, if available.

### Expected Result

The user should be able to identify the create client action and access the client creation flow when available.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If client creation is not available in the current version, document the behavior during execution.

---

## TC-CLI-005 — Create client with valid required information

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-005 |
| Module | Clients |
| Type | Functional |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The client creation flow is available.

### Steps

1. Access the clients page.
2. Click the create client action.
3. Fill in the required fields with valid client information.
4. Submit the form.
5. Observe the system behavior.

### Expected Result

The client should be created successfully, and the user should receive clear feedback or see the new client in the client list.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Use only fictional data during testing.

---

## TC-CLI-006 — Create client with required fields empty

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-006 |
| Module | Clients |
| Type | Negative / Validation |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The client creation flow is available.

### Steps

1. Access the clients page.
2. Click the create client action.
3. Leave required fields empty.
4. Submit the form.
5. Observe validation behavior.

### Expected Result

The system should prevent client creation and display clear validation messages for required fields.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Required fields should be understandable to the user.

---

## TC-CLI-007 — Create client with invalid contact information

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-007 |
| Module | Clients |
| Type | Negative / Validation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The client creation flow is available.
- The form includes contact fields such as email or phone.

### Steps

1. Access the client creation flow.
2. Fill required fields with valid information.
3. Enter invalid contact information, such as an invalid email format.
4. Submit the form.
5. Observe validation behavior.

### Expected Result

The system should prevent invalid contact data from being submitted or display a clear validation message.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the application does not validate contact format by design, document the observed behavior.

---

## TC-CLI-008 — Client details are visible when opening a client record

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-008 |
| Module | Clients |
| Type | Functional |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one client record exists.
- Client details view is available.

### Steps

1. Access the clients page.
2. Select an existing client record.
3. Open the client details view.
4. Verify if client information is visible and readable.

### Expected Result

The client details view should display relevant client information clearly.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the application does not have a details view, this test may be marked as Not Applicable.

---

## TC-CLI-009 — Client-related navigation works correctly

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-009 |
| Module | Clients |
| Type | Functional / Navigation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The clients page is loaded.

### Steps

1. Access the clients page.
2. Interact with available client-related navigation actions.
3. Navigate to another related area, if available.
4. Return to the clients page.
5. Observe if navigation works correctly.

### Expected Result

Client-related navigation should work without broken routes, unexpected errors or confusing behavior.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Any broken navigation should be documented as a bug.

---

## TC-CLI-010 — Clients page does not display broken or placeholder information

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-010 |
| Module | Clients |
| Type | Visual / Usability |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The clients page is loaded.

### Steps

1. Access the clients page.
2. Review visible titles, labels, cards, tables or list items.
3. Check for placeholder text.
4. Check for missing values.
5. Check for duplicated or broken information.

### Expected Result

The clients page should not display broken text, unexpected placeholder content, duplicated labels or visually incomplete information.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test helps identify polish and presentation issues.

---

## TC-CLI-011 — Clients page remains usable after refresh

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-011 |
| Module | Clients |
| Type | Functional / Session |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The clients page is loaded.

### Steps

1. Access the clients page.
2. Refresh the browser page.
3. Wait for the page to reload.
4. Observe the page behavior.

### Expected Result

The clients page should reload correctly and remain usable as long as the user session is still valid.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the session expires after refresh by design, document the behavior.

---

## TC-CLI-012 — Clients page is usable on mobile-like viewport

| Field | Information |
|---|---|
| Test Case ID | TC-CLI-012 |
| Module | Clients |
| Type | Responsive / Usability |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The clients page is loaded.
- The browser viewport is resized to a mobile-like width.

### Steps

1. Access the clients page.
2. Resize the browser to a mobile-like viewport or use DevTools device mode.
3. Verify if the client list or empty state remains readable.
4. Verify if buttons remain visible and usable.
5. Check if navigation remains accessible.
6. Check for horizontal scrolling or content overflow.

### Expected Result

The clients page should remain usable on a mobile-like viewport, without broken layout or unreadable content.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Any layout issue should be documented with screenshot evidence.

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

If a feature is not available in the current Firmus version, the related test case should be marked as Blocked or Not Applicable, with a clear note explaining why.
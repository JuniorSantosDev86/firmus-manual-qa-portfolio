# Quotes Test Cases — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Module | Quotes |
| Test Type | Manual Functional Testing |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | In progress |

---

## 2. Module Overview

The Quotes module is responsible for managing service quote workflows within the Firmus application.

This test suite validates whether the user can access the quotes area, view existing quotes, create new quotes, understand quote statuses and interact with quote-related actions.

The goal is to ensure that quote management flows are clear, reliable and usable from the user's perspective.

---

## 3. Test Scope

This test suite covers:

- Quotes page loading
- Quote list visibility
- Empty state behavior
- Quote creation flow, when available
- Required field validation
- Quote value input behavior
- Quote status visibility
- Quote details visibility, when available
- Public quote access, when available
- Navigation involving quote records
- Basic visual consistency
- Basic responsive behavior
- Basic usability of quote-related flows

Out of scope:

- Deep PDF generation validation
- Email delivery validation
- Payment-related behavior
- Backend calculation rules not visible in the UI
- Database validation
- API testing
- Automated testing

---

## 4. Test Cases

---

## TC-QUO-001 — Quotes page loads successfully

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-001 |
| Module | Quotes |
| Type | Functional / Smoke |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.

### Steps

1. Log in to the Firmus application.
2. Navigate to the quotes area.
3. Observe the page loading behavior.

### Expected Result

The quotes page should load successfully without errors, broken layout or unexpected redirects.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This is a smoke test for the quotes module.

---

## TC-QUO-002 — Quotes list is visible when records exist

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-002 |
| Module | Quotes |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one quote record exists.

### Steps

1. Access the quotes page.
2. Observe the quote list area.
3. Verify if quote records are displayed.
4. Check if each quote record shows relevant information, such as client, service, value or status.

### Expected Result

The quotes page should display existing quote records clearly and in an organized way.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the environment has no quote records, this test may be marked as Blocked or Not Applicable.

---

## TC-QUO-003 — Quotes empty state is clear when no records exist

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-003 |
| Module | Quotes |
| Type | Functional / Empty State |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- No quote records are available in the current environment.

### Steps

1. Access the quotes page.
2. Observe the quote list area.
3. Verify if an empty state message is displayed.
4. Check if the message is clear and helpful.
5. Check if the user receives guidance for creating a new quote, when applicable.

### Expected Result

The page should display a clear empty state explaining that no quotes are available, without appearing broken or incomplete.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the environment always contains sample quotes, this test may be marked as Not Applicable.

---

## TC-QUO-004 — Create quote action is visible when available

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-004 |
| Module | Quotes |
| Type | Functional / Usability |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The quotes page is loaded.

### Steps

1. Access the quotes page.
2. Look for a button or action to create a new quote.
3. Verify if the action is visible and understandable.
4. Click the create quote action, if available.

### Expected Result

The user should be able to identify the create quote action and access the quote creation flow when available.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If quote creation is not available in the current version, document the behavior during execution.

---

## TC-QUO-005 — Create quote with valid required information

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-005 |
| Module | Quotes |
| Type | Functional |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The quote creation flow is available.
- Required test data is available, such as a client and service description.

### Steps

1. Access the quotes page.
2. Click the create quote action.
3. Fill in all required fields with valid quote information.
4. Enter a valid quote value.
5. Submit the quote form.
6. Observe the system behavior.

### Expected Result

The quote should be created successfully, and the user should receive clear feedback or see the new quote in the quotes list.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Use only fictional data during testing.

---

## TC-QUO-006 — Create quote with required fields empty

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-006 |
| Module | Quotes |
| Type | Negative / Validation |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The quote creation flow is available.

### Steps

1. Access the quotes page.
2. Click the create quote action.
3. Leave required fields empty.
4. Submit the form.
5. Observe validation behavior.

### Expected Result

The system should prevent quote creation and display clear validation messages for required fields.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Required fields should be understandable to the user.

---

## TC-QUO-007 — Create quote with invalid monetary value

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-007 |
| Module | Quotes |
| Type | Negative / Validation |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The quote creation flow is available.
- The form includes a quote value field.

### Steps

1. Access the quote creation flow.
2. Fill required fields with valid information.
3. Enter an invalid monetary value, such as text, negative value or unsupported format.
4. Submit the form.
5. Observe validation behavior.

### Expected Result

The system should prevent invalid quote value submission or display a clear validation message.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the application accepts only formatted monetary values, this behavior should be documented.

---

## TC-QUO-008 — Quote status is visible and understandable

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-008 |
| Module | Quotes |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one quote record exists.

### Steps

1. Access the quotes page.
2. Locate an existing quote record.
3. Verify if the quote status is visible.
4. Check if the status label is clear and understandable.

### Expected Result

Each quote should display a clear and understandable status when applicable.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Examples of statuses may include draft, sent, accepted, rejected or similar, depending on the current application behavior.

---

## TC-QUO-009 — Quote details are visible when opening a quote record

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-009 |
| Module | Quotes |
| Type | Functional |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one quote record exists.
- Quote details view is available.

### Steps

1. Access the quotes page.
2. Select an existing quote record.
3. Open the quote details view.
4. Verify if quote information is visible and readable.

### Expected Result

The quote details view should display relevant quote information clearly, such as client, service description, value, status and related actions.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the application does not have a details view, this test may be marked as Not Applicable.

---

## TC-QUO-010 — Public quote access works when available

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-010 |
| Module | Quotes |
| Type | Functional / Public Flow |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- At least one quote has a public access page or shareable link.
- The public quote flow is available.

### Steps

1. Access or generate a public quote link.
2. Open the public quote link in a browser.
3. Observe the public quote page.
4. Verify if quote information is displayed clearly.
5. Check if no private internal information is exposed.

### Expected Result

The public quote page should load correctly and display only the information intended for public viewing.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If public quote access is not available in the current version, this test may be marked as Not Applicable.

---

## TC-QUO-011 — Quote-related navigation works correctly

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-011 |
| Module | Quotes |
| Type | Functional / Navigation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The quotes page is loaded.

### Steps

1. Access the quotes page.
2. Interact with available quote-related navigation actions.
3. Navigate to another related area, if available.
4. Return to the quotes page.
5. Observe if navigation works correctly.

### Expected Result

Quote-related navigation should work without broken routes, unexpected errors or confusing behavior.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Any broken navigation should be documented as a bug.

---

## TC-QUO-012 — Quotes page does not display broken or placeholder information

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-012 |
| Module | Quotes |
| Type | Visual / Usability |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The quotes page is loaded.

### Steps

1. Access the quotes page.
2. Review visible titles, labels, cards, tables or list items.
3. Check for placeholder text.
4. Check for missing values.
5. Check for duplicated or broken information.

### Expected Result

The quotes page should not display broken text, unexpected placeholder content, duplicated labels or visually incomplete information.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test helps identify polish and presentation issues.

---

## TC-QUO-013 — Quotes page remains usable after refresh

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-013 |
| Module | Quotes |
| Type | Functional / Session |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The quotes page is loaded.

### Steps

1. Access the quotes page.
2. Refresh the browser page.
3. Wait for the page to reload.
4. Observe the page behavior.

### Expected Result

The quotes page should reload correctly and remain usable as long as the user session is still valid.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the session expires after refresh by design, document the behavior.

---

## TC-QUO-014 — Quotes page is usable on mobile-like viewport

| Field | Information |
|---|---|
| Test Case ID | TC-QUO-014 |
| Module | Quotes |
| Type | Responsive / Usability |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The quotes page is loaded.
- The browser viewport is resized to a mobile-like width.

### Steps

1. Access the quotes page.
2. Resize the browser to a mobile-like viewport or use DevTools device mode.
3. Verify if the quote list or empty state remains readable.
4. Verify if buttons remain visible and usable.
5. Check if navigation remains accessible.
6. Check for horizontal scrolling or content overflow.

### Expected Result

The quotes page should remain usable on a mobile-like viewport, without broken layout or unreadable content.

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
| Not Executed | 14 |

---

## 6. Notes for Execution

During execution, the tester should update each test case with:

- Actual result
- Status
- Evidence, when applicable
- Notes, when useful

If a test fails, a bug report should be created in the `bug-reports/` folder using the project bug report template.

If a feature is not available in the current Firmus version, the related test case should be marked as Blocked or Not Applicable, with a clear note explaining why.
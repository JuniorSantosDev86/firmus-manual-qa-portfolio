# Financial Test Cases — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Module | Financial Overview |
| Test Type | Manual Functional Testing |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | In progress |

---

## 2. Module Overview

The Financial Overview module is responsible for presenting financial information and business visibility within the Firmus application.

This test suite validates whether the user can access the financial area, understand financial summary information, view monetary values clearly and interact with available financial-related actions.

The goal is to ensure that financial information is readable, organized, useful and consistent from the user's perspective.

---

## 3. Test Scope

This test suite covers:

- Financial page loading
- Financial summary cards
- Monetary value formatting
- Empty state behavior
- Financial records visibility, when available
- Pending, paid or overdue indicators, when available
- Basic filtering behavior, when available
- Navigation involving financial information
- Basic visual consistency
- Basic responsive behavior
- Basic usability of financial information

Out of scope:

- Accounting accuracy validation
- Tax calculation validation
- External financial integrations
- Payment gateway validation
- Bank reconciliation
- Database-level financial validation
- API testing
- Automated testing

---

## 4. Test Cases

---

## TC-FIN-001 — Financial page loads successfully

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-001 |
| Module | Financial Overview |
| Type | Functional / Smoke |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.

### Steps

1. Log in to the Firmus application.
2. Navigate to the financial area.
3. Observe the page loading behavior.

### Expected Result

The financial page should load successfully without errors, broken layout or unexpected redirects.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This is a smoke test for the financial module.

---

## TC-FIN-002 — Financial summary cards are visible

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-002 |
| Module | Financial Overview |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page is loaded.

### Steps

1. Access the financial page.
2. Locate the financial summary section.
3. Verify if summary cards are visible.
4. Check if each card has a clear label.
5. Check if each card displays a value or state.

### Expected Result

The financial page should display clear summary cards with readable labels and visible values or states.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Examples may include revenue, pending values, paid values, overdue values or similar indicators depending on the current application behavior.

---

## TC-FIN-003 — Monetary values are formatted correctly

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-003 |
| Module | Financial Overview |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page displays monetary values.

### Steps

1. Access the financial page.
2. Locate monetary values displayed on cards, lists or records.
3. Verify if values use a clear currency format.
4. Check if values are readable and consistent across the page.

### Expected Result

Monetary values should be displayed in a clear and consistent currency format.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the product uses Brazilian currency, values should be easy to understand for Brazilian users.

---

## TC-FIN-004 — Financial records are visible when records exist

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-004 |
| Module | Financial Overview |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one financial record exists.

### Steps

1. Access the financial page.
2. Locate the financial records section.
3. Verify if records are displayed.
4. Check if each record shows relevant information, such as description, value, status or date.

### Expected Result

The financial page should display existing financial records clearly and in an organized way.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the environment has no financial records, this test may be marked as Blocked or Not Applicable.

---

## TC-FIN-005 — Financial empty state is clear when no records exist

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-005 |
| Module | Financial Overview |
| Type | Functional / Empty State |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- No financial records are available in the current environment.

### Steps

1. Access the financial page.
2. Observe the financial records area.
3. Verify if an empty state message is displayed.
4. Check if the message is clear and helpful.
5. Check if the page avoids looking broken or incomplete.

### Expected Result

The page should display a clear empty state explaining that no financial records are available.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the environment always contains sample financial data, this test may be marked as Not Applicable.

---

## TC-FIN-006 — Financial status indicators are visible and understandable

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-006 |
| Module | Financial Overview |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- Financial records or summary indicators are available.

### Steps

1. Access the financial page.
2. Locate status indicators, such as paid, pending, overdue or similar states.
3. Verify if each status is visible.
4. Check if the status labels are understandable.

### Expected Result

Financial statuses should be visible, readable and understandable to the user.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Status labels should not be ambiguous or confusing.

---

## TC-FIN-007 — Financial page does not display negative or inconsistent values unexpectedly

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-007 |
| Module | Financial Overview |
| Type | Functional / Data Presentation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page displays values.

### Steps

1. Access the financial page.
2. Review financial summary cards and records.
3. Check if any value appears negative unexpectedly.
4. Check if any value appears missing, duplicated or inconsistent.
5. Observe if values match the visual context where they are displayed.

### Expected Result

Financial values should appear consistent with their labels and should not display unexpected negative, missing or duplicated information.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test validates visible data presentation only, not backend financial accuracy.

---

## TC-FIN-008 — Financial filters work when available

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-008 |
| Module | Financial Overview |
| Type | Functional / Filter |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page is loaded.
- Financial filters are available.

### Steps

1. Access the financial page.
2. Locate available filters, such as status, period or category.
3. Apply one filter.
4. Observe the displayed results.
5. Clear or change the filter, if possible.

### Expected Result

The financial page should update the displayed information according to the selected filter, or clearly indicate when no results are found.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If filters are not available in the current version, this test may be marked as Not Applicable.

---

## TC-FIN-009 — Financial-related navigation works correctly

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-009 |
| Module | Financial Overview |
| Type | Functional / Navigation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page is loaded.

### Steps

1. Access the financial page.
2. Interact with available financial-related navigation actions.
3. Navigate to another related area, if available.
4. Return to the financial page.
5. Observe if navigation works correctly.

### Expected Result

Financial-related navigation should work without broken routes, unexpected errors or confusing behavior.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Any broken navigation should be documented as a bug.

---

## TC-FIN-010 — Financial page does not display broken or placeholder information

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-010 |
| Module | Financial Overview |
| Type | Visual / Usability |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page is loaded.

### Steps

1. Access the financial page.
2. Review visible titles, labels, cards, tables or list items.
3. Check for placeholder text.
4. Check for missing values.
5. Check for duplicated or broken information.

### Expected Result

The financial page should not display broken text, unexpected placeholder content, duplicated labels or visually incomplete information.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test helps identify polish and presentation issues.

---

## TC-FIN-011 — Financial page remains usable after refresh

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-011 |
| Module | Financial Overview |
| Type | Functional / Session |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page is loaded.

### Steps

1. Access the financial page.
2. Refresh the browser page.
3. Wait for the page to reload.
4. Observe the page behavior.

### Expected Result

The financial page should reload correctly and remain usable as long as the user session is still valid.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the session expires after refresh by design, document the behavior.

---

## TC-FIN-012 — Financial page is readable on desktop viewport

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-012 |
| Module | Financial Overview |
| Type | Responsive / Visual |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page is loaded.
- The browser is using a desktop viewport.

### Steps

1. Access the financial page using a desktop viewport.
2. Verify if summary cards are aligned correctly.
3. Verify if monetary values are readable.
4. Verify if sections have proper spacing.
5. Verify if navigation remains visible and usable.

### Expected Result

The financial page should be readable, organized and usable on desktop viewport.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test supports basic responsive validation.

---

## TC-FIN-013 — Financial page is usable on mobile-like viewport

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-013 |
| Module | Financial Overview |
| Type | Responsive / Usability |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page is loaded.
- The browser viewport is resized to a mobile-like width.

### Steps

1. Access the financial page.
2. Resize the browser to a mobile-like viewport or use DevTools device mode.
3. Verify if summary cards remain readable.
4. Verify if financial records or empty states remain readable.
5. Verify if buttons remain visible and usable.
6. Check for horizontal scrolling or content overflow.

### Expected Result

The financial page should remain usable on a mobile-like viewport, without broken layout or unreadable content.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Any layout issue should be documented with screenshot evidence.

---

## TC-FIN-014 — Financial information is understandable for the user

| Field | Information |
|---|---|
| Test Case ID | TC-FIN-014 |
| Module | Financial Overview |
| Type | Usability / Content |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The financial page is loaded.

### Steps

1. Access the financial page.
2. Review the page title, section labels and financial cards.
3. Check if the user can understand what each number means.
4. Check if financial statuses are clear.
5. Check if the page provides useful business visibility.

### Expected Result

The financial page should communicate financial information clearly, helping the user understand the current business situation.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test helps evaluate the financial module from a real user's perspective.

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
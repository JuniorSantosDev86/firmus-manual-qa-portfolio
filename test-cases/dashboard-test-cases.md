# Dashboard / Control Tower Test Cases — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Module | Dashboard / Control Tower |
| Test Type | Manual Functional Testing |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | In progress |

---

## 2. Module Overview

The Dashboard / Control Tower is the main operational overview area of the Firmus application.

This test suite validates whether the dashboard loads correctly, displays relevant operational information, presents clear navigation options and provides a usable overview for the authenticated user.

The goal is to ensure that users can quickly understand the current state of their business operations after logging in.

---

## 3. Test Scope

This test suite covers:

- Dashboard loading after login
- Visibility of main dashboard sections
- Operational summary cards
- Next actions section
- Recent activities section
- Navigation from dashboard to related modules
- Empty state behavior, when applicable
- Basic visual consistency
- Basic responsive behavior
- Usability of dashboard information

Out of scope:

- Backend data validation
- Deep calculation validation
- Real-time update validation
- Database consistency checks
- Performance benchmarking
- Automated dashboard testing

---

## 4. Test Cases

---

## TC-DASH-001 — Dashboard loads after successful login

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-001 |
| Module | Dashboard / Control Tower |
| Type | Functional / Smoke |
| Priority | High |
| Severity if failed | Critical |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user has valid credentials.
- The user is on the login page.

### Steps

1. Open the Firmus application.
2. Log in with valid credentials.
3. Observe the page loaded after authentication.

### Expected Result

The user should be redirected to the dashboard or main operational area after successful login.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This is a critical smoke test because the dashboard is the main entry point after authentication.

---

## TC-DASH-002 — Dashboard main sections are visible

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-002 |
| Module | Dashboard / Control Tower |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The user is on the dashboard page.

### Steps

1. Access the dashboard.
2. Verify if the main dashboard title or heading is visible.
3. Verify if summary sections are visible.
4. Verify if the next actions section is visible.
5. Verify if the recent activities section is visible.

### Expected Result

The dashboard should display its main sections clearly, allowing the user to understand the operational overview.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If a section is intentionally hidden due to empty data, this behavior should be documented.

---

## TC-DASH-003 — Operational summary cards are displayed correctly

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-003 |
| Module | Dashboard / Control Tower |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard page is loaded.

### Steps

1. Access the dashboard.
2. Locate the operational summary cards.
3. Verify if each card has a clear label.
4. Verify if each card displays a visible value or state.
5. Check if the information is readable and visually organized.

### Expected Result

The dashboard should display summary cards with clear labels and readable values or states.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test validates whether the dashboard gives useful operational visibility.

---

## TC-DASH-004 — Next actions section is visible and understandable

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-004 |
| Module | Dashboard / Control Tower |
| Type | Functional / Usability |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard page is loaded.

### Steps

1. Access the dashboard.
2. Locate the next actions section.
3. Verify if the section title is clear.
4. Verify if the listed actions are readable.
5. Verify if action labels or statuses are understandable.

### Expected Result

The next actions section should be visible, readable and understandable, helping the user identify what needs attention.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If no actions are available, the application should display a clear empty state.

---

## TC-DASH-005 — Recent activities section is visible and readable

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-005 |
| Module | Dashboard / Control Tower |
| Type | Functional / Usability |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard page is loaded.

### Steps

1. Access the dashboard.
2. Locate the recent activities section.
3. Verify if the section title is visible.
4. Verify if activity items are readable.
5. Verify if dates, descriptions or statuses are understandable, when available.

### Expected Result

The recent activities section should display readable and useful information about recent operational events.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If there are no recent activities, a clear empty state should be displayed.

---

## TC-DASH-006 — Dashboard navigation links or shortcuts work correctly

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-006 |
| Module | Dashboard / Control Tower |
| Type | Functional / Navigation |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard page is loaded.

### Steps

1. Access the dashboard.
2. Identify available navigation links, buttons or shortcuts.
3. Click a shortcut to a related module, such as clients, quotes, financial area or NFSe.
4. Observe the result.

### Expected Result

The selected shortcut should navigate the user to the correct destination without errors.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Each important dashboard shortcut may generate a separate bug report if it fails.

---

## TC-DASH-007 — Dashboard does not expose broken or duplicated information

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-007 |
| Module | Dashboard / Control Tower |
| Type | Functional / Visual |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard page is loaded.

### Steps

1. Access the dashboard.
2. Review the visible dashboard sections.
3. Check for duplicated cards, duplicated labels or repeated items.
4. Check for broken text, missing values or placeholder content.
5. Check if any section appears visually incomplete.

### Expected Result

The dashboard should not display duplicated, broken, missing or placeholder information unless intentionally designed.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test is useful for identifying polish and data presentation issues.

---

## TC-DASH-008 — Dashboard empty states are clear when no data is available

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-008 |
| Module | Dashboard / Control Tower |
| Type | Functional / Empty State |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard has one or more sections without available data.

### Steps

1. Access the dashboard.
2. Locate sections that have no available records or activities.
3. Verify if an empty state message is displayed.
4. Check if the message explains the situation clearly.
5. Check if the user receives guidance for what to do next, when applicable.

### Expected Result

Empty states should be clear, helpful and should not look like system errors.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the current test environment always contains data, this test can be marked as Blocked or Not Applicable during execution.

---

## TC-DASH-009 — Dashboard remains usable after page refresh

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-009 |
| Module | Dashboard / Control Tower |
| Type | Functional / Session |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard page is loaded.

### Steps

1. Access the dashboard.
2. Refresh the browser page.
3. Wait for the page to reload.
4. Observe the dashboard behavior.

### Expected Result

The dashboard should reload correctly and remain usable after refresh, as long as the user session is still valid.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the session expires after refresh by design, this behavior should be documented.

---

## TC-DASH-010 — Dashboard is readable on desktop viewport

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-010 |
| Module | Dashboard / Control Tower |
| Type | Responsive / Visual |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard page is loaded.
- The browser is using a desktop viewport.

### Steps

1. Access the dashboard using a desktop viewport.
2. Verify if summary cards are aligned correctly.
3. Verify if text is readable.
4. Verify if sections have proper spacing.
5. Verify if navigation remains visible and usable.

### Expected Result

The dashboard should be readable, organized and usable on desktop viewport.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test supports basic responsive validation.

---

## TC-DASH-011 — Dashboard is usable on mobile-like viewport

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-011 |
| Module | Dashboard / Control Tower |
| Type | Responsive / Usability |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard page is loaded.
- The browser viewport is resized to a mobile-like width.

### Steps

1. Access the dashboard.
2. Resize the browser to a mobile-like viewport or use DevTools device mode.
3. Verify if the main content remains readable.
4. Verify if cards stack properly.
5. Verify if navigation remains accessible.
6. Check for horizontal scrolling or content overflow.

### Expected Result

The dashboard should remain usable on a mobile-like viewport, without broken layout or unreadable content.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Any layout issue should be documented with screenshot evidence.

---

## TC-DASH-012 — Dashboard visual hierarchy is clear

| Field | Information |
|---|---|
| Test Case ID | TC-DASH-012 |
| Module | Dashboard / Control Tower |
| Type | Usability / Visual |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The dashboard page is loaded.

### Steps

1. Access the dashboard.
2. Observe the page title, section titles and cards.
3. Verify if important information is visually emphasized.
4. Verify if secondary information does not compete with critical information.
5. Check if the user can quickly understand the dashboard purpose.

### Expected Result

The dashboard should have a clear visual hierarchy, making important operational information easy to identify.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test helps evaluate the dashboard from a real user's perspective.

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
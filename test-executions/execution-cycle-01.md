# Test Execution Cycle 01 — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Document Type | Manual Test Execution Cycle |
| Execution Cycle | Cycle 01 |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | In Progress|

---

## 2. Objective

The objective of this document is to record the official execution of the first manual QA cycle for the Firmus application.

This execution cycle will validate the main user-facing flows documented in the manual test case files, including authentication, dashboard, clients, quotes, financial overview and NFSe foundation.

The goal is to document what was tested, what passed, what failed, what was blocked, which bugs were found and what evidence was collected.

---

## 3. Execution Scope

This execution cycle includes the following areas:

- Authentication
- Protected routes
- Dashboard / Control Tower
- Clients
- Quotes
- Financial overview
- NFSe foundation
- Basic responsive behavior
- Basic usability observations

This cycle is based on the test cases documented in:

```txt
test-cases/authentication-test-cases.md
test-cases/dashboard-test-cases.md
test-cases/clients-test-cases.md
test-cases/quotes-test-cases.md
test-cases/financial-test-cases.md
test-cases/nfse-test-cases.md
```

---

## 4. Out of Scope

The following items are not part of this execution cycle:

- Automated test execution
- API testing
- Load testing
- Stress testing
- Deep security testing
- Accessibility audit with specialized tools
- Database validation
- Backend code review
- Real NFSe provider validation
- Production monitoring

---

## 5. Execution Environment

| Field | Information |
|---|---|
| Execution Date | 2026-04-24|
| Environment | Local development |
| Application URL | http://localhost:3000  |
| Browser | Google Chrome / Chromium-based browser |
| Operating System | Ubuntu Linux |
| Device | Desktop / Notebook |
| Viewports Used | Desktop and mobile-like viewport |
| Executed by | Ademir dos Santos Junior |

---

## 6. Status Legend

| Status | Meaning |
|---|---|
| Passed | The actual result matches the expected result |
| Failed | The actual result does not match the expected result |
| Blocked | The test could not be executed due to a blocker or dependency |
| Not Applicable | The test does not apply to the current version of the application |
| Not Executed | The test has not been executed yet |

---

## 7. Pre-Execution Checklist

Before starting the execution cycle, confirm the following items:

| ID | Checkpoint | Status | Notes |
|---|---|---|---|
| PRE-001 | Firmus application is running locally | Passed | Application running locally |
| PRE-002 | Browser is available and updated | Passed | Google Chrome available |
| PRE-003 | Tester can access the application URL | Passed | Application URL opened successfully |
| PRE-004 | Valid test credentials are available | Passed | Test credentials available |
| PRE-005 | Test data is available or can be created | Passed | Local test data available or can be created |
| PRE-006 | Evidence folders are available | Passed | evidences/screenshots and evidences/videos folders available |
| PRE-007 | Bug report template is available | Passed | Template available in bug-reports folder |
| PRE-008 | Test cases are ready for execution | Passed | Test case files available in test-cases folder |
---

## 8. Execution Summary

| Status | Total |
|---|---:|
| Passed | 24 |
| Failed | 0 |
| Blocked | 0 |
| Not Applicable | 0 |
| Not Executed | 54 |

---


## 9. Module Summary

| Module | Total Test Cases | Passed | Failed | Blocked | Not Applicable | Not Executed |
|---|---:|---:|---:|---:|---:|---:|
| Authentication | 12 | 12 | 0 | 0 | 0 | 0 |
| Dashboard / Control Tower | 12 | 12 | 0 | 0 | 0 | 0 |
| Clients | 12 | 0 | 0 | 0 | 0 | 12 |
| Quotes | 14 | 0 | 0 | 0 | 0 | 14 |
| Financial Overview | 14 | 0 | 0 | 0 | 0 | 14 |
| NFSe Foundation | 14 | 0 | 0 | 0 | 0 | 14 |
| Total | 78 | 24 | 0 | 0 | 0 | 54 |
---

## 10. Detailed Test Execution

### 10.1 Authentication

### 10.1 Authentication

| Test Case ID | Test Case Title | Status | Actual Result | Evidence | Bug ID | Notes |
|---|---|---|---|---|---|---|
| TC-AUTH-001 | Login with valid credentials | Passed | Login worked successfully and the user was redirected to the dashboard. | evidences/screenshots/TC-AUTH-001-login-success.png | - | Critical login flow worked as expected. |
| TC-AUTH-002 | Login with invalid email | Passed | Invalid credentials were rejected by the system. | - | - | Authentication validation worked as expected. |
| TC-AUTH-003 | Login with invalid password | Passed | Invalid password was rejected by the system. | - | - | User remained unauthenticated. |
| TC-AUTH-004 | Login with empty email field | Passed | Login was blocked when the email field was empty. | - | - | Required field validation worked as expected. |
| TC-AUTH-005 | Login with empty password field | Passed | Login was blocked when the password field was empty. | - | - | Required field validation worked as expected. |
| TC-AUTH-006 | Login with both fields empty | Passed | Login was blocked when both fields were empty. | - | - | Required field validation worked as expected. |
| TC-AUTH-007 | Access protected route without authentication | Passed | Protected route access was blocked and the user was redirected. | - | - | Route protection worked as expected. |
| TC-AUTH-008 | Access protected route after login | Passed | Protected route was accessible after successful login. | - | - | Authenticated access worked as expected. |
| TC-AUTH-009 | Logout from authenticated session | Passed | Logout worked successfully. | - | - | User session was ended as expected. |
| TC-AUTH-010 | Access protected route after logout | Passed | Protected route access was blocked after logout. | - | - | Post-logout route protection worked as expected. |
| TC-AUTH-011 | Refresh page while authenticated | Passed | Page refresh preserved the authenticated session. | - | - | Session behavior worked as expected. |
| TC-AUTH-012 | Login page visual and usability validation | Passed | Login page was clear, readable and usable. | - | - | Login UI passed basic usability validation. |

---

### 10.2 Dashboard / Control Tower

| Test Case ID | Test Case Title | Status | Actual Result | Evidence | Bug ID | Notes |
|---|---|---|---|---|---|---|
| TC-DASH-001 | Dashboard loads after successful login | Passed | Dashboard loaded successfully after login. | | - | Main dashboard entry point worked as expected. |
| TC-DASH-002 | Dashboard main sections are visible | Passed | Main dashboard sections were visible. | - | - | Dashboard structure was displayed correctly. |
| TC-DASH-003 | Operational summary cards are displayed correctly | Passed | Operational summary cards were displayed correctly. | - | - | Summary cards were readable and organized. |
| TC-DASH-004 | Next actions section is visible and understandable | Passed | Next actions section was visible and understandable. | - | - | Action labels and statuses were clear. |
| TC-DASH-005 | Recent activities section is visible and readable | Passed | Recent activities section was visible and readable. | - | - | Activity information was clear. |
| TC-DASH-006 | Dashboard navigation links or shortcuts work correctly | Passed | Dashboard navigation links and shortcuts worked correctly. | - | - | Navigation from dashboard behaved as expected. |
| TC-DASH-007 | Dashboard does not expose broken or duplicated information | Passed | No broken or duplicated dashboard information was observed. | - | - | Dashboard content looked consistent. |
| TC-DASH-008 | Dashboard empty states are clear when no data is available | Passed | Dashboard empty states were clear when applicable. | - | - | Empty-state behavior was acceptable in the current environment. |
| TC-DASH-009 | Dashboard remains usable after page refresh | Passed | Dashboard remained usable after page refresh. | - | - | Refresh behavior worked as expected. |
| TC-DASH-010 | Dashboard is readable on desktop viewport | Passed | Dashboard was readable and organized on desktop viewport. | - | - | Desktop layout passed validation. |
| TC-DASH-011 | Dashboard is usable on mobile-like viewport | Passed | Dashboard remained usable on mobile-like viewport. | - | - | Mobile-like layout passed validation. |
| TC-DASH-012 | Dashboard visual hierarchy is clear | Passed | Dashboard visual hierarchy was clear. | - | - | Important operational information was easy to identify. |
---

### 10.3 Clients

| Test Case ID | Test Case Title | Status | Actual Result | Evidence | Bug ID | Notes |
|---|---|---|---|---|---|---|
| TC-CLI-001 | Clients page loads successfully | Not Executed |  |  |  |  |
| TC-CLI-002 | Clients list is visible when records exist | Not Executed |  |  |  |  |
| TC-CLI-003 | Clients empty state is clear when no records exist | Not Executed |  |  |  |  |
| TC-CLI-004 | Create client action is visible when available | Not Executed |  |  |  |  |
| TC-CLI-005 | Create client with valid required information | Not Executed |  |  |  |  |
| TC-CLI-006 | Create client with required fields empty | Not Executed |  |  |  |  |
| TC-CLI-007 | Create client with invalid contact information | Not Executed |  |  |  |  |
| TC-CLI-008 | Client details are visible when opening a client record | Not Executed |  |  |  |  |
| TC-CLI-009 | Client-related navigation works correctly | Not Executed |  |  |  |  |
| TC-CLI-010 | Clients page does not display broken or placeholder information | Not Executed |  |  |  |  |
| TC-CLI-011 | Clients page remains usable after refresh | Not Executed |  |  |  |  |
| TC-CLI-012 | Clients page is usable on mobile-like viewport | Not Executed |  |  |  |  |

---

### 10.4 Quotes

| Test Case ID | Test Case Title | Status | Actual Result | Evidence | Bug ID | Notes |
|---|---|---|---|---|---|---|
| TC-QUO-001 | Quotes page loads successfully | Not Executed |  |  |  |  |
| TC-QUO-002 | Quotes list is visible when records exist | Not Executed |  |  |  |  |
| TC-QUO-003 | Quotes empty state is clear when no records exist | Not Executed |  |  |  |  |
| TC-QUO-004 | Create quote action is visible when available | Not Executed |  |  |  |  |
| TC-QUO-005 | Create quote with valid required information | Not Executed |  |  |  |  |
| TC-QUO-006 | Create quote with required fields empty | Not Executed |  |  |  |  |
| TC-QUO-007 | Create quote with invalid monetary value | Not Executed |  |  |  |  |
| TC-QUO-008 | Quote status is visible and understandable | Not Executed |  |  |  |  |
| TC-QUO-009 | Quote details are visible when opening a quote record | Not Executed |  |  |  |  |
| TC-QUO-010 | Public quote access works when available | Not Executed |  |  |  |  |
| TC-QUO-011 | Quote-related navigation works correctly | Not Executed |  |  |  |  |
| TC-QUO-012 | Quotes page does not display broken or placeholder information | Not Executed |  |  |  |  |
| TC-QUO-013 | Quotes page remains usable after refresh | Not Executed |  |  |  |  |
| TC-QUO-014 | Quotes page is usable on mobile-like viewport | Not Executed |  |  |  |  |

---

### 10.5 Financial Overview

| Test Case ID | Test Case Title | Status | Actual Result | Evidence | Bug ID | Notes |
|---|---|---|---|---|---|---|
| TC-FIN-001 | Financial page loads successfully | Not Executed |  |  |  |  |
| TC-FIN-002 | Financial summary cards are visible | Not Executed |  |  |  |  |
| TC-FIN-003 | Monetary values are formatted correctly | Not Executed |  |  |  |  |
| TC-FIN-004 | Financial records are visible when records exist | Not Executed |  |  |  |  |
| TC-FIN-005 | Financial empty state is clear when no records exist | Not Executed |  |  |  |  |
| TC-FIN-006 | Financial status indicators are visible and understandable | Not Executed |  |  |  |  |
| TC-FIN-007 | Financial page does not display negative or inconsistent values unexpectedly | Not Executed |  |  |  |  |
| TC-FIN-008 | Financial filters work when available | Not Executed |  |  |  |  |
| TC-FIN-009 | Financial-related navigation works correctly | Not Executed |  |  |  |  |
| TC-FIN-010 | Financial page does not display broken or placeholder information | Not Executed |  |  |  |  |
| TC-FIN-011 | Financial page remains usable after refresh | Not Executed |  |  |  |  |
| TC-FIN-012 | Financial page is readable on desktop viewport | Not Executed |  |  |  |  |
| TC-FIN-013 | Financial page is usable on mobile-like viewport | Not Executed |  |  |  |  |
| TC-FIN-014 | Financial information is understandable for the user | Not Executed |  |  |  |  |

---

### 10.6 NFSe Foundation

| Test Case ID | Test Case Title | Status | Actual Result | Evidence | Bug ID | Notes |
|---|---|---|---|---|---|---|
| TC-NFSE-001 | NFSe page loads successfully | Not Executed |  |  |  |  |
| TC-NFSE-002 | NFSe records are visible when records exist | Not Executed |  |  |  |  |
| TC-NFSE-003 | NFSe empty state is clear when no records exist | Not Executed |  |  |  |  |
| TC-NFSE-004 | NFSe fiscal status is visible and understandable | Not Executed |  |  |  |  |
| TC-NFSE-005 | Provider reference is displayed when available | Not Executed |  |  |  |  |
| TC-NFSE-006 | Document number is displayed when available | Not Executed |  |  |  |  |
| TC-NFSE-007 | NFSe issue date or emitted date is displayed when available | Not Executed |  |  |  |  |
| TC-NFSE-008 | NFSe record information is not duplicated inside the same card | Not Executed |  |  |  |  |
| TC-NFSE-009 | NFSe page does not display placeholder or broken information | Not Executed |  |  |  |  |
| TC-NFSE-010 | NFSe-related navigation works correctly | Not Executed |  |  |  |  |
| TC-NFSE-011 | NFSe page remains usable after refresh | Not Executed |  |  |  |  |
| TC-NFSE-012 | NFSe page is readable on desktop viewport | Not Executed |  |  |  |  |
| TC-NFSE-013 | NFSe page is usable on mobile-like viewport | Not Executed |  |  |  |  |
| TC-NFSE-014 | NFSe information is understandable for the user | Not Executed |  |  |  |  |

---

## 11. Bugs Found During Execution

| Bug ID | Title | Module | Severity | Priority | Status | Evidence |
|---|---|---|---|---|---|---|
| - | - | - | - | - | - | - |

---

## 12. Evidence Collected

| Evidence ID | Related Test Case | Related Bug ID | Evidence Type | File Path | Notes |
|---|---|---|---|---|---|
| EVD-001 | TC-AUTH-001 | - | Screenshot | evidences/screenshots/TC-AUTH-001-login-success.png | Successful login redirected the user to the dashboard. |

Evidence should be stored in:

```txt
evidences/screenshots/
evidences/videos/
```

---

## 13. General Execution Notes

Use this section to document relevant observations from the execution cycle.

Examples:

- Environment instability
- Missing test data
- Features not available in the current application version
- Behaviors that need product clarification
- Usability concerns that are not necessarily bugs
- Any limitation found during manual execution

Notes:

```txt
To be filled during execution.
```

---

## 14. Execution Result

| Field | Result |
|---|---|
| Execution Started | Yes |
| Execution Completed | No |
| Critical Bugs Found | 0 |
| High Bugs Found | 0 |
| Medium Bugs Found | 0 |
| Low Bugs Found | 0 |
| Overall Result | In progress |

---

## 15. Go / No-Go Assessment

| Decision | Meaning |
|---|---|
| Go | The application is stable enough based on this test cycle |
| Go with Known Issues | The application can proceed, but documented issues remain |
| No-Go | Critical or high-risk issues block approval |
| Not Evaluated | Execution has not been completed yet |

Current decision:

```txt
Not Evaluated
```

---

## 16. Exit Criteria

This execution cycle can be considered complete when:

- Pre-execution checklist has been reviewed.
- Planned test cases have been executed or properly marked.
- Each test case has a status.
- Failed tests have clear notes.
- Bugs have been documented when applicable.
- Evidence has been collected when useful.
- Execution summary has been updated.
- Overall result has been defined.

---

## 17. Approval Criteria

This execution cycle document is considered ready when:

- Execution environment is documented.
- Status legend is available.
- Pre-execution checklist is included.
- Test cases are listed by module.
- Bug tracking section is included.
- Evidence tracking section is included.
- Execution result section is included.
- Go / No-Go assessment is included.
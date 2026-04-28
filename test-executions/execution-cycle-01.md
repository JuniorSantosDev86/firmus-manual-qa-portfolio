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
| Passed | 72 |
| Failed | 5 |
| Blocked | 0 |
| Not Applicable | 1 |
| Not Executed | 0 |
---


## 9. Module Summary

| Module | Total Test Cases | Passed | Failed | Blocked | Not Applicable | Not Executed |
|---|---:|---:|---:|---:|---:|---:|
| Authentication | 12 | 12 | 0 | 0 | 0 | 0 |
| Dashboard / Control Tower | 12 | 12 | 0 | 0 | 0 | 0 |
| Clients | 12 | 10 | 2 | 0 | 0 | 0 |
| Quotes | 14 | 11 | 3 | 0 | 0 | 0 |
| Financial Overview | 14 | 13 | 0 | 0 | 1 | 0 |
| NFSe Foundation | 14 | 14 | 0 | 0 | 0 | 0 |
| Total | 78 | 72 | 5 | 0 | 1 | 0 |

---

## 10. Detailed Test Execution

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
| TC-CLI-001 | Clients page loads successfully | Passed | Clients page loaded successfully. |  | - | Clients module was accessible and usable. |
| TC-CLI-002 | Clients list is visible when records exist | Passed | Existing clients were displayed correctly. | - | - | Client list was visible and readable. |
| TC-CLI-003 | Clients empty state is clear when no records exist | Passed | Empty state behavior was validated successfully when applicable. | - | - | Empty state did not appear broken. |
| TC-CLI-004 | Create client action is visible when available | Passed | Create client action was visible and accessible. | - | - | User could access the client creation flow. |
| TC-CLI-005 | Create client with valid required information | Passed | Client was created successfully with valid information. | - | - | Valid client creation worked as expected. |
| TC-CLI-006 | Create client with required fields empty | Failed | The system allowed client creation with only the client name filled and no other required data. | evidences/screenshots/BUG-001-client-created-with-only-name.png | BUG-001 | Required field validation did not prevent incomplete client creation. |
| TC-CLI-007 | Create client with invalid contact information | Failed | The system allowed client creation without contact information or with invalid contact information. | evidences/screenshots/BUG-002-client-invalid-contact-accepted.png | BUG-002 | Contact information validation did not work as expected. |
| TC-CLI-008 | Client details are visible when opening a client record | Passed | Client details were visible when opening a client record. | - | - | Client information was readable. |
| TC-CLI-009 | Client-related navigation works correctly | Passed | Client-related navigation worked correctly. | - | - | No broken navigation was observed in the tested flow. |
| TC-CLI-010 | Clients page does not display broken or placeholder information | Passed | No broken or placeholder information was observed. | - | - | Clients page looked consistent. |
| TC-CLI-011 | Clients page remains usable after refresh | Passed | Clients page remained usable after refresh. | - | - | Refresh behavior worked as expected. |
| TC-CLI-012 | Clients page is usable on mobile-like viewport | Passed | Clients page remained usable on mobile-like viewport. | - | - | Mobile-like layout passed validation. |

---

### 10.4 Quotes

| Test Case ID | Test Case Title | Status | Actual Result | Evidence | Bug ID | Notes |
|---|---|---|---|---|---|---|
| TC-QUO-001 | Quotes page loads successfully | Passed | Quotes page loaded successfully. | - | - | Quotes module was accessible and usable. |
| TC-QUO-002 | Quotes list is visible when records exist | Passed | Existing quotes were displayed correctly. | - | - | Quotes list was visible and readable. |
| TC-QUO-003 | Quotes empty state is clear when no records exist | Passed | Empty state behavior was validated successfully when applicable. | - | - | Empty state did not appear broken. |
| TC-QUO-004 | Create quote action is visible when available | Passed | Create quote action was visible and accessible. | - | - | User could access the quote creation flow. |
| TC-QUO-005 | Create quote with valid required information | Passed | Quote was created successfully with valid information. | - | - | Valid quote creation worked as expected. |
| TC-QUO-006 | Create quote with required fields empty | Failed | The system allowed quote creation with empty fields or invalid/random data. | evidences/screenshots/BUG-004-quote-created-with-empty-or-invalid-fields.png | BUG-004 | Required field validation did not prevent invalid quote creation. |
| TC-QUO-007 | Create quote with invalid monetary value | Failed | The system allowed quote creation with text in the monetary value field. | evidences/screenshots/BUG-005-quote-value-accepts-text.png | BUG-005 | Monetary value validation did not work as expected. |
| TC-QUO-008 | Quote status is visible and understandable | Passed | Quote status was visible and understandable. | - | - | Status information was clear. |
| TC-QUO-009 | Quote details are visible when opening a quote record | Passed | Quote details were visible when opening a quote record. | - | - | Quote information was readable. |
| TC-QUO-010 | Public quote access works when available | Passed | Public quote access worked when available. | - | - | Public quote flow behaved as expected in the tested scenario. |
| TC-QUO-011 | Quote-related navigation works correctly | Passed | Quote-related navigation worked correctly. | - | - | No broken navigation was observed in the tested flow. |
| TC-QUO-012 | Quotes page does not display broken or placeholder information | Passed | No broken or placeholder information was observed. | - | - | Quotes page looked consistent. |
| TC-QUO-013 | Quotes page remains usable after refresh | Passed | Quotes page remained usable after refresh. | - | - | Refresh behavior worked as expected. |
| TC-QUO-014 | Quotes page is usable on mobile-like viewport | Failed | A box overflowed or broke the layout in the mobile-like viewport. | evidences/screenshots/BUG-006-quote-mobile-layout-overflow.png | BUG-006 | Mobile-like layout did not remain fully usable. |

---

### 10.5 Financial Overview

| Test Case ID | Test Case Title | Status | Actual Result | Evidence | Bug ID | Notes |
|---|---|---|---|---|---|---|
| TC-FIN-001 | Financial page loads successfully | Passed | Financial page loaded successfully. | - | - | Financial module was accessible and usable. |
| TC-FIN-002 | Financial summary cards are visible | Passed | Financial summary cards were visible. | - | - | The financial view displayed the expected summary cards. |
| TC-FIN-003 | Monetary values are formatted correctly | Passed | Monetary values were displayed in a clear and readable format. | - | - | Currency information was understandable. |
| TC-FIN-004 | Financial records are visible when records exist | Passed | Financial information was visible in the current environment. | - | - | Available financial information was displayed correctly. |
| TC-FIN-005 | Financial empty state is clear when no records exist | Passed | Empty state behavior was clear when applicable. | - | - | The page did not look broken or incomplete. |
| TC-FIN-006 | Financial status indicators are visible and understandable | Passed | Financial indicators were visible and understandable. | - | - | Status and summary information were clear. |
| TC-FIN-007 | Financial page does not display negative or inconsistent values unexpectedly | Passed | No unexpected negative, missing, duplicated or inconsistent values were observed. | - | - | Financial values looked consistent with their labels. |
| TC-FIN-008 | Financial filters work when available | Not Applicable | Financial filters are not available in the current simple financial view. | - | - | The current version displays only summary cards, so there were no filters to validate. |
| TC-FIN-009 | Financial-related navigation works correctly | Passed | Financial-related navigation worked correctly. | - | - | No broken navigation was observed. |
| TC-FIN-010 | Financial page does not display broken or placeholder information | Passed | No broken or placeholder information was observed. | - | - | Financial page looked consistent. |
| TC-FIN-011 | Financial page remains usable after refresh | Passed | Financial page remained usable after refresh. | - | - | Refresh behavior worked as expected. |
| TC-FIN-012 | Financial page is readable on desktop viewport | Passed | Financial page was readable and organized on desktop viewport. | - | - | Desktop layout passed validation. |
| TC-FIN-013 | Financial page is usable on mobile-like viewport | Passed | Financial page remained usable on mobile-like viewport. | - | - | No blocking responsive issue was observed. |
| TC-FIN-014 | Financial information is understandable for the user | Passed | Financial information was clear and understandable for the user. | - | - | The financial view provided useful business visibility. |

---

### 10.6 NFSe Foundation

| Test Case ID | Test Case Title | Status | Actual Result | Evidence | Bug ID | Notes |
|---|---|---|---|---|---|---|
| TC-NFSE-001 | NFSe page loads successfully | Passed | NFSe page loaded successfully. | - | - | NFSe module was accessible and usable. |
| TC-NFSE-002 | NFSe records are visible when records exist | Passed | NFSe records were visible when records existed. | - | - | Records were displayed correctly. |
| TC-NFSE-003 | NFSe empty state is clear when no records exist | Passed | Empty state behavior was clear when applicable. | - | - | Empty state did not look broken. |
| TC-NFSE-004 | NFSe fiscal status is visible and understandable | Passed | Fiscal status information was visible and understandable. | - | - | Status labels were clear. |
| TC-NFSE-005 | Provider reference is displayed when available | Passed | Provider reference was displayed when available. | - | - | Provider reference information appeared correctly. |
| TC-NFSE-006 | Document number is displayed when available | Passed | Document number was displayed when available. | - | - | Document number information appeared correctly. |
| TC-NFSE-007 | NFSe issue date or emitted date is displayed when available | Passed | NFSe issue/emitted date was displayed when available. | - | - | Date information was readable. |
| TC-NFSE-008 | NFSe record information is not duplicated inside the same card | Passed | No duplicated NFSe information was observed inside the same card. | - | - | Previous duplication risk was not observed. |
| TC-NFSE-009 | NFSe page does not display placeholder or broken information | Passed | No placeholder or broken information was observed. | - | - | NFSe page looked consistent. |
| TC-NFSE-010 | NFSe-related navigation works correctly | Passed | NFSe-related navigation worked correctly. | - | - | No broken navigation was observed. |
| TC-NFSE-011 | NFSe page remains usable after refresh | Passed | NFSe page remained usable after refresh. | - | - | Refresh behavior worked as expected. |
| TC-NFSE-012 | NFSe page is readable on desktop viewport | Passed | NFSe page was readable and organized on desktop viewport. | - | - | Desktop layout passed validation. |
| TC-NFSE-013 | NFSe page is usable on mobile-like viewport | Passed | NFSe page remained usable on mobile-like viewport. | - | - | Mobile-like layout passed validation. |
| TC-NFSE-014 | NFSe information is understandable for the user | Passed | NFSe information was clear and understandable for the user. | - | - | The page communicated fiscal information clearly. |

---

## 11. Bugs Found During Execution

| Bug ID | Title | Module | Severity | Priority | Status | Evidence |
|---|---|---|---|---|---|---|
| BUG-001 | Client can be created with only the name field filled | Clients | Medium | Medium | Open | evidences/screenshots/BUG-001-client-created-with-only-name.png |
| BUG-002 | Client can be created without valid contact information | Clients | Medium | Medium | Open | evidences/screenshots/BUG-002-client-invalid-contact-accepted.png |
| BUG-003 | Delete client action does not remove the client after confirmation | Clients | High | High | Open | evidences/screenshots/BUG-003-delete-client-not-working.png |
| BUG-004 | Quote can be created with empty or invalid required fields | Quotes | Medium | Medium | Open | evidences/screenshots/BUG-004-quote-created-with-empty-or-invalid-fields.png |
| BUG-005 | Quote value field accepts text instead of numeric value | Quotes | Medium | Medium | Open | evidences/screenshots/BUG-005-quote-value-accepts-text.png |
| BUG-006 | Quote layout breaks on mobile-like viewport | Quotes | Medium | Medium | Open | evidences/screenshots/BUG-006-quote-mobile-layout-overflow.png |

---

## 12. Evidence Collected

| Evidence ID | Related Test Case | Related Bug ID | Evidence Type | File Path | Notes |
|---|---|---|---|---|---|
| EVD-001 | TC-AUTH-001 | - | Screenshot | evidences/screenshots/TC-AUTH-001-login-success.png | Successful login redirected the user to the dashboard. |
| EVD-002 | TC-CLI-006 | BUG-001 | Screenshot | evidences/screenshots/BUG-001-client-created-with-only-name.png | Client was created with only the name field filled. |
| EVD-003 | TC-CLI-007 | BUG-002 | Screenshot | evidences/screenshots/BUG-002-client-invalid-contact-accepted.png | Client was created without valid contact information or with invalid contact information. |
| EVD-004 | Exploratory finding | BUG-003 | Screenshot | evidences/screenshots/BUG-003-delete-client-not-working.png | Delete client confirmation did not remove the client. |
| EVD-005 | TC-QUO-006 | BUG-004 | Screenshot | evidences/screenshots/BUG-004-quote-created-with-empty-or-invalid-fields.png | Quote was created with empty or invalid required fields. |
| EVD-006 | TC-QUO-007 | BUG-005 | Screenshot | evidences/screenshots/BUG-005-quote-value-accepts-text.png | Quote value field accepted text instead of a numeric value. |
| EVD-007 | TC-QUO-014 | BUG-006 | Screenshot | evidences/screenshots/BUG-006-quote-mobile-layout-overflow.png | Quote layout overflowed or broke in mobile-like viewport. |

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
| Execution Completed | Yes |
| Critical Bugs Found | 0 |
| High Bugs Found | 1 |
| Medium Bugs Found | 5 |
| Low Bugs Found | 0 |
| Overall Result | Completed with known issues |

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
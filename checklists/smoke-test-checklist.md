# Smoke Test Checklist — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Document Type | Smoke Test Checklist |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | Ready for execution |

---

## 2. Objective

The objective of this smoke test checklist is to quickly validate whether the most critical flows of the Firmus application are working before starting a deeper manual QA execution cycle.

Smoke testing helps identify major blockers early and confirms whether the application is stable enough for functional, regression, exploratory and responsive testing.

---

## 3. Smoke Test Scope

This checklist covers the most critical user-facing areas of the Firmus application:

- Application loading
- Login
- Protected routes
- Dashboard / Control Tower
- Main navigation
- Clients
- Quotes
- Financial overview
- NFSe foundation
- Logout
- Basic responsive access

This smoke test does not replace detailed functional testing. It only validates if the main flows are available and usable at a basic level.

---

## 4. Execution Information

| Field | Information |
|---|---|
| Execution Date | YYYY-MM-DD |
| Environment | Local development |
| Browser | Google Chrome / Chromium-based browser |
| Operating System | Ubuntu Linux |
| Executed by | Ademir dos Santos Junior |

---

## 5. Status Legend

| Status | Meaning |
|---|---|
| Passed | The item worked as expected |
| Failed | The item did not work as expected |
| Blocked | The item could not be tested due to a blocker |
| Not Applicable | The item does not apply to the current application version |
| Not Executed | The item has not been executed yet |

---

## 6. Smoke Test Checklist

| ID | Area | Checkpoint | Expected Result | Status | Notes |
|---|---|---|---|---|---|
| SMK-001 | Application | Open the Firmus application | The application should load without critical errors | Not Executed |  |
| SMK-002 | Authentication | Access the login page | The login page should be visible and usable | Not Executed |  |
| SMK-003 | Authentication | Log in with valid credentials | The user should be authenticated successfully | Not Executed |  |
| SMK-004 | Authentication | Access protected area after login | The authenticated user should access private areas | Not Executed |  |
| SMK-005 | Protected Routes | Try to access a protected route while logged out | The system should prevent access and redirect the user | Not Executed |  |
| SMK-006 | Dashboard | Load the Dashboard / Control Tower | The dashboard should load after login | Not Executed |  |
| SMK-007 | Dashboard | Verify dashboard main sections | Main sections should be visible and readable | Not Executed |  |
| SMK-008 | Navigation | Use the main navigation menu | Navigation should work without broken routes | Not Executed |  |
| SMK-009 | Clients | Access the clients area | The clients page should load successfully | Not Executed |  |
| SMK-010 | Quotes | Access the quotes area | The quotes page should load successfully | Not Executed |  |
| SMK-011 | Financial | Access the financial area | The financial page should load successfully | Not Executed |  |
| SMK-012 | NFSe | Access the NFSe area | The NFSe page should load successfully | Not Executed |  |
| SMK-013 | UI | Check for critical broken layout | The application should not show critical layout breaks | Not Executed |  |
| SMK-014 | Session | Refresh a protected page while authenticated | The page should remain usable if the session is valid | Not Executed |  |
| SMK-015 | Logout | Log out from the application | The user should be logged out successfully | Not Executed |  |
| SMK-016 | Post-Logout Access | Try to access a protected route after logout | The system should prevent access to protected areas | Not Executed |  |
| SMK-017 | Responsive | Open the application in a mobile-like viewport | Main navigation and content should remain usable | Not Executed |  |

---

## 7. Smoke Test Exit Criteria

The smoke test can be considered passed when:

- The application loads successfully.
- The user can log in.
- Protected routes behave correctly.
- The dashboard loads.
- Main navigation works.
- Core modules are accessible.
- The user can log out.
- No critical blocker prevents deeper testing.

If one or more critical items fail, the full manual execution cycle should not start until the blocker is documented and resolved or accepted as a known limitation.

---

## 8. Critical Smoke Failures

The following failures should be treated as major blockers:

- Application does not load.
- Login does not work with valid credentials.
- Dashboard does not load after login.
- Main navigation is broken.
- Protected routes are exposed to unauthenticated users.
- Logout does not work.
- Multiple core modules are inaccessible.
- The application crashes during basic navigation.

Any critical smoke failure should generate a bug report.

---

## 9. Execution Summary

| Status | Total |
|---|---:|
| Passed | 0 |
| Failed | 0 |
| Blocked | 0 |
| Not Applicable | 0 |
| Not Executed | 17 |

---

## 10. Notes for Execution

During execution, update each checklist item with:

- Status
- Notes
- Evidence, when applicable

If an item fails, create a bug report using:

```txt
bug-reports/bug-report-template.md


Evidence should be stored in:
evidences/screenshots/
evidences/videos/



Evidence should be stored in:
evidences/screenshots/
evidences/videos/

## 11. Approval Criteria

This smoke test checklist is considered ready when:

- Critical flows are listed.
- Expected results are clear.
- Status options are defined.
- The checklist supports a quick go/no-go decision before deeper testing.
- The checklist can be reused in future regression cycles.
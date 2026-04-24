# Regression Test Checklist — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Document Type | Regression Test Checklist |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | Ready for execution |

---

## 2. Objective

The objective of this regression test checklist is to verify that previously working features in the Firmus application continue to work correctly after changes, fixes, improvements or new implementations.

Regression testing helps reduce the risk of new changes breaking existing behavior.

This checklist supports repeated validation of the main user-facing flows in the application.

---

## 3. Regression Test Scope

This checklist covers the main areas of the Firmus application that should be revalidated after relevant changes:

- Authentication
- Protected routes
- Dashboard / Control Tower
- Main navigation
- Clients
- Quotes
- Financial overview
- NFSe foundation
- Session behavior
- Responsive behavior
- Basic usability

This checklist does not replace detailed test cases. It works as a practical regression validation guide.

---

## 4. When to Execute Regression Testing

Regression testing should be executed when:

- A bug fix is implemented.
- A new feature is added.
- Existing UI behavior changes.
- Navigation changes.
- Authentication or session behavior changes.
- A core module is refactored.
- A release candidate needs validation.
- The application is being prepared for portfolio demonstration.

---

## 5. Execution Information

| Field | Information |
|---|---|
| Execution Date | YYYY-MM-DD |
| Environment | Local development |
| Browser | Google Chrome / Chromium-based browser |
| Operating System | Ubuntu Linux |
| Executed by | Ademir dos Santos Junior |
| Related Change / Fix | To be filled during execution |

---

## 6. Status Legend

| Status | Meaning |
|---|---|
| Passed | The item worked as expected |
| Failed | The item did not work as expected |
| Blocked | The item could not be tested due to a blocker |
| Not Applicable | The item does not apply to the current application version |
| Not Executed | The item has not been executed yet |

---

## 7. Regression Test Checklist

| ID | Area | Checkpoint | Expected Result | Status | Notes |
|---|---|---|---|---|---|
| REG-001 | Application | Open the Firmus application | The application should load without critical errors | Not Executed |  |
| REG-002 | Authentication | Access the login page | The login page should be visible and usable | Not Executed |  |
| REG-003 | Authentication | Log in with valid credentials | The user should be authenticated successfully | Not Executed |  |
| REG-004 | Authentication | Try login with invalid credentials | The system should reject invalid credentials and show feedback | Not Executed |  |
| REG-005 | Protected Routes | Access a protected route while logged out | The system should prevent access and redirect the user | Not Executed |  |
| REG-006 | Protected Routes | Access a protected route while logged in | The authenticated user should access the route successfully | Not Executed |  |
| REG-007 | Session | Refresh a protected page while authenticated | The page should remain usable if the session is valid | Not Executed |  |
| REG-008 | Logout | Log out from the application | The user should be logged out successfully | Not Executed |  |
| REG-009 | Post-Logout Access | Try to access a protected route after logout | The system should prevent access to protected areas | Not Executed |  |
| REG-010 | Dashboard | Load the Dashboard / Control Tower | The dashboard should load correctly after login | Not Executed |  |
| REG-011 | Dashboard | Verify dashboard summary cards | Summary cards should be visible, readable and organized | Not Executed |  |
| REG-012 | Dashboard | Verify next actions section | The section should be visible and understandable | Not Executed |  |
| REG-013 | Dashboard | Verify recent activities section | The section should be visible and readable | Not Executed |  |
| REG-014 | Navigation | Use the main navigation menu | Navigation should work without broken routes | Not Executed |  |
| REG-015 | Clients | Access the clients area | The clients page should load successfully | Not Executed |  |
| REG-016 | Clients | Verify clients list or empty state | The page should show records or a clear empty state | Not Executed |  |
| REG-017 | Clients | Validate create client action, if available | The action should be visible and usable | Not Executed |  |
| REG-018 | Quotes | Access the quotes area | The quotes page should load successfully | Not Executed |  |
| REG-019 | Quotes | Verify quotes list or empty state | The page should show records or a clear empty state | Not Executed |  |
| REG-020 | Quotes | Validate create quote action, if available | The action should be visible and usable | Not Executed |  |
| REG-021 | Quotes | Verify quote status visibility | Quote statuses should be visible and understandable | Not Executed |  |
| REG-022 | Financial | Access the financial area | The financial page should load successfully | Not Executed |  |
| REG-023 | Financial | Verify financial summary cards | Financial summary information should be visible and readable | Not Executed |  |
| REG-024 | Financial | Verify monetary value formatting | Monetary values should be displayed clearly and consistently | Not Executed |  |
| REG-025 | NFSe | Access the NFSe area | The NFSe page should load successfully | Not Executed |  |
| REG-026 | NFSe | Verify NFSe records or empty state | The page should show records or a clear empty state | Not Executed |  |
| REG-027 | NFSe | Verify fiscal status visibility | Fiscal statuses should be visible and understandable | Not Executed |  |
| REG-028 | NFSe | Verify provider reference and document number, when available | Fiscal identifiers should be readable and not duplicated | Not Executed |  |
| REG-029 | UI | Check for broken text or placeholder content | The application should not show unintended placeholder content | Not Executed |  |
| REG-030 | UI | Check for duplicated visible information | Information should not appear duplicated unexpectedly | Not Executed |  |
| REG-031 | Responsive | Validate desktop viewport | Main pages should remain readable and usable on desktop | Not Executed |  |
| REG-032 | Responsive | Validate mobile-like viewport | Main pages should remain usable without critical layout issues | Not Executed |  |
| REG-033 | Usability | Review main labels, buttons and messages | The application should communicate actions clearly | Not Executed |  |
| REG-034 | Evidence | Capture evidence for failed items | Failed items should have screenshots or videos when useful | Not Executed |  |

---

## 8. Regression Exit Criteria

Regression testing can be considered passed when:

- Critical authentication flows work correctly.
- Protected route behavior remains correct.
- Dashboard loads and displays key information.
- Main navigation works.
- Core modules are accessible.
- No critical blocker is found.
- No previously fixed critical bug reappears.
- Failed items are documented with clear notes or bug reports.

If a critical regression failure is found, the application should not be considered stable until the issue is documented and fixed or accepted as a known limitation.

---

## 9. Critical Regression Failures

The following failures should be treated as critical or high risk:

- Login stops working.
- Logout stops working.
- Protected routes become accessible without authentication.
- Dashboard stops loading.
- Main navigation breaks.
- Clients area becomes inaccessible.
- Quotes area becomes inaccessible.
- Financial area becomes inaccessible.
- NFSe area becomes inaccessible.
- A previously fixed critical bug reappears.
- The application crashes during normal navigation.

Any critical regression failure should generate a bug report.

---

## 10. Regression Notes

During execution, update each checklist item with:

- Status
- Notes
- Evidence, when applicable
- Related bug ID, when applicable

If an item fails, create a bug report using:

```txt
bug-reports/bug-report-template.md
```

Evidence should be stored in:

```txt
evidences/screenshots/
evidences/videos/
```

---

## 11. Relationship With Test Cases

This checklist is a high-level regression guide.

Detailed validation should still reference the manual test case files:

```txt
test-cases/authentication-test-cases.md
test-cases/dashboard-test-cases.md
test-cases/clients-test-cases.md
test-cases/quotes-test-cases.md
test-cases/financial-test-cases.md
test-cases/nfse-test-cases.md
```

When a regression item needs deeper validation, the related test cases should be executed.

---

## 12. Approval Criteria

This regression test checklist is considered ready when:

- Critical application areas are listed.
- Main regression risks are covered.
- Expected results are clear.
- Status options are defined.
- The checklist supports repeated validation after changes.
- Failed items can be linked to bug reports and evidence.
# NFSe Test Cases — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Module | NFSe Foundation |
| Test Type | Manual Functional Testing |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | In progress |

---

## 2. Module Overview

The NFSe Foundation module is responsible for presenting the foundational user-facing flows related to service invoice operations within the Firmus application.

This test suite validates whether the user can access the NFSe area, view NFSe-related records, understand fiscal statuses and interact with available NFSe information from the user interface.

The goal is to ensure that NFSe-related information is clear, organized and usable from the user's perspective.

---

## 3. Test Scope

This test suite covers:

- NFSe page loading
- NFSe records visibility
- Empty state behavior
- Provider reference visibility, when available
- Document number visibility, when available
- Fiscal status visibility
- Basic validation of user-facing NFSe information
- NFSe-related navigation
- Basic visual consistency
- Basic responsive behavior
- Basic usability of fiscal information

Out of scope:

- Real NFSe issuance with government provider
- Fiscal authority integration
- Legal tax validation
- Provider API behavior
- XML validation
- Production fiscal compliance validation
- Database validation
- API testing
- Automated testing

---

## 4. Test Cases

---

## TC-NFSE-001 — NFSe page loads successfully

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-001 |
| Module | NFSe Foundation |
| Type | Functional / Smoke |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.

### Steps

1. Log in to the Firmus application.
2. Navigate to the NFSe area.
3. Observe the page loading behavior.

### Expected Result

The NFSe page should load successfully without errors, broken layout or unexpected redirects.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This is a smoke test for the NFSe module.

---

## TC-NFSE-002 — NFSe records are visible when records exist

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-002 |
| Module | NFSe Foundation |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | High |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one NFSe record exists.

### Steps

1. Access the NFSe page.
2. Locate the NFSe records section.
3. Verify if NFSe records are displayed.
4. Check if each record shows relevant visible information.

### Expected Result

The NFSe page should display existing NFSe records clearly and in an organized way.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the environment has no NFSe records, this test may be marked as Blocked or Not Applicable.

---

## TC-NFSE-003 — NFSe empty state is clear when no records exist

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-003 |
| Module | NFSe Foundation |
| Type | Functional / Empty State |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- No NFSe records are available in the current environment.

### Steps

1. Access the NFSe page.
2. Observe the NFSe records area.
3. Verify if an empty state message is displayed.
4. Check if the message is clear and helpful.
5. Check if the page avoids looking broken or incomplete.

### Expected Result

The page should display a clear empty state explaining that no NFSe records are available.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the environment always contains sample NFSe records, this test may be marked as Not Applicable.

---

## TC-NFSE-004 — NFSe fiscal status is visible and understandable

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-004 |
| Module | NFSe Foundation |
| Type | Functional / Visual |
| Priority | High |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one NFSe record exists.

### Steps

1. Access the NFSe page.
2. Locate an existing NFSe record.
3. Verify if the fiscal status is visible.
4. Check if the status label is readable and understandable.

### Expected Result

Each NFSe record should display a clear fiscal status when applicable.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Status labels should help the user understand the current fiscal state of the record.

---

## TC-NFSE-005 — Provider reference is displayed when available

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-005 |
| Module | NFSe Foundation |
| Type | Functional / Data Presentation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one NFSe record has a provider reference.

### Steps

1. Access the NFSe page.
2. Locate an NFSe record with provider reference.
3. Verify if the provider reference is displayed.
4. Check if the information is readable and not duplicated.

### Expected Result

The provider reference should be displayed clearly when available and should not appear duplicated or broken.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If no provider reference exists in the current environment, this test may be marked as Not Applicable.

---

## TC-NFSE-006 — Document number is displayed when available

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-006 |
| Module | NFSe Foundation |
| Type | Functional / Data Presentation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one NFSe record has a document number.

### Steps

1. Access the NFSe page.
2. Locate an NFSe record with document number.
3. Verify if the document number is displayed.
4. Check if the information is readable and not duplicated.

### Expected Result

The document number should be displayed clearly when available and should not appear duplicated or broken.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If no document number exists in the current environment, this test may be marked as Not Applicable.

---

## TC-NFSE-007 — NFSe issue date or emitted date is displayed when available

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-007 |
| Module | NFSe Foundation |
| Type | Functional / Data Presentation |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- At least one NFSe record has an issue date or emitted date.

### Steps

1. Access the NFSe page.
2. Locate an NFSe record with date information.
3. Verify if the date is displayed.
4. Check if the date format is readable and understandable.

### Expected Result

The NFSe date information should be displayed clearly when available.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Date information should not be confusing or inconsistent with the rest of the UI.

---

## TC-NFSE-008 — NFSe record information is not duplicated inside the same card

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-008 |
| Module | NFSe Foundation |
| Type | Functional / Visual |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The NFSe page is loaded.
- At least one NFSe record exists.

### Steps

1. Access the NFSe page.
2. Review each visible NFSe record.
3. Check if provider reference appears only once when available.
4. Check if document number appears only once when available.
5. Check if fiscal status appears only once when available.
6. Check for duplicated labels or repeated information inside the same record.

### Expected Result

Each NFSe record should display information only once unless repetition is intentionally designed.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test helps detect visual duplication or selector/namespace issues visible in the UI.

---

## TC-NFSE-009 — NFSe page does not display placeholder or broken information

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-009 |
| Module | NFSe Foundation |
| Type | Visual / Usability |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The NFSe page is loaded.

### Steps

1. Access the NFSe page.
2. Review visible titles, labels, cards, tables or list items.
3. Check for placeholder text.
4. Check for missing values.
5. Check for duplicated or broken information.
6. Check if any section appears visually incomplete.

### Expected Result

The NFSe page should not display broken text, unexpected placeholder content, duplicated labels or visually incomplete information.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test helps identify polish and presentation issues.

---

## TC-NFSE-010 — NFSe-related navigation works correctly

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-010 |
| Module | NFSe Foundation |
| Type | Functional / Navigation |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The NFSe page is loaded.

### Steps

1. Access the NFSe page.
2. Interact with available NFSe-related navigation actions.
3. Navigate to another related area, if available.
4. Return to the NFSe page.
5. Observe if navigation works correctly.

### Expected Result

NFSe-related navigation should work without broken routes, unexpected errors or confusing behavior.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Any broken navigation should be documented as a bug.

---

## TC-NFSE-011 — NFSe page remains usable after refresh

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-011 |
| Module | NFSe Foundation |
| Type | Functional / Session |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The NFSe page is loaded.

### Steps

1. Access the NFSe page.
2. Refresh the browser page.
3. Wait for the page to reload.
4. Observe the page behavior.

### Expected Result

The NFSe page should reload correctly and remain usable as long as the user session is still valid.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

If the session expires after refresh by design, document the behavior.

---

## TC-NFSE-012 — NFSe page is readable on desktop viewport

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-012 |
| Module | NFSe Foundation |
| Type | Responsive / Visual |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The NFSe page is loaded.
- The browser is using a desktop viewport.

### Steps

1. Access the NFSe page using a desktop viewport.
2. Verify if records or empty states are aligned correctly.
3. Verify if fiscal information is readable.
4. Verify if sections have proper spacing.
5. Verify if navigation remains visible and usable.

### Expected Result

The NFSe page should be readable, organized and usable on desktop viewport.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test supports basic responsive validation.

---

## TC-NFSE-013 — NFSe page is usable on mobile-like viewport

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-013 |
| Module | NFSe Foundation |
| Type | Responsive / Usability |
| Priority | Medium |
| Severity if failed | Medium |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The NFSe page is loaded.
- The browser viewport is resized to a mobile-like width.

### Steps

1. Access the NFSe page.
2. Resize the browser to a mobile-like viewport or use DevTools device mode.
3. Verify if records or empty states remain readable.
4. Verify if buttons remain visible and usable.
5. Verify if navigation remains accessible.
6. Check for horizontal scrolling or content overflow.

### Expected Result

The NFSe page should remain usable on a mobile-like viewport, without broken layout or unreadable content.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

Any layout issue should be documented with screenshot evidence.

---

## TC-NFSE-014 — NFSe information is understandable for the user

| Field | Information |
|---|---|
| Test Case ID | TC-NFSE-014 |
| Module | NFSe Foundation |
| Type | Usability / Content |
| Priority | Medium |
| Severity if failed | Low |
| Status | Not Executed |

### Preconditions

- The application is running.
- The user is authenticated.
- The NFSe page is loaded.

### Steps

1. Access the NFSe page.
2. Review the page title, section labels and NFSe records.
3. Check if the user can understand what each fiscal information means.
4. Check if fiscal statuses are clear.
5. Check if the page avoids using confusing technical terms without context.

### Expected Result

The NFSe page should communicate fiscal information clearly enough for the user to understand the current state of each record.

### Actual Result

To be filled during execution.

### Evidence

To be added if necessary.

### Notes

This test validates only user-facing clarity, not legal or fiscal compliance.

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
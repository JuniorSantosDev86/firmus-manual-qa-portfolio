# Bug Report Template — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Document Type | Bug Report Template |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | Approved for use |

---

## 2. Bug Report Purpose

This template defines the standard format for reporting bugs found during the manual QA process applied to the Firmus application.

The goal is to make each bug report clear, objective, reproducible and useful for developers, QA reviewers and stakeholders.

Each bug report should describe only one issue.

---

## 3. Bug Report Structure

Use the following structure when documenting a bug:

```txt
Bug ID:
Title:
Module:
Environment:
Severity:
Priority:
Status:
Reported by:
Reported date:
Preconditions:
Steps to reproduce:
Actual result:
Expected result:
Evidence:
Additional notes:
```

---

## 4. Bug Report Template

## BUG-XXX — Short and clear bug title

| Field | Information |
|---|---|
| Bug ID | BUG-XXX |
| Module | Module name |
| Environment | Local development |
| Browser | Browser name and version |
| Operating System | OS name and version |
| Device / Viewport | Desktop, tablet-like or mobile-like |
| Severity | Critical / High / Medium / Low |
| Priority | High / Medium / Low |
| Status | Open / In Review / Fixed / Retest / Closed |
| Reported by | Ademir dos Santos Junior |
| Reported date | YYYY-MM-DD |

---

## Summary

Briefly describe the issue in one or two sentences.

The summary should explain what is wrong and where the issue happens.

---

## Preconditions

- Describe what must be true before reproducing the bug.
- Example: The user must be authenticated.
- Example: At least one client record must exist.
- Example: The application must be running locally.

---

## Steps to Reproduce

1. Step one.
2. Step two.
3. Step three.
4. Step four.

---

## Actual Result

Describe what actually happened.

The actual result must be objective and based on observed behavior.

---

## Expected Result

Describe what should have happened according to the expected system behavior.

---

## Evidence

Add evidence when available.

Examples:

- Screenshot: `../evidences/screenshots/example-file-name.png`
- Video: `../evidences/videos/example-file-name.mp4`
- Console observation: describe the visible console issue if relevant

---

## Additional Notes

Add any extra context that helps understand or reproduce the bug.

Examples:

- The issue happens only on mobile viewport.
- The issue happens after page refresh.
- The issue happens only when there are no records.
- The issue may be related to navigation behavior.
- The issue was reproduced more than once.

---

## 5. Example Bug Report

## BUG-001 — Dashboard remains accessible after logout

| Field | Information |
|---|---|
| Bug ID | BUG-001 |
| Module | Authentication / Protected Routes |
| Environment | Local development |
| Browser | Google Chrome |
| Operating System | Ubuntu Linux |
| Device / Viewport | Desktop |
| Severity | Critical |
| Priority | High |
| Status | Open |
| Reported by | Ademir dos Santos Junior |
| Reported date | YYYY-MM-DD |

---

## Summary

After logging out, the user can still access a protected dashboard route by using the browser back button or direct URL access.

---

## Preconditions

- The application is running locally.
- The user has valid credentials.
- The user is authenticated.
- The user has accessed the dashboard before logging out.

---

## Steps to Reproduce

1. Open the Firmus application.
2. Log in with valid credentials.
3. Access the dashboard page.
4. Click the logout option.
5. After logout, try to access the dashboard route directly or use the browser back button.
6. Observe the system behavior.

---

## Actual Result

The user can still view or access the protected dashboard area after logout.

---

## Expected Result

The system should prevent access to protected routes after logout and redirect the user to the login page or another public route.

---

## Evidence

Evidence should be added during real execution if this issue is reproduced.

Example:

- Screenshot: `../evidences/screenshots/BUG-001-dashboard-access-after-logout.png`
- Video: `../evidences/videos/BUG-001-dashboard-access-after-logout.mp4`

---

## Additional Notes

This is only an example bug report structure. Real bug reports should be created only when the issue is reproduced during the official execution cycle.

---

## 6. Bug Writing Guidelines

A good bug report should be:

- Clear
- Objective
- Reproducible
- Specific
- Evidence-based
- Useful for developers

Avoid vague titles such as:

```txt
Something is wrong
Page broken
Error happened
Bug in dashboard
```

Prefer clear titles such as:

```txt
Dashboard displays duplicated financial summary cards
User remains on protected page after logout
Quote creation allows invalid monetary value
Mobile layout shows horizontal scroll on clients page
NFSe record displays duplicated provider reference
```

---

## 7. Severity and Priority Reference

Use the project severity and priority guide before classifying bugs:

```txt
docs/severity-priority-guide.md
```

Severity describes the impact of the issue.

Priority describes how urgently the issue should be fixed.

---

## 8. Bug Status Definitions

| Status | Meaning |
|---|---|
| Open | The bug was reported and is waiting for review |
| In Review | The bug is being analyzed |
| Fixed | A correction was implemented |
| Retest | The bug is ready to be retested |
| Closed | The bug was validated and no longer reproduces |
| Not a Bug | The behavior was confirmed as expected |
| Won't Fix | The issue will not be fixed at this time |

---

## 9. Evidence Naming Convention

Evidence files should use clear and traceable names.

Recommended format:

```txt
BUG-XXX-short-description.png
BUG-XXX-short-description.mp4
```

Examples:

```txt
BUG-001-dashboard-access-after-logout.png
BUG-002-mobile-clients-horizontal-scroll.png
BUG-003-invalid-quote-value-accepted.png
```

Evidence should be stored in:

```txt
evidences/screenshots/
evidences/videos/
```

---

## 10. Approval Criteria

This bug report template is considered ready when:

- The structure is clear.
- The fields support reproducibility.
- Severity and priority are included.
- Evidence guidance is included.
- Example bug report is included.
- The template can be reused during the official manual execution cycle.
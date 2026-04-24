# Severity and Priority Guide — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Document Type | Severity and Priority Guide |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | In progress |

---

## 2. Objective

The objective of this document is to define how severity and priority are classified during the manual QA process applied to the Firmus application.

This guide helps ensure that bugs are reported consistently, objectively and professionally.

It also supports better communication between QA, developers, product stakeholders and reviewers.

---

## 3. Severity vs Priority

Severity and priority are related, but they are not the same.

**Severity** describes the impact of a bug on the system, user flow or business operation.

**Priority** describes how urgently the bug should be fixed.

A bug can have high severity but medium priority, or low severity but high priority, depending on business context.

Example:

- A login bug that blocks all users from accessing the application has **Critical severity** and **High priority**.
- A typo on a public page may have **Low severity**, but if it appears on a production landing page during a launch, it may have **High priority**.

---

## 4. Severity Classification

Severity is based on the technical or functional impact of the issue.

| Severity | Description |
|---|---|
| Critical | Blocks a critical flow or prevents the system from being used |
| High | Affects an important feature with no simple workaround |
| Medium | Affects a feature but has an available workaround |
| Low | Minor visual, text, layout or usability issue |

---

## 5. Critical Severity

A bug should be classified as **Critical** when it prevents the user from using an essential part of the system.

### Examples

- User cannot log in with valid credentials.
- Authenticated user cannot access the dashboard.
- Protected routes are accessible without authentication.
- The application crashes during a critical flow.
- The quote creation flow is completely blocked.
- The client management area is unavailable.
- A fiscal or financial page fails to load completely.

### Expected Handling

Critical bugs should be documented immediately with clear reproduction steps and evidence.

---

## 6. High Severity

A bug should be classified as **High** when it affects an important feature and there is no simple workaround.

### Examples

- A client cannot be created even with valid data.
- A quote is created but does not appear in the quote list.
- Financial summary cards display missing or unreadable values.
- NFSe records do not show important fiscal status information.
- Logout does not properly end the authenticated session.
- A main navigation item redirects to the wrong page.

### Expected Handling

High severity bugs should be prioritized for investigation because they affect relevant business flows.

---

## 7. Medium Severity

A bug should be classified as **Medium** when it affects a feature, but the user can still continue using the system with a workaround.

### Examples

- A validation message is unclear but the form still prevents invalid submission.
- A filter does not work correctly, but records can still be manually reviewed.
- A dashboard card displays information with minor inconsistency.
- A page refresh causes temporary confusion but does not block the flow.
- A status label is visible but not very clear.
- A mobile layout has spacing issues but remains usable.

### Expected Handling

Medium severity bugs should be documented clearly and reviewed during planned correction cycles.

---

## 8. Low Severity

A bug should be classified as **Low** when it has minor impact on functionality or user experience.

### Examples

- Minor typo.
- Small spacing inconsistency.
- Slight visual misalignment.
- Placeholder text appears in a non-critical area.
- Button label could be clearer.
- A non-critical visual element appears inconsistent.

### Expected Handling

Low severity bugs should still be reported when they affect polish, clarity or professional quality.

---

## 9. Priority Classification

Priority is based on urgency and business relevance.

| Priority | Description |
|---|---|
| High | Should be fixed as soon as possible |
| Medium | Should be fixed in a planned development cycle |
| Low | Can be fixed later without major impact |

---

## 10. High Priority

A bug should be classified as **High Priority** when it needs quick attention because it affects a critical user journey, business operation or product credibility.

### Examples

- Login is blocked.
- Dashboard is unavailable.
- Client creation is blocked.
- Quote creation is blocked.
- Protected routes are exposed.
- Main navigation is broken.
- Public quote page exposes incorrect or private information.

---

## 11. Medium Priority

A bug should be classified as **Medium Priority** when it should be fixed in a planned development cycle, but does not require immediate interruption of other work.

### Examples

- A secondary action does not work.
- A filter behaves inconsistently.
- A validation message needs improvement.
- A responsive issue affects usability but does not block the user.
- Some records have unclear status labels.
- Empty states need clearer guidance.

---

## 12. Low Priority

A bug should be classified as **Low Priority** when it can be fixed later without significant impact on the user or business flow.

### Examples

- Minor visual inconsistency.
- Small text improvement.
- Non-critical spacing issue.
- Minor alignment issue.
- Low-impact UI polish.
- Optional improvement in wording.

---

## 13. Severity and Priority Matrix

| Severity | Common Priority | Example |
|---|---|---|
| Critical | High | Login is unavailable for valid users |
| High | High or Medium | Quote creation fails with valid data |
| Medium | Medium | Filter does not update results correctly |
| Low | Low or Medium | Minor visual issue on a secondary page |

This matrix is a guide. Final priority may change depending on business context.

---

## 14. Classification Examples for Firmus

| Scenario | Severity | Priority | Reason |
|---|---|---|---|
| User cannot log in with valid credentials | Critical | High | Blocks access to the entire application |
| Dashboard does not load after login | Critical | High | Blocks the main operational entry point |
| Client creation fails with valid data | High | High | Blocks an important business workflow |
| Quote value accepts invalid format | Medium | Medium | Affects data quality, but may have workaround |
| Financial card has unclear label | Low | Medium | Minor issue, but affects business understanding |
| NFSe status is missing from a record | Medium | Medium | Reduces clarity of fiscal information |
| Mobile layout has horizontal scroll | Medium | Medium | Affects usability on smaller screens |
| Typo in a secondary section | Low | Low | Does not block usage |

---

## 15. Bug Classification Rules

When classifying a bug, consider the following questions:

1. Does the bug block the user from completing a critical flow?
2. Does the bug affect authentication, dashboard, clients, quotes, financial data or NFSe visibility?
3. Is there a workaround?
4. Does the bug affect many users or only a specific scenario?
5. Does the bug expose private or incorrect information?
6. Does the bug damage user trust?
7. Is the bug only visual or does it affect functionality?
8. Does the issue appear in a public-facing flow?

The answers help define severity and priority more accurately.

---

## 16. General QA Guidelines

- Report one bug per bug report.
- Use objective language.
- Avoid emotional or vague descriptions.
- Always describe the actual result and expected result.
- Add evidence when possible.
- Do not classify every bug as Critical.
- Do not ignore Low severity bugs when they affect professionalism.
- Separate functional impact from business urgency.
- Reevaluate priority if product context changes.

---

## 17. Approval Criteria

This guide is considered approved when:

- Severity levels are clearly defined.
- Priority levels are clearly defined.
- Severity and priority are explained separately.
- Practical examples are documented.
- Firmus-specific scenarios are included.
- The guide supports future bug reporting activities.
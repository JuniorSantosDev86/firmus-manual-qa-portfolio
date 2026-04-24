# Exploratory Test Checklist — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Document Type | Exploratory Test Checklist |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | Ready for execution |

---

## 2. Objective

The objective of this exploratory test checklist is to guide unscripted manual testing activities in the Firmus application.

Exploratory testing helps identify issues that may not be covered by predefined test cases, smoke checks or regression checklists.

The goal is to observe the application from a real user's perspective, investigate unexpected behaviors and discover usability, navigation, validation, layout or flow problems.

---

## 3. Exploratory Testing Scope

This checklist covers exploratory validation for the main user-facing areas of the Firmus application:

- Authentication
- Protected routes
- Dashboard / Control Tower
- Main navigation
- Clients
- Quotes
- Financial overview
- NFSe foundation
- Forms and validations
- Empty states
- Error messages
- Responsive behavior
- General usability
- Visual consistency
- Unexpected user behavior

This checklist does not replace structured test cases. It complements them by encouraging investigation beyond predefined steps.

---

## 4. Exploratory Testing Approach

Exploratory testing should be performed with curiosity, critical thinking and attention to real user behavior.

During execution, the tester should ask questions such as:

- What happens if the user does something unexpected?
- Is the interface clear enough?
- Are error messages helpful?
- Does the application recover well from mistakes?
- Are important actions easy to find?
- Are empty states understandable?
- Does navigation feel consistent?
- Does the application behave correctly after refresh?
- Does the application remain usable on smaller screens?
- Is there any confusing, duplicated or broken information?

---

## 5. Execution Information

| Field | Information |
|---|---|
| Execution Date | YYYY-MM-DD |
| Environment | Local development |
| Browser | Google Chrome / Chromium-based browser |
| Operating System | Ubuntu Linux |
| Executed by | Ademir dos Santos Junior |
| Session Duration | To be filled during execution |

---

## 6. Status Legend

| Status | Meaning |
|---|---|
| Passed | No relevant issue was found in this area |
| Failed | An issue was found and should be documented |
| Blocked | The area could not be explored due to a blocker |
| Not Applicable | The item does not apply to the current application version |
| Not Executed | The item has not been explored yet |

---

## 7. Exploratory Test Checklist

| ID | Area | Exploration Focus | Expected Observation | Status | Notes |
|---|---|---|---|---|---|
| EXP-001 | Application | Open the application and observe initial loading | The application should load without critical errors or broken UI | Not Executed |  |
| EXP-002 | Application | Navigate through the app like a first-time user | The main purpose and navigation should be understandable | Not Executed |  |
| EXP-003 | Authentication | Explore login behavior with valid credentials | Login should be clear, stable and predictable | Not Executed |  |
| EXP-004 | Authentication | Explore invalid login attempts | Error feedback should be visible and understandable | Not Executed |  |
| EXP-005 | Authentication | Try submitting login form with empty fields | Required field behavior should be clear | Not Executed |  |
| EXP-006 | Authentication | Refresh page during authenticated session | Session behavior should remain consistent | Not Executed |  |
| EXP-007 | Protected Routes | Try accessing private routes while logged out | Private areas should not be accessible without authentication | Not Executed |  |
| EXP-008 | Logout | Explore logout behavior | User should be logged out and protected areas should no longer be accessible | Not Executed |  |
| EXP-009 | Dashboard | Explore dashboard information as a business user | Dashboard should provide clear operational visibility | Not Executed |  |
| EXP-010 | Dashboard | Look for confusing or duplicated dashboard information | Dashboard should not show duplicated, broken or unclear information | Not Executed |  |
| EXP-011 | Dashboard | Explore next actions section | Actions should be readable, useful and understandable | Not Executed |  |
| EXP-012 | Dashboard | Explore recent activities section | Activities should be clear, readable and useful | Not Executed |  |
| EXP-013 | Navigation | Click through main navigation items | Navigation should be consistent and predictable | Not Executed |  |
| EXP-014 | Navigation | Use browser back and forward buttons | Application state should remain understandable | Not Executed |  |
| EXP-015 | Navigation | Refresh pages inside protected areas | Pages should reload correctly when session is valid | Not Executed |  |
| EXP-016 | Clients | Explore clients page as a business user | Client information should be clear and usable | Not Executed |  |
| EXP-017 | Clients | Explore client empty state, if available | Empty state should explain what is happening and guide the user | Not Executed |  |
| EXP-018 | Clients | Explore client creation flow, if available | Form should be understandable and validation should be clear | Not Executed |  |
| EXP-019 | Clients | Try invalid or incomplete client data | System should prevent invalid submission or show clear feedback | Not Executed |  |
| EXP-020 | Quotes | Explore quotes page as a service provider | Quote information should be clear and useful | Not Executed |  |
| EXP-021 | Quotes | Explore quote creation flow, if available | Quote creation should be understandable and predictable | Not Executed |  |
| EXP-022 | Quotes | Try unusual monetary values | System should handle invalid or unusual values clearly | Not Executed |  |
| EXP-023 | Quotes | Explore quote statuses | Status labels should be visible and understandable | Not Executed |  |
| EXP-024 | Quotes | Explore public quote access, if available | Public quote page should expose only intended information | Not Executed |  |
| EXP-025 | Financial | Explore financial overview as a business user | Financial information should be readable and useful | Not Executed |  |
| EXP-026 | Financial | Look for unclear monetary values | Monetary values should be formatted consistently | Not Executed |  |
| EXP-027 | Financial | Explore financial statuses or indicators | Statuses should be understandable and not misleading | Not Executed |  |
| EXP-028 | Financial | Look for inconsistent financial information | Values should not appear duplicated, missing or unexpectedly negative | Not Executed |  |
| EXP-029 | NFSe | Explore NFSe page as a user with fiscal needs | Fiscal information should be clear enough for the user | Not Executed |  |
| EXP-030 | NFSe | Look for duplicated fiscal identifiers | Provider reference and document number should not appear duplicated | Not Executed |  |
| EXP-031 | NFSe | Explore fiscal statuses | Status labels should help the user understand the record state | Not Executed |  |
| EXP-032 | NFSe | Explore NFSe empty state, if available | Empty state should not look like an error | Not Executed |  |
| EXP-033 | Forms | Try submitting forms without required data | Validation messages should be visible and helpful | Not Executed |  |
| EXP-034 | Forms | Try unusual characters in text fields | System should handle input safely and clearly | Not Executed |  |
| EXP-035 | Forms | Try very long text in available fields | Layout should not break and input behavior should remain stable | Not Executed |  |
| EXP-036 | Forms | Try canceling or leaving a form | User should understand whether data was saved or discarded | Not Executed |  |
| EXP-037 | Empty States | Explore pages with no available records | Empty states should be clear and helpful | Not Executed |  |
| EXP-038 | Error Messages | Look for unclear or generic error messages | Error messages should help the user understand the issue | Not Executed |  |
| EXP-039 | Visual UI | Look for broken text, typos or placeholders | UI should not show unintended placeholder or broken content | Not Executed |  |
| EXP-040 | Visual UI | Look for duplicated labels or cards | UI should not display repeated information unexpectedly | Not Executed |  |
| EXP-041 | Visual UI | Check spacing and alignment | Layout should look organized and professional | Not Executed |  |
| EXP-042 | Responsive | Explore the application on mobile-like viewport | Main flows should remain usable on smaller screens | Not Executed |  |
| EXP-043 | Responsive | Explore mobile navigation | Drawer or mobile navigation should be accessible and usable | Not Executed |  |
| EXP-044 | Responsive | Look for horizontal scrolling | Pages should not show unexpected horizontal scrolling | Not Executed |  |
| EXP-045 | Usability | Evaluate whether main actions are easy to find | Important actions should be visible and understandable | Not Executed |  |
| EXP-046 | Usability | Evaluate page titles and labels | The user should understand where they are in the system | Not Executed |  |
| EXP-047 | Usability | Evaluate feedback after user actions | The application should provide feedback after important actions | Not Executed |  |
| EXP-048 | Usability | Explore user confusion points | Confusing flows should be documented for improvement | Not Executed |  |

---

## 8. Exploratory Testing Charters

Use the following charters to guide exploratory sessions.

### Charter 1 — Authentication and Session

Explore how the application behaves when users log in, log out, refresh protected pages and attempt to access private routes without authentication.

Focus on:

- Login clarity
- Invalid login feedback
- Session persistence
- Protected route behavior
- Logout behavior
- Post-logout access

---

### Charter 2 — Operational Visibility

Explore whether the dashboard gives the user a clear understanding of the current business situation.

Focus on:

- Summary cards
- Next actions
- Recent activities
- Empty states
- Visual hierarchy
- Duplicated or unclear information

---

### Charter 3 — Core Business Flows

Explore whether the main operational modules are clear and usable.

Focus on:

- Clients
- Quotes
- Financial overview
- NFSe foundation
- Navigation between modules
- Main actions
- Data visibility
- Status labels

---

### Charter 4 — Forms and Validation

Explore how the application behaves when the user submits incomplete, invalid, unusual or unexpected data.

Focus on:

- Required fields
- Invalid formats
- Long text
- Special characters
- Monetary values
- Clear validation feedback
- Form cancellation or navigation away

---

### Charter 5 — Responsive and Usability

Explore whether the application remains usable across smaller screens and whether the user can understand the interface easily.

Focus on:

- Mobile-like viewport
- Navigation drawer
- Card stacking
- Text readability
- Button visibility
- Horizontal scrolling
- Content overflow
- Touch-friendly actions

---

## 9. Exploratory Exit Criteria

Exploratory testing can be considered complete when:

- Main exploratory charters have been executed.
- Critical modules have been explored.
- Unexpected behaviors have been documented.
- Potential bugs have been reviewed.
- Valid bugs have been reported using the bug report template.
- Evidence has been captured when useful.
- Notes have been added for usability or improvement observations.

---

## 10. Critical Exploratory Findings

The following findings should be treated as high risk:

- User can access protected areas without authentication.
- User remains authenticated after logout unexpectedly.
- Critical modules are inaccessible.
- Data is duplicated or misleading in important business areas.
- Financial or fiscal information appears broken or unclear.
- Main navigation fails during normal use.
- Forms accept clearly invalid critical data without feedback.
- Mobile layout blocks access to core functionality.
- Public quote page exposes private or unintended information.

High-risk findings should generate bug reports.

---

## 11. Evidence Guidelines

When an exploratory finding is relevant, evidence should include:

- Screenshot or video of the behavior.
- Page or module where the issue happened.
- Short description of the action performed.
- Viewport size, when related to responsive behavior.
- Browser console observation, when relevant.

Evidence should be stored in:

```txt
evidences/screenshots/
evidences/videos/
```

Recommended file naming format:

```txt
BUG-XXX-module-short-description.png
BUG-XXX-module-short-description.mp4
```

Examples:

```txt
BUG-005-dashboard-duplicated-summary-card.png
BUG-006-quotes-invalid-value-accepted.png
BUG-007-mobile-navigation-not-opening.mp4
```

---

## 12. Relationship With Other Artifacts

This exploratory checklist supports and complements:

```txt
docs/test-plan.md
docs/test-scope.md
docs/test-strategy.md
docs/severity-priority-guide.md
bug-reports/bug-report-template.md
test-cases/authentication-test-cases.md
test-cases/dashboard-test-cases.md
test-cases/clients-test-cases.md
test-cases/quotes-test-cases.md
test-cases/financial-test-cases.md
test-cases/nfse-test-cases.md
checklists/smoke-test-checklist.md
checklists/regression-test-checklist.md
checklists/responsive-test-checklist.md
```

If exploratory testing reveals a repeatable issue, it should become a bug report.

If exploratory testing reveals a missing important scenario, a new test case may be added in the future.

---

## 13. Exploratory Testing Notes

During execution, update each checklist item with:

- Status
- Notes
- Evidence, when applicable
- Related bug ID, when applicable
- Viewport size, when relevant

Exploratory notes should be objective and based on observed behavior.

Avoid vague notes such as:

```txt
Bad screen.
Looks weird.
Something is wrong.
```

Prefer clear notes such as:

```txt
The dashboard summary card title is truncated on 390px mobile viewport.
The quote creation form accepts negative monetary values without validation.
The NFSe provider reference appears duplicated inside the same record card.
```

---

## 14. Approval Criteria

This exploratory test checklist is considered ready when:

- Main exploratory areas are listed.
- Exploratory charters are defined.
- Authentication, dashboard and core modules are covered.
- Forms, validation and empty states are included.
- Responsive and usability risks are included.
- Evidence guidance is included.
- Findings can be converted into bug reports.
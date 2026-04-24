# Responsive Test Checklist — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Document Type | Responsive Test Checklist |
| Tester | Ademir dos Santos Junior |
| Version | 1.0 |
| Status | Ready for execution |

---

## 2. Objective

The objective of this responsive test checklist is to validate whether the Firmus application remains readable, usable and visually consistent across different viewport sizes.

Responsive testing helps identify layout, navigation, readability and usability issues that may affect users accessing the application from desktop, tablet-like or mobile-like screens.

This checklist focuses on user-facing behavior and practical usability, not pixel-perfect visual certification.

---

## 3. Responsive Test Scope

This checklist covers responsive validation for the main user-facing areas of the Firmus application:

- Login page
- Protected routes
- Dashboard / Control Tower
- Main navigation
- Sidebar or mobile drawer
- Clients page
- Quotes page
- Financial overview
- NFSe foundation
- Forms, buttons and cards
- Text readability
- Horizontal scrolling
- Content overflow
- Basic touch-friendly usability

This checklist does not replace a full cross-device certification process.

---

## 4. Viewports Used for Testing

The following viewport sizes may be used during manual responsive testing:

| Viewport Type | Suggested Size | Purpose |
|---|---:|---|
| Desktop | 1366 x 768 | Validate standard notebook/desktop experience |
| Large Desktop | 1920 x 1080 | Validate larger screen layout behavior |
| Tablet-like | 768 x 1024 | Validate medium screen behavior |
| Mobile-like | 390 x 844 | Validate common mobile-like behavior |
| Small Mobile-like | 360 x 740 | Validate tighter mobile layout behavior |

Viewport sizes may be adjusted according to available browser DevTools presets.

---

## 5. Execution Information

| Field | Information |
|---|---|
| Execution Date | YYYY-MM-DD |
| Environment | Local development |
| Browser | Google Chrome / Chromium-based browser |
| Operating System | Ubuntu Linux |
| Executed by | Ademir dos Santos Junior |

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

## 7. Responsive Test Checklist

| ID | Area | Checkpoint | Expected Result | Status | Notes |
|---|---|---|---|---|---|
| RSP-001 | Application | Open the application on desktop viewport | The application should load with readable and organized layout | Not Executed |  |
| RSP-002 | Application | Open the application on mobile-like viewport | The application should load without critical layout issues | Not Executed |  |
| RSP-003 | Login | Validate login page on desktop viewport | Login fields and button should be visible and aligned | Not Executed |  |
| RSP-004 | Login | Validate login page on mobile-like viewport | Login form should remain usable and readable | Not Executed |  |
| RSP-005 | Login | Check login form spacing on small viewport | Fields and button should not overlap or overflow | Not Executed |  |
| RSP-006 | Navigation | Validate desktop navigation | Sidebar or navigation should be visible and usable | Not Executed |  |
| RSP-007 | Navigation | Validate mobile navigation | Drawer, menu or mobile navigation should be accessible | Not Executed |  |
| RSP-008 | Navigation | Open and close mobile navigation | Mobile navigation should open and close correctly | Not Executed |  |
| RSP-009 | Navigation | Navigate between main modules on mobile-like viewport | Navigation should work without broken routes or blocked access | Not Executed |  |
| RSP-010 | Dashboard | Validate dashboard on desktop viewport | Dashboard cards and sections should be readable and organized | Not Executed |  |
| RSP-011 | Dashboard | Validate dashboard on tablet-like viewport | Dashboard content should adapt without critical layout issues | Not Executed |  |
| RSP-012 | Dashboard | Validate dashboard on mobile-like viewport | Dashboard cards should stack correctly and remain readable | Not Executed |  |
| RSP-013 | Dashboard | Check dashboard horizontal scrolling | The page should not require unexpected horizontal scrolling | Not Executed |  |
| RSP-014 | Dashboard | Validate next actions section on mobile-like viewport | The section should remain readable and usable | Not Executed |  |
| RSP-015 | Dashboard | Validate recent activities section on mobile-like viewport | The section should remain readable and organized | Not Executed |  |
| RSP-016 | Clients | Validate clients page on desktop viewport | Client list or empty state should be readable and organized | Not Executed |  |
| RSP-017 | Clients | Validate clients page on mobile-like viewport | Client content should remain readable without broken layout | Not Executed |  |
| RSP-018 | Clients | Validate create client action on mobile-like viewport | The action should be visible and usable when available | Not Executed |  |
| RSP-019 | Quotes | Validate quotes page on desktop viewport | Quote list or empty state should be readable and organized | Not Executed |  |
| RSP-020 | Quotes | Validate quotes page on mobile-like viewport | Quote content should remain readable without broken layout | Not Executed |  |
| RSP-021 | Quotes | Validate quote actions on mobile-like viewport | Quote-related actions should remain visible and usable | Not Executed |  |
| RSP-022 | Financial | Validate financial page on desktop viewport | Financial cards and records should be readable and organized | Not Executed |  |
| RSP-023 | Financial | Validate financial page on mobile-like viewport | Financial values should remain readable and not overflow | Not Executed |  |
| RSP-024 | Financial | Check monetary values on small viewport | Monetary values should not be cut off or visually broken | Not Executed |  |
| RSP-025 | NFSe | Validate NFSe page on desktop viewport | NFSe records or empty state should be readable and organized | Not Executed |  |
| RSP-026 | NFSe | Validate NFSe page on mobile-like viewport | Fiscal information should remain readable and usable | Not Executed |  |
| RSP-027 | NFSe | Check provider reference and document number on mobile-like viewport | Long identifiers should not break the layout | Not Executed |  |
| RSP-028 | Forms | Validate form fields on mobile-like viewport | Fields should be visible, readable and usable | Not Executed |  |
| RSP-029 | Forms | Validate buttons on mobile-like viewport | Buttons should be visible, tappable and not overlapping | Not Executed |  |
| RSP-030 | Cards | Validate card stacking behavior | Cards should stack naturally without overlap | Not Executed |  |
| RSP-031 | Text | Check text readability on mobile-like viewport | Text should remain readable without excessive compression | Not Executed |  |
| RSP-032 | Layout | Check for content overflow | Content should not overflow outside the visible area unexpectedly | Not Executed |  |
| RSP-033 | Layout | Check for unexpected horizontal scroll | Pages should not show horizontal scrolling unless intentionally designed | Not Executed |  |
| RSP-034 | Layout | Check spacing between sections | Sections should have enough spacing to remain readable | Not Executed |  |
| RSP-035 | Usability | Validate touch-friendly interaction areas | Important buttons and links should be easy to interact with | Not Executed |  |
| RSP-036 | Usability | Validate page purpose clarity on smaller screens | The user should still understand the page purpose on mobile-like viewport | Not Executed |  |

---

## 8. Responsive Exit Criteria

Responsive testing can be considered passed when:

- Main pages are readable on desktop and mobile-like viewports.
- Main navigation remains usable across viewport sizes.
- Core modules remain accessible.
- Important buttons and actions remain visible.
- Cards, lists and sections adapt without critical overlap.
- Text remains readable.
- No unexpected horizontal scrolling appears in critical pages.
- No critical content is cut off.
- Failed items are documented with notes and evidence when applicable.

---

## 9. Critical Responsive Failures

The following issues should be treated as high risk during responsive testing:

- User cannot log in on mobile-like viewport.
- Main navigation is not accessible on mobile-like viewport.
- Dashboard is unreadable or unusable on smaller screens.
- Core modules cannot be accessed due to layout issues.
- Important buttons are hidden or impossible to click.
- Forms cannot be completed on mobile-like viewport.
- Financial values or fiscal identifiers break the layout.
- Horizontal scrolling prevents normal usage.
- Content overlaps in a way that blocks user actions.

Any critical responsive failure should generate a bug report.

---

## 10. Evidence Guidelines

When a responsive issue is found, evidence should include:

- Screenshot of the affected viewport.
- Viewport size used during testing.
- Page or module where the issue happened.
- Short description of the visible problem.
- Video evidence when the issue involves navigation, drawer behavior or interaction.

Evidence should be stored in:

```txt
evidences/screenshots/
evidences/videos/
```

Recommended file naming format:

```txt
BUG-XXX-module-responsive-issue.png
BUG-XXX-module-responsive-issue.mp4
```

Examples:

```txt
BUG-002-clients-mobile-horizontal-scroll.png
BUG-003-dashboard-cards-overlap-mobile.png
BUG-004-nfse-provider-reference-overflow.png
```

---

## 11. Relationship With Test Cases

This checklist supports responsive validation across the main test case files:

```txt
test-cases/authentication-test-cases.md
test-cases/dashboard-test-cases.md
test-cases/clients-test-cases.md
test-cases/quotes-test-cases.md
test-cases/financial-test-cases.md
test-cases/nfse-test-cases.md
```

When a responsive issue affects a specific module, the related test case should be referenced during bug reporting.

---

## 12. Responsive Testing Notes

During execution, update each checklist item with:

- Status
- Notes
- Evidence, when applicable
- Related bug ID, when applicable
- Viewport size, when relevant

If an item fails, create a bug report using:

```txt
bug-reports/bug-report-template.md
```

Responsive issues should be described clearly, including the viewport where the issue was reproduced.

---

## 13. Approval Criteria

This responsive test checklist is considered ready when:

- Main responsive risk areas are listed.
- Desktop, tablet-like and mobile-like validation are covered.
- Navigation behavior is included.
- Core modules are included.
- Layout, readability and usability risks are covered.
- Evidence guidance is included.
- Failed items can be linked to bug reports and screenshots or videos.
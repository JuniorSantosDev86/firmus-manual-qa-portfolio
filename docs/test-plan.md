# Test Plan — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Tester | Junior Santos |
| Test Type | Manual QA |
| Version | 1.0 |
| Status | In progress |
| Environment | Local development environment |

---

## 2. Objective

The objective of this test plan is to define the scope, strategy, risks, resources, test types and deliverables for the manual QA process applied to the Firmus application.

This document guides the manual testing activities and ensures that the validation process is structured, consistent and aligned with professional QA practices.

---

## 3. Application Overview

Firmus is a B2B operational web application designed to support service providers and small businesses in their daily operations.

The application includes workflows related to:

- Authentication
- Operational dashboard
- Client management
- Service quotes
- Financial visibility
- NFSe-related operations
- Assisted operational actions

The application source code is maintained in a separate repository:

[https://github.com/JuniorSantosDev86/firmus-app](https://github.com/JuniorSantosDev86/firmus-app)

---

## 4. Test Scope

The manual QA scope includes validation of the main user-facing flows available in the Firmus application.

The scope includes:

- Login and logout behavior
- Protected route access
- Dashboard / Control Tower validation
- Client listing and client-related flows
- Quote creation and quote-related flows
- Financial overview validation
- NFSe foundation screens and records
- Responsive behavior
- Basic usability review
- Error handling in visible user flows

---

## 5. Out of Scope

The following items are not part of this manual test cycle:

- Automated test implementation
- Deep security testing
- Load testing
- Stress testing
- Performance benchmarking
- Real NFSe provider integration validation
- Payment gateway validation
- Production monitoring
- Backend code review
- Database integrity testing
- Accessibility audit with specialized tools

These areas may be covered in separate QA portfolio repositories or future testing cycles.

---

## 6. Test Approach

The manual QA process will follow a structured approach based on:

1. Understanding the application context
2. Defining critical user flows
3. Creating manual test cases
4. Executing test cases in a controlled cycle
5. Recording actual results
6. Collecting evidence when necessary
7. Reporting bugs with clear reproduction steps
8. Summarizing the execution results
9. Producing a final QA report

The focus is to validate business-critical flows from the user's perspective.

---

## 7. Test Types

The following test types will be applied:

| Test Type | Purpose |
|---|---|
| Smoke Testing | Validate if the most critical flows are working before deeper testing |
| Functional Testing | Validate if each feature behaves according to the expected behavior |
| Regression Testing | Recheck existing flows after changes or fixes |
| Exploratory Testing | Investigate potential issues beyond scripted test cases |
| Responsive Testing | Validate basic usability across different screen sizes |
| Usability Review | Identify friction points, confusing flows or unclear interface behavior |

---

## 8. Test Environment

The tests will be executed in a local development environment.

| Item | Description |
|---|---|
| Application | Firmus |
| Environment | Localhost |
| Browser | Google Chrome or Chromium-based browser |
| Operating System | Linux Ubuntu |
| Device | Desktop / Notebook |
| Network | Local environment |
| Test Data | Local or mocked application data |

Environment details may be updated during test execution.

---

## 9. Entry Criteria

Testing can start when:

- The application is running locally
- The main routes are accessible
- The tester can access the system under test
- The main UI flows are available
- Test cases or checklists are prepared
- The environment is stable enough for manual validation

---

## 10. Exit Criteria

Testing can be considered complete when:

- Planned test cases have been executed
- Smoke test checklist has been completed
- Critical flows have been validated
- Bugs found during execution have been documented
- Evidence has been collected when applicable
- Execution summary has been created
- Final test report has been prepared

---

## 11. Test Deliverables

The following deliverables will be produced:

- Test Plan
- Test Scope
- Test Strategy
- Severity and Priority Guide
- Manual Test Cases
- Smoke Test Checklist
- Regression Test Checklist
- Responsive Test Checklist
- Exploratory Test Checklist
- Bug Reports
- Test Execution Cycle
- Execution Summary
- Final QA Report
- Screenshots and video evidence when applicable

---

## 12. Roles and Responsibilities

| Role | Responsibility |
|---|---|
| QA Lead | Defines structure, scope and quality direction |
| QA Senior | Reviews risks, test strategy and coverage |
| QA Analyst | Designs test scenarios and test cases |
| QA Junior | Executes test cases, records results and reports bugs |

In this portfolio project, Junior Santos performs the execution and documentation activities while following a professional QA workflow.

---

## 13. Risk Analysis

| Risk | Impact | Mitigation |
|---|---|---|
| Local environment instability | May block test execution | Document environment issues and rerun validation after stabilization |
| Incomplete feature behavior | May affect expected results | Clearly document assumptions and actual behavior |
| Missing test data | May block specific test cases | Create or reuse available local test data |
| UI changes during testing | May require test case updates | Keep test cases versioned and updated |
| Mocked or temporary data | May limit validation depth | Clearly mention environment limitations in reports |

---

## 14. Severity Classification

| Severity | Description |
|---|---|
| Critical | Blocks a critical flow or prevents the system from being used |
| High | Affects an important feature with no simple workaround |
| Medium | Affects a feature but has an available workaround |
| Low | Minor visual, text, layout or usability issue |

---

## 15. Priority Classification

| Priority | Description |
|---|---|
| High | Should be fixed as soon as possible |
| Medium | Should be fixed in a planned development cycle |
| Low | Can be fixed later without major impact |

---

## 16. Test Data

The test data may include:

- Valid user credentials
- Existing clients
- New client records
- Quote examples
- Financial records
- NFSe example records
- Empty state scenarios
- Invalid input scenarios

Sensitive or private data must not be included in this repository.

---

## 17. Evidence Strategy

Evidence will be collected when necessary to support test results or bug reports.

Evidence may include:

- Screenshots
- Short videos
- Browser console observations
- Visible UI states
- Error messages
- Before and after comparisons

Evidence files should be stored in:

```txt
evidences/screenshots/
evidences/videos/
18. Bug Reporting Strategy

Each bug report should describe only one issue.

Bug reports must include:

Clear title
Environment
Preconditions
Steps to reproduce
Actual result
Expected result
Severity
Priority
Evidence when applicable
Additional notes when useful

The goal is to make each issue clear, reproducible and useful for developers.

19. Assumptions

This test plan assumes that:

The application can be executed locally
The tester has access to the required flows
The application is still evolving
Some data may be mocked or manually created
The goal is portfolio demonstration and practical QA documentation
20. Approval Criteria

This test plan is considered approved when:

The test scope is clear
The out-of-scope items are defined
Test types are documented
Entry and exit criteria are defined
Deliverables are listed
Risks are identified
The document supports the next QA activities
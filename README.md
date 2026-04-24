# Firmus Manual QA Portfolio

Manual QA portfolio project documenting test planning, test scope, test cases, bug reports, test executions and QA evidence for the Firmus application.

> Portuguese version: [README.pt-BR.md](./README.pt-BR.md)

---

## Project Overview

This repository presents a complete Manual Quality Assurance process applied to **Firmus**, a web application designed to support service providers and small businesses in their daily operations.

The main goal of this portfolio is to demonstrate practical QA skills through structured documentation, test planning, scope definition, manual test case design, bug reporting, evidence collection and test execution reporting.

This project is part of a professional QA portfolio focused on real-world software testing practices.

---

## System Under Test

**Firmus** is a B2B operational web application built to help service providers manage important business workflows such as:

- Client management
- Service quotes
- Financial visibility
- Operational dashboard
- NFSe-related workflows
- Assisted operational actions

The application used as the system under test is maintained in a separate repository.

**Application Repository:**  
[https://github.com/JuniorSantosDev86/firmus-app](https://github.com/JuniorSantosDev86/firmus-app)

---

## QA Portfolio Objective

The objective of this repository is to demonstrate the ability to plan, design, execute and document a manual QA process in a professional way.

This includes:

- Understanding the application context
- Defining the test scope
- Creating a test strategy
- Writing manual test cases
- Executing functional test cycles
- Reporting bugs clearly
- Collecting test evidence
- Producing QA documentation
- Communicating test results objectively

---

## QA Activities Covered

This portfolio includes the following QA activities:

| Area | Description |
|---|---|
| Test Planning | Definition of objectives, risks, resources, criteria and deliverables |
| Test Scope | Definition of modules, flows and areas covered by manual testing |
| Test Strategy | Manual testing approach and test types used |
| Test Case Design | Structured test cases with steps, expected results and status |
| Functional Testing | Validation of core application flows |
| Smoke Testing | Quick validation of critical features |
| Regression Testing | Rechecking existing flows after changes |
| Exploratory Testing | Investigation of possible issues beyond scripted cases |
| Responsive Testing | Basic validation across different screen sizes |
| Bug Reporting | Clear documentation of defects with severity and priority |
| Evidence Collection | Screenshots and videos supporting test results |
| Test Execution Report | Summary of executed tests and results |

---

## Tested Modules

The manual QA scope covers the main areas of the Firmus application:

- Authentication
- Protected routes
- Dashboard / Control Tower
- Clients
- Quotes
- Financial overview
- NFSe foundation
- Responsive behavior
- Basic usability

---

## Repository Structure

```txt
firmus-manual-qa-portfolio/
├── README.md
├── README.pt-BR.md
├── bug-reports/
│   ├── bug-report-template.md
│   └── sample-bugs.md
├── checklists/
│   ├── exploratory-test-checklist.md
│   ├── regression-test-checklist.md
│   ├── responsive-test-checklist.md
│   └── smoke-test-checklist.md
├── docs/
│   ├── final-test-report.md
│   ├── severity-priority-guide.md
│   ├── test-plan.md
│   ├── test-scope.md
│   └── test-strategy.md
├── evidences/
│   ├── screenshots/
│   └── videos/
├── test-cases/
│   ├── authentication-test-cases.md
│   ├── clients-test-cases.md
│   ├── dashboard-test-cases.md
│   ├── financial-test-cases.md
│   ├── nfse-test-cases.md
│   └── quotes-test-cases.md
└── test-executions/
    ├── execution-cycle-01.md
    └── execution-summary.md
```

---

## QA Artifacts

This repository contains the following QA artifacts:

### Documentation

- Test Plan
- Test Scope
- Test Strategy
- Severity and Priority Guide
- Final Test Report

### Test Design

- Authentication test cases
- Dashboard test cases
- Clients test cases
- Quotes test cases
- Financial test cases
- NFSe test cases

### Test Execution

- Manual execution cycle
- Execution summary
- Smoke test checklist
- Regression test checklist
- Responsive test checklist
- Exploratory test checklist

### Bug Reporting

- Bug report template
- Sample bug reports
- Evidence-based documentation

---

## Test Case Format

Each test case follows a structured format:

```txt
Test Case ID
Title
Module
Type
Priority
Severity if failed
Preconditions
Steps to reproduce
Expected result
Actual result
Status
Evidence
Notes
```

Example:

```txt
TC-AUTH-001 — Login with valid credentials

Module: Authentication
Type: Functional
Priority: High
Severity if failed: Critical

Preconditions:
- The user has valid credentials
- The application is running
- The user is on the login page

Steps:
1. Open the Firmus application
2. Enter a valid email
3. Enter a valid password
4. Click the login button

Expected Result:
The user should be authenticated and redirected to the dashboard.

Status:
Not executed
```

---

## Bug Report Format

Bug reports follow a professional structure:

```txt
Bug ID
Title
Environment
Severity
Priority
Preconditions
Steps to reproduce
Actual result
Expected result
Evidence
Additional notes
```

This format helps ensure that each bug report is clear, reproducible and useful for developers.

---

## Severity and Priority

This project separates **severity** from **priority**.

**Severity** describes the impact of the issue on the system.

**Priority** describes how urgently the issue should be fixed.

### Severity

| Severity | Meaning |
|---|---|
| Critical | Blocks a critical flow or prevents system usage |
| High | Affects an important feature with no easy workaround |
| Medium | Affects a feature but has a workaround |
| Low | Minor visual, text or usability issue |

### Priority

| Priority | Meaning |
|---|---|
| High | Should be fixed as soon as possible |
| Medium | Should be fixed in a planned cycle |
| Low | Can be fixed later |

---

## Tools Used

The following tools and resources are used in this manual QA process:

- GitHub
- Markdown
- Browser DevTools
- Screenshots
- Video evidence
- Manual exploratory testing
- Local application environment
- QA documentation practices

---

## Current Status

| Area | Status |
|---|---|
| Repository structure | Completed |
| README documentation | Completed |
| Test plan | Completed |
| Test scope | Completed |
| Test strategy | Completed |
| Test cases | Completed |
| Test execution cycle | In Progress |
| Bug reports | Pending |
| Final QA report | Pending |

---

## Professional Skills Demonstrated

This project demonstrates the following QA skills:

- Manual testing
- Test planning
- Test scope definition
- Test case creation
- Bug reporting
- Functional testing
- Regression testing
- Smoke testing
- Exploratory testing
- Responsive testing
- Evidence collection
- Technical documentation
- Quality-oriented thinking
- Communication of test results

---

## About the Tester

**Ademir dos Santos Junior**  
QA Analyst | Full Stack Developer

I am building a professional QA portfolio focused on practical testing activities, real-world documentation and hands-on validation of web applications.

This repository is part of my learning and career development path in Quality Assurance, combining manual testing foundations with software development experience.

---

## Related Projects

- [Firmus Application](https://github.com/JuniorSantosDev86/firmus-app)
- [Cypress Mini Shop QA](https://github.com/JuniorSantosDev86/cypress-mini-shop-qa)
- [Manual QA Tests — SauceDemo Login](https://github.com/JuniorSantosDev86/qa-manual-tests-saucedemo-login)

---

## Repository Purpose

This repository was created to show a complete and organized manual QA workflow applied to a real application.

It is intended to be used as a professional portfolio project for QA, software testing and quality assurance opportunities.

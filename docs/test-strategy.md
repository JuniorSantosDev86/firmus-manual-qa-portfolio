# Test Strategy — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Document Type | Test Strategy |
| Tester | Junior Santos |
| Version | 1.0 |
| Status | In progress |
| Test Approach | Manual QA |

---

## 2. Objective

The objective of this document is to define the manual testing strategy used to validate the Firmus application.

This strategy describes the testing approach, test levels, test types, prioritization criteria, execution method, evidence strategy and bug reporting approach used during the manual QA cycle.

The goal is to ensure that testing is structured, realistic and focused on the most important user-facing flows.

---

## 3. Testing Approach

The testing approach for this project is based on manual validation of critical business flows from the end user's perspective.

The strategy focuses on:

- Understanding the expected behavior of each feature
- Designing clear and reproducible test cases
- Validating the most important user journeys
- Executing smoke and functional test cycles
- Exploring edge cases and unexpected behaviors
- Reporting defects with clear evidence
- Documenting results in a professional QA format

The main priority is to validate whether the application behaves correctly, consistently and clearly for users.

---

## 4. Test Levels

This manual QA cycle focuses on system-level and user-facing validation.

| Test Level | Included | Description |
|---|---|---|
| Unit Testing | No | Not covered in this manual QA repository |
| Integration Testing | Partial | Only visible integration behavior is observed from the UI |
| System Testing | Yes | Main focus of this manual QA cycle |
| Acceptance Testing | Partial | Basic validation of expected business behavior |
| End-to-End Testing | Partial | Manual validation of complete user flows where applicable |

---

## 5. Test Types Strategy

### 5.1 Smoke Testing

Smoke testing will be used to quickly validate whether the most critical areas of the application are working.

Smoke tests will focus on:

- Application loading
- Login behavior
- Dashboard access
- Main navigation
- Client area access
- Quote area access
- Financial area access
- NFSe area access
- Logout behavior

Smoke testing should be executed before deeper manual testing.

---

### 5.2 Functional Testing

Functional testing will validate whether each feature behaves according to the expected result.

Functional tests will focus on:

- Forms
- Buttons
- Navigation
- User actions
- Required fields
- Error messages
- Visible data
- Status changes
- Empty states
- Main business flows

Each functional test case must include clear steps, expected results and execution status.

---

### 5.3 Regression Testing

Regression testing will be used to ensure that existing functionality continues to work after fixes, improvements or changes.

Regression testing will focus on:

- Authentication
- Protected routes
- Dashboard
- Clients
- Quotes
- Financial overview
- NFSe foundation
- Navigation
- Responsive behavior

Regression testing should be executed after relevant changes in the application.

---

### 5.4 Exploratory Testing

Exploratory testing will be used to investigate behaviors that are not fully covered by scripted test cases.

Exploratory testing will focus on:

- Unexpected user actions
- Unusual navigation paths
- Invalid inputs
- Empty states
- UI inconsistencies
- Confusing messages
- Broken flows
- Visual issues
- Usability friction

Findings from exploratory testing may become bug reports or new test cases.

---

### 5.5 Responsive Testing

Responsive testing will validate whether the application remains usable across different viewport sizes.

Responsive testing will focus on:

- Desktop layout
- Tablet-like layout
- Mobile-like layout
- Sidebar behavior
- Drawer behavior
- Button visibility
- Form usability
- Text readability
- Content overflow
- Navigation usability

This is not a full cross-device certification, but a practical responsive validation from a QA perspective.

---

### 5.6 Basic Usability Review

Basic usability review will be used to observe whether the application is clear and easy to use.

The review will focus on:

- Clear labels
- Understandable actions
- Visible feedback
- Consistent navigation
- Clear empty states
- Helpful error messages
- Readable content
- Avoidance of confusing flows

This is not a formal UX research process.

---

## 6. Test Prioritization

Testing will be prioritized based on business impact and user risk.

High-priority areas:

1. Authentication and protected routes
2. Dashboard / Control Tower
3. Clients
4. Quotes
5. Financial overview
6. NFSe foundation
7. Responsive navigation
8. Basic usability

Critical flows must be tested before secondary flows.

---

## 7. Test Case Design Technique

The test cases will be designed using practical manual QA techniques, including:

- Positive testing
- Negative testing
- Boundary thinking
- Required field validation
- User journey validation
- Error message validation
- Empty state validation
- Basic equivalence partitioning
- Exploratory scenario discovery

Each test case should be clear enough for another tester to execute without needing additional explanation.

---

## 8. Execution Strategy

The manual execution will follow this order:

1. Prepare the local environment
2. Confirm that the application is running
3. Execute the smoke checklist
4. Execute functional test cases by module
5. Record actual results
6. Capture evidence when needed
7. Report bugs found during execution
8. Execute regression checks when applicable
9. Update the execution summary
10. Prepare the final QA report

Each test case must receive one of the following statuses:

| Status | Meaning |
|---|---|
| Passed | The actual result matches the expected result |
| Failed | The actual result does not match the expected result |
| Blocked | The test could not be executed due to an issue or dependency |
| Not Executed | The test has not been executed yet |

---

## 9. Bug Reporting Strategy

Each bug report must describe only one issue.

A valid bug report should include:

- Bug ID
- Clear title
- Environment
- Severity
- Priority
- Preconditions
- Steps to reproduce
- Actual result
- Expected result
- Evidence
- Additional notes when useful

The goal is to make each issue easy to understand, reproduce and prioritize.

---

## 10. Evidence Strategy

Evidence will be collected when it helps support a test result or bug report.

Evidence may include:

- Screenshots
- Short videos
- Browser console observations
- UI states
- Error messages
- Before and after comparisons

Evidence should be stored in:

| Evidence Type | Folder |
|---|---|
| Screenshots | evidences/screenshots/ |
| Videos | evidences/videos/ |

Evidence files should use clear names, such as:

- `login-invalid-credentials-error.png`
- `dashboard-mobile-layout-overflow.png`
- `quote-required-field-validation.png`

---

## 11. Severity Strategy

Severity will be defined based on the impact of the issue on the system or user flow.

| Severity | Description |
|---|---|
| Critical | Blocks a critical flow or prevents the system from being used |
| High | Affects an important feature with no simple workaround |
| Medium | Affects a feature but has an available workaround |
| Low | Minor visual, text, layout or usability issue |

---

## 12. Priority Strategy

Priority will be defined based on how urgently the issue should be fixed.

| Priority | Description |
|---|---|
| High | Should be fixed as soon as possible |
| Medium | Should be fixed in a planned development cycle |
| Low | Can be fixed later without major impact |

Severity and priority must be evaluated separately.

---

## 13. Test Data Strategy

The test data will be based on local or mocked application data.

Test data may include:

- Valid user credentials
- Invalid login inputs
- Existing client records
- New client examples
- Quote examples
- Financial records
- NFSe sample records
- Empty state scenarios
- Invalid input scenarios

Sensitive or private data must not be committed to this repository.

---

## 14. Risk-Based Testing

The strategy follows a risk-based testing approach.

The highest-risk areas are tested first because failures in these areas could have the greatest impact on the user experience.

| Risk Area | Reason |
|---|---|
| Authentication | Users must access the application safely |
| Protected routes | Private areas must not be accessible without authentication |
| Dashboard | Users depend on operational visibility |
| Clients | Client records are central to the system |
| Quotes | Quotes are a core business workflow |
| Financial overview | Users need reliable business visibility |
| NFSe foundation | Fiscal information has business relevance |
| Responsive navigation | The application must remain usable on different screen sizes |

---

## 15. Communication Strategy

Test results must be documented clearly and objectively.

The QA documentation should make it easy to understand:

- What was tested
- How it was tested
- What passed
- What failed
- What was blocked
- Which bugs were found
- What evidence supports the results
- What risks remain

The documentation should be useful for recruiters, developers and QA reviewers.

---

## 16. Strategy Approval Criteria

This test strategy is considered approved when:

- The testing approach is defined
- The test types are documented
- The execution method is clear
- The prioritization criteria are defined
- The evidence strategy is documented
- The bug reporting strategy is documented
- The strategy supports test case creation and manual execution
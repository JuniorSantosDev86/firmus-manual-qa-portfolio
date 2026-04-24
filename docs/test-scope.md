# Test Scope — Firmus Manual QA

## 1. Document Information

| Field | Information |
|---|---|
| Project | Firmus Manual QA Portfolio |
| System Under Test | Firmus Application |
| Document Type | Test Scope |
| Tester | Junior Santos |
| Version | 1.0 |
| Status | In progress |

---

## 2. Objective

The objective of this document is to define the manual testing scope for the Firmus application.

This scope helps clarify which modules, flows and behaviors will be validated during the manual QA cycle, as well as the areas that are intentionally out of scope.

The goal is to keep the testing process focused, realistic and aligned with the most important user-facing flows.

---

## 3. Scope Overview

The manual QA scope focuses on validating the main operational flows available in the Firmus application from the user's perspective.

The testing activities will cover:

- Authentication behavior
- Protected route behavior
- Dashboard / Control Tower visibility
- Client-related flows
- Quote-related flows
- Financial overview
- NFSe foundation screens
- Responsive behavior
- Basic usability
- Error handling in visible user flows

This scope does not include deep technical validation, backend code review, load testing or production-level monitoring.

---

## 4. Modules in Scope

### 4.1 Authentication

The authentication module includes the flows related to user access and session behavior.

In scope:

- Login with valid credentials
- Login with invalid credentials
- Logout behavior
- Session persistence
- Access to protected routes without authentication
- Redirection after login
- Redirection after logout
- Basic validation of authentication error messages

Out of scope:

- Password recovery flow, unless available
- Multi-factor authentication
- Deep session security testing
- Token inspection or backend auth implementation

---

### 4.2 Protected Routes

Protected routes are areas of the application that should only be accessible to authenticated users.

In scope:

- Direct access to private routes while logged out
- Access to private routes while logged in
- Redirect behavior for unauthenticated users
- Navigation consistency after authentication
- Basic route protection from a user perspective

Out of scope:

- Backend authorization rules
- Role-based access control, unless available
- Advanced permission matrix validation

---

### 4.3 Dashboard / Control Tower

The Dashboard / Control Tower is the main operational overview area of the application.

In scope:

- Dashboard page loading
- Visibility of main summary cards
- Operational summary information
- Next actions section
- Recent activities section
- Empty states, if applicable
- Basic layout consistency
- Navigation from the dashboard to related areas

Out of scope:

- Deep validation of calculation logic
- Backend data source validation
- Real-time update validation, unless available

---

### 4.4 Clients

The clients module includes flows related to client information and client management.

In scope:

- Clients page loading
- Client list visibility
- Empty state behavior
- Client creation flow, if available
- Required field validation
- Invalid input validation
- Client details visibility, if available
- Basic navigation involving client records

Out of scope:

- Database validation
- Duplicate detection logic, unless visible in UI
- Bulk import or export, unless available
- Advanced client segmentation

---

### 4.5 Quotes

The quotes module includes flows related to creating and managing service quotes.

In scope:

- Quotes page loading
- Quote list visibility
- Quote creation flow
- Required field validation
- Quote value input behavior
- Quote status visibility
- Quote details visibility, if available
- Basic quote lifecycle from a user perspective
- Public quote access, if available

Out of scope:

- PDF generation deep validation, unless manually visible
- Email delivery validation
- Payment-related quote behavior
- Backend quote calculation rules not visible in UI

---

### 4.6 Financial Overview

The financial module includes information related to financial visibility and operational summaries.

In scope:

- Financial page loading
- Visibility of financial summary cards
- Display of revenue, pending values or related indicators
- Empty states
- Basic formatting of monetary values
- Basic filtering behavior, if available
- Navigation between financial information and related records

Out of scope:

- Accounting accuracy validation
- Tax calculation validation
- External financial integration
- Database-level financial reconciliation

---

### 4.7 NFSe Foundation

The NFSe module includes the foundational screens and records related to service invoice operations.

In scope:

- NFSe page loading
- NFSe record visibility
- Display of provider reference, document number or fiscal status when available
- Empty states
- Basic status visibility
- Basic validation of user-facing NFSe information
- Navigation involving NFSe records

Out of scope:

- Real NFSe issuance with government provider
- Fiscal authority integration
- Legal tax validation
- Provider API behavior
- XML validation
- Production fiscal compliance validation

---

### 4.8 Responsive Behavior

Responsive testing validates whether the application remains usable across different screen sizes.

In scope:

- Desktop viewport
- Tablet-like viewport
- Mobile-like viewport
- Sidebar or drawer behavior
- Main navigation usability
- Content readability
- Button visibility
- Form usability on smaller screens

Out of scope:

- Full cross-device certification
- Native mobile app testing
- BrowserStack or device farm validation
- Pixel-perfect design audit

---

### 4.9 Basic Usability

Basic usability testing validates whether the application is understandable and easy to use from the user's perspective.

In scope:

- Clear labels
- Clear buttons
- Understandable empty states
- Consistent navigation
- Visible feedback after user actions
- Basic readability
- Clear error messages
- Avoidance of confusing flows

Out of scope:

- Formal UX research
- User interviews
- A/B testing
- Heatmap analysis
- Advanced accessibility audit

---

## 5. Test Types in Scope

The following test types are included in this manual QA cycle:

| Test Type | Included | Notes |
|---|---|---|
| Smoke Testing | Yes | Used to validate critical flows quickly |
| Functional Testing | Yes | Main focus of this manual QA cycle |
| Regression Testing | Yes | Used after fixes or changes |
| Exploratory Testing | Yes | Used to identify unexpected issues |
| Responsive Testing | Yes | Basic validation across screen sizes |
| Usability Review | Yes | Focused on visible user experience |
| Accessibility Testing | Partial | Only basic visual/usability observations |
| Performance Testing | No | Covered in a separate portfolio area |
| API Testing | No | Covered in a separate portfolio area |
| Security Testing | Partial | Only basic user-facing route protection |

---

## 6. Features Out of Scope

The following areas are intentionally out of scope for this manual QA cycle:

- Automated Cypress test implementation
- API testing with Postman
- Load and performance testing
- Security penetration testing
- Database validation
- Backend code review
- Real external service integration
- Real NFSe provider validation
- Production monitoring
- Accessibility audit with specialized tools
- Contract testing
- Schema validation
- Unit testing
- Source code quality review

These topics may be covered in separate repositories or future QA portfolio projects.

---

## 7. Test Depth

The manual QA cycle will focus on user-facing behavior.

The validation depth includes:

- Page loading
- Navigation
- Form behavior
- Visible data
- Required field validation
- Empty states
- Error messages
- User feedback
- Basic responsive behavior
- Clear expected versus actual result documentation

The validation depth does not include internal implementation details, database state inspection or backend service validation.

---

## 8. Business-Critical Flows

The most important flows for this test cycle are:

| Flow | Reason |
|---|---|
| Login and access control | Users must be able to securely access the application |
| Dashboard visibility | Users need a clear operational overview |
| Client management | Client records are central to the product |
| Quote management | Quotes are one of the core business workflows |
| Financial overview | Users need visibility over business information |
| NFSe foundation | Fiscal workflows are relevant for service providers |
| Responsive navigation | Users may access the system from different screen sizes |

---

## 9. Test Limitations

This test scope has the following limitations:

- Testing is performed in a local development environment
- Some data may be mocked, seeded or manually created
- Some features may still be evolving
- External integrations may not represent production behavior
- Manual testing may not cover all possible edge cases
- This cycle is focused on portfolio demonstration and practical QA documentation

---

## 10. Scope Approval Criteria

This test scope is considered approved when:

- The modules in scope are clearly defined
- The out-of-scope areas are documented
- The test depth is realistic
- The most important business flows are identified
- The scope supports the creation of test cases and execution checklists
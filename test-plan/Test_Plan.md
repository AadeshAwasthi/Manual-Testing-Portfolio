# Test Plan: SauceDemo Web Application

| Item | Details |
|---|---|
| Document | Test Plan (Demo Project) |
| Application | SauceDemo, https://www.saucedemo.com |
| Prepared By | Aadesh Awasthi |
| Version | 1.0 |

## 1. Introduction

This test plan describes the scope, approach, resources and schedule for testing the SauceDemo e-commerce web application. It is a demo project prepared for portfolio purposes.

## 2. Objectives

- Verify that all main user flows work as expected (login, browse, cart, checkout).
- Find and report defects with clear steps and evidence.
- Confirm the application works on the supported browsers and screen sizes.

## 3. Scope

### In Scope

| Module | Features |
|---|---|
| Login | Valid and invalid login, locked user, error messages, logout |
| Product Listing | Product display, sorting, product details |
| Cart | Add, remove, cart badge, cart page |
| Checkout | Customer information, order overview, price calculation, order completion |
| Navigation | Side menu, footer links, Reset App State |
| UI and Compatibility | Chrome, Firefox, Edge; desktop, tablet and mobile viewport |

### Out of Scope

- Load and stress testing
- Penetration testing
- Payment gateway testing (the demo site has no real payment)
- Database testing (no database access on the demo site)

## 4. Test Approach

| Testing Type | Description |
|---|---|
| Smoke Testing | Quick check of critical flows on every new build |
| Functional Testing | Each feature is tested against expected behaviour |
| Negative Testing | Invalid and empty inputs, direct URL access |
| UI Testing | Layout, alignment, images, text |
| Browser Compatibility | Chrome, Firefox and Edge (latest versions) |
| Regression Testing | Re-run of impacted test cases after bug fixes |
| Retesting | Verification of fixed bugs |

## 5. Test Environment

| Item | Details |
|---|---|
| URL | https://www.saucedemo.com |
| OS | Windows 11 |
| Browsers | Google Chrome, Mozilla Firefox, Microsoft Edge (latest) |
| Devices | Desktop 1920 x 1080; tablet and mobile through browser DevTools |
| Test Users | standard_user, locked_out_user, problem_user, performance_glitch_user, error_user, visual_user |

## 6. Entry and Exit Criteria

### Entry Criteria

- Application URL is accessible and stable.
- Test cases are written and reviewed.
- Test data (test users) is available.

### Exit Criteria

- 100% of planned test cases are executed.
- No Blocker or Critical bug is open.
- All Major bugs are fixed or accepted by the stakeholders.
- Test Summary Report is shared.

## 7. Suspension and Resumption Criteria

- **Suspend** testing if the application is down or login is blocked for all users.
- **Resume** testing once the blocker is fixed and the smoke test passes.

## 8. Test Deliverables

- Test Plan and Test Strategy
- Test Scenarios and Test Cases
- Smoke and Regression Checklists
- Bug Reports
- Requirement Traceability Matrix
- Test Execution Report and Test Summary Report

## 9. Schedule

| Activity | Duration |
|---|---|
| Requirement analysis and test planning | 1 day |
| Test scenario and test case design | 3 days |
| Test execution, cycle 1 | 2 days |
| Bug reporting and retesting | 1 day |
| Regression and test closure | 1 day |

## 10. Roles and Responsibilities

| Role | Responsibility |
|---|---|
| QA Engineer (Aadesh Awasthi) | Planning, test design, execution, bug reporting, reporting |

## 11. Risks and Mitigation

| Risk | Mitigation |
|---|---|
| Demo site may be down or changed without notice | Re-check the site before execution, update test cases if needed |
| No requirement document is available | Requirements are derived from application behaviour and common e-commerce standards |
| Limited time for all browsers | Full run on Chrome, smoke and key flows on Firefox and Edge |

## 12. Tools

| Purpose | Tool |
|---|---|
| Test case management | Markdown / Excel |
| Bug tracking | Jira style bug reports |
| Browser testing | Chrome DevTools |
| Version control | Git and GitHub |

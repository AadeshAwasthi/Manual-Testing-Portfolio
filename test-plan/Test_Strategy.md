# Test Strategy: SauceDemo Web Application

> Demo document prepared by Aadesh Awasthi for portfolio purposes.

## 1. Purpose

The test strategy explains **how** testing will be done. The test plan explains what, when and who; this document explains the approach behind it.

## 2. Test Levels

| Level | Covered | Notes |
|---|---|---|
| Unit Testing | No | Done by developers |
| Integration Testing | Partly | Cart to checkout data flow |
| System Testing | Yes | Complete application, end to end |
| User Acceptance Testing | Yes | Real user flows: buy one or more products |

## 3. Test Types

1. **Smoke Testing** on each build, using the [Smoke Checklist](../checklists/Smoke_Testing_Checklist.md).
2. **Functional Testing** of every module using detailed test cases.
3. **Negative Testing** with invalid, empty and unexpected inputs.
4. **UI Testing** for layout, alignment, images, spelling and consistency.
5. **Browser Compatibility Testing** on Chrome, Firefox and Edge.
6. **Responsive Testing** on desktop, tablet and mobile viewport.
7. **Regression Testing** after each fix, using the [Regression Checklist](../checklists/Regression_Testing_Checklist.md).
8. **Retesting** of every fixed bug.

## 4. Test Design Techniques

| Technique | Where it is used |
|---|---|
| Equivalence Partitioning | Login: valid user, invalid user, locked user |
| Boundary Value Analysis | Empty and very long values in form fields |
| Decision Table | Login combinations of username and password |
| State Transition | Cart button: Add to cart <-> Remove |
| Error Guessing | Direct URL access, Back button after logout, empty cart checkout |

### Example decision table: Login

| Username | Password | Result |
|---|---|---|
| Valid | Valid | Login successful |
| Valid | Invalid | Error: do not match |
| Invalid | Valid | Error: do not match |
| Empty | Any | Error: Username is required |
| Valid | Empty | Error: Password is required |
| Locked user | Valid | Error: user has been locked out |

## 5. Test Data

Test users are given on the application login page. Checkout data (name and postal code) is dummy data created by the tester.

## 6. Defect Management

### Bug life cycle

`New > Assigned > Open > Fixed > Retest > Verified > Closed`  (`Reopened` if the fix fails)

### Severity definition

| Severity | Definition | Example |
|---|---|---|
| Blocker | Main flow cannot continue | Finish button does not place the order |
| Critical | Main feature broken, no workaround | Cannot add product to cart |
| Major | Feature works wrongly, workaround exists | Sorting does not work |
| Minor | Small UI or validation issue | Button is misaligned |

Each bug report contains: title, steps to reproduce, expected result, actual result, severity, priority, environment and screenshot.

## 7. Test Metrics

| Metric | Formula |
|---|---|
| Test execution % | (Executed test cases / Total test cases) x 100 |
| Pass % | (Passed test cases / Executed test cases) x 100 |
| Defect density | Number of defects / Number of modules |
| Defect leakage | Defects found after release / Total defects |

## 8. Automation Approach

Stable and repeated flows (login, add to cart, checkout) are good candidates for automation. Sample scripts are in the [Selenium-Java-Automation](https://github.com/AadeshAwasthi/Selenium-Java-Automation) repository. New features and UI checks stay manual.

## 9. Reporting

- Daily status: executed, passed, failed, blocked, bugs raised.
- End of cycle: Test Execution Report.
- End of testing: Test Summary Report with go / no-go recommendation.

# Test Execution Report: Cycle 1

> Demo document. Figures below are sample data for a demo test cycle on SauceDemo.

| Item | Details |
|---|---|
| Application | SauceDemo, https://www.saucedemo.com |
| Test Cycle | Cycle 1 (functional run with `standard_user`) |
| Environment | Windows 11, Google Chrome (latest) |
| Tested By | Aadesh Awasthi |

## 1. Execution Summary

| Metric | Count |
|---|---|
| Total test cases | 60 |
| Executed | 60 |
| Passed | 58 |
| Failed | 2 |
| Blocked | 0 |
| Not run | 0 |
| **Execution %** | **100%** |
| **Pass %** | **96.7%** |

## 2. Module-wise Result

| Module | Total | Passed | Failed | Blocked | Pass % |
|---|---|---|---|---|---|
| Login | 12 | 12 | 0 | 0 | 100% |
| Product Listing | 10 | 10 | 0 | 0 | 100% |
| Shopping Cart | 10 | 10 | 0 | 0 | 100% |
| Checkout | 12 | 11 | 1 | 0 | 91.7% |
| Navigation Menu and Footer | 8 | 7 | 1 | 0 | 87.5% |
| UI and Browser Compatibility | 8 | 8 | 0 | 0 | 100% |
| **Total** | **60** | **58** | **2** | **0** | **96.7%** |

## 3. Failed Test Cases

| TC ID | Title | Linked Bug | Severity |
|---|---|---|---|
| TC_044 | Checkout with empty cart | BUG-014 | Major |
| TC_050 | Reset App State | BUG-017 | Minor |

## 4. Exploratory Testing with Other Test Users

In addition to the scripted run, exploratory testing was done with `problem_user`, `error_user`, `visual_user` and `performance_glitch_user`.

| Test User | Bugs Found | Bug IDs |
|---|---|---|
| problem_user | 7 | BUG-001 to BUG-007 |
| performance_glitch_user | 1 | BUG-008 |
| error_user | 2 | BUG-009, BUG-010 |
| visual_user | 3 | BUG-011 to BUG-013 |
| standard_user | 7 | BUG-014 to BUG-020 |
| **Total** | **20** | |

## 5. Defect Summary

| Severity | Count |
|---|---|
| Blocker | 1 |
| Critical | 4 |
| Major | 8 |
| Minor | 7 |
| **Total** | **20** |

Detailed reports: [Bug-Report-Examples](https://github.com/AadeshAwasthi/Bug-Report-Examples)

## 6. Observations

- Main purchase flow works end to end for `standard_user`.
- Checkout form has weak input validation (BUG-015, BUG-016).
- Cart data is shared between users on the same browser (BUG-020).

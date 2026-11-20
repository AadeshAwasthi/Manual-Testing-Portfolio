# Test Summary Report

> Demo document. Figures are sample data for a demo test cycle on SauceDemo.

| Item | Details |
|---|---|
| Application | SauceDemo |
| Prepared By | Aadesh Awasthi |
| Test Types | Smoke, Functional, Negative, UI, Compatibility, Exploratory |

## 1. Objective

To summarise the testing done on SauceDemo and give a recommendation on release readiness.

## 2. Scope Covered

Login, Product Listing, Product Details, Cart, Checkout, Navigation Menu, UI and browser compatibility.

## 3. Results at a Glance

| Item | Value |
|---|---|
| Test scenarios | 21 |
| Test cases planned | 60 |
| Test cases executed | 60 (100%) |
| Passed | 58 (96.7%) |
| Failed | 2 |
| Total bugs reported | 20 |
| Open Blocker / Critical bugs | 5 |
| Requirement coverage | 100% (17 of 17) |

## 4. Exit Criteria Check

| Exit Criteria | Status |
|---|---|
| 100% planned test cases executed | Met |
| No open Blocker or Critical bug | **Not met** (BUG-003, BUG-004, BUG-010, BUG-012, BUG-020) |
| All Major bugs fixed or accepted | Not met |
| Test Summary Report shared | Met |

## 5. Key Risks

1. Order cannot be completed for `error_user` (BUG-010).
2. Cart data is visible across users on the same browser (BUG-020).
3. Checkout is possible with an empty cart (BUG-014).

## 6. Recommendation

**No-Go.** The main flow works for the standard user, but Blocker and Critical bugs are still open. Release is recommended only after these are fixed, retested, and a regression cycle is completed.

## 7. Lessons Learned

- Testing with different user types found most of the bugs, so user-role coverage should be planned early.
- Negative and validation test cases should be part of every checkout form review.
- A smoke checklist saved time by confirming build stability before detailed testing.

# Requirement Traceability Matrix (RTM)

> Demo document. The RTM maps each requirement to its test scenarios, test cases and bugs, so that no requirement is left untested. Requirements are derived from the behaviour of the demo application.

| Req ID | Requirement | Scenario | Test Cases | Bugs | Status |
|---|---|---|---|---|---|
| REQ_01 | User can login with valid credentials | TS_01 | TC_001, TC_009 | - | Pass |
| REQ_02 | Invalid login shows a proper error | TS_02 | TC_002 to TC_006, TC_010, TC_012 | - | Pass |
| REQ_03 | Protected pages need login | TS_03, TS_20 | TC_011, TC_047 | - | Pass |
| REQ_04 | Products are listed with details | TS_04 | TC_013, TC_021, TC_022 | BUG-001, BUG-012 | Pass (standard_user) |
| REQ_05 | Products can be sorted | TS_05 | TC_014 to TC_017 | BUG-002, BUG-009, BUG-018 | Pass (standard_user) |
| REQ_06 | Product details can be viewed | TS_06 | TC_018 to TC_020 | BUG-006 | Pass (standard_user) |
| REQ_07 | User can add products to cart | TS_07 | TC_023, TC_024, TC_030 | BUG-004 | Pass (standard_user) |
| REQ_08 | User can remove products from cart | TS_08 | TC_025, TC_026 | BUG-005 | Pass (standard_user) |
| REQ_09 | Cart shows correct items and count | TS_09 | TC_027 to TC_029, TC_031, TC_032 | BUG-020 | Pass |
| REQ_10 | Checkout needs valid customer information | TS_10, TS_11 | TC_033 to TC_037 | BUG-003, BUG-015, BUG-016 | Pass |
| REQ_11 | Order totals are calculated correctly | TS_12 | TC_038, TC_039 | - | Pass |
| REQ_12 | User can complete an order | TS_13 | TC_040, TC_041 | BUG-010, BUG-019 | Pass (standard_user) |
| REQ_13 | Empty cart cannot be checked out | TS_14 | TC_044 | BUG-014 | **Fail** |
| REQ_14 | Side menu options work | TS_15 | TC_045 to TC_051 | BUG-007, BUG-017 | **Fail** (TC_050) |
| REQ_15 | Footer links work | TS_16 | TC_052 | - | Pass |
| REQ_16 | Application works on supported browsers and screen sizes | TS_17 to TS_19 | TC_053 to TC_060 | BUG-011, BUG-013 | Pass (standard_user) |

**Coverage:** 16 of 16 requirements are mapped to test cases (100%).

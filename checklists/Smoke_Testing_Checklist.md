# Smoke Testing Checklist: SauceDemo

> Demo document. Smoke testing is a quick check (about 10 to 15 minutes) to confirm that the build is stable enough for detailed testing. If any item fails, the build is rejected.

| Build / Date | Tester | Browser | Result |
|---|---|---|---|
| Demo cycle 1 | Aadesh Awasthi | Chrome (latest) | PASS |

| # | Check | Expected Result | Status |
|---|---|---|---|
| 1 | Application URL opens | Login page loads without error | ✅ Pass |
| 2 | Login with valid user | Products page is displayed | ✅ Pass |
| 3 | Login with invalid user | Error message is displayed | ✅ Pass |
| 4 | Products are listed | 6 products with name, price and image | ✅ Pass |
| 5 | Product detail page opens | Correct product details are shown | ✅ Pass |
| 6 | Sort dropdown works | Order changes as per selected option | ✅ Pass |
| 7 | Add product to cart | Cart badge count increases | ✅ Pass |
| 8 | Open cart page | Added product is listed | ✅ Pass |
| 9 | Remove product from cart | Product is removed, badge updates | ✅ Pass |
| 10 | Start checkout | Checkout information page opens | ✅ Pass |
| 11 | Submit customer information | Overview page opens with totals | ✅ Pass |
| 12 | Finish order | "Thank you for your order!" is shown | ✅ Pass |
| 13 | Side menu opens | Menu options are visible | ✅ Pass |
| 14 | Logout | User returns to login page | ✅ Pass |
| 15 | No console or page crash in the main flow | Pages load without blank screen | ✅ Pass |

**Smoke test decision:** Build accepted for detailed testing.

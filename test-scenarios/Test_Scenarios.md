# Test Scenarios: SauceDemo

> Demo document. A test scenario is a high-level "what to test". Detailed steps are in [Test-Case-Documentation](https://github.com/AadeshAwasthi/Test-Case-Documentation).

| Scenario ID | Module | Scenario | Priority |
|---|---|---|---|
| TS_01 | Login | Verify login with valid credentials | High |
| TS_02 | Login | Verify login with invalid, empty and locked user credentials | High |
| TS_03 | Login | Verify protected pages cannot be opened without login | High |
| TS_04 | Product Listing | Verify all products are displayed with correct details | High |
| TS_05 | Product Listing | Verify sorting by name and by price | Medium |
| TS_06 | Product Details | Verify product detail page shows the correct product | Medium |
| TS_07 | Cart | Verify adding one or more products to the cart | High |
| TS_08 | Cart | Verify removing products from Products page and Cart page | High |
| TS_09 | Cart | Verify cart badge count and cart persistence | Medium |
| TS_10 | Checkout | Verify checkout with valid customer information | High |
| TS_11 | Checkout | Verify mandatory field validation on checkout form | High |
| TS_12 | Checkout | Verify item total, tax and total calculation | High |
| TS_13 | Checkout | Verify order completion and Back Home | High |
| TS_14 | Checkout | Verify cancel at each checkout step | Medium |
| TS_15 | Navigation | Verify side menu options: All Items, About, Logout, Reset App State | Medium |
| TS_16 | Navigation | Verify footer social links | Low |
| TS_17 | UI | Verify layout and alignment of all pages | Low |
| TS_18 | Compatibility | Verify application on Chrome, Firefox and Edge | Medium |
| TS_19 | Responsive | Verify application on tablet and mobile viewport | Medium |
| TS_20 | Session | Verify logout ends the session and Back button does not open protected pages | High |
| TS_21 | Checkout | Verify checkout is not allowed with an empty cart | Medium |

**Total scenarios:** 21

Dynamic Catalog pages (Lazy Load, Spinner, Slider) are out of scope for this cycle.

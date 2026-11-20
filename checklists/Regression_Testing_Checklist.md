# Regression Testing Checklist: SauceDemo

> Demo document. Regression testing confirms that existing features still work after a bug fix or a new change. Tick each item during the regression cycle.

## 1. Login

- [ ] Valid login works
- [ ] Invalid username or password shows correct error
- [ ] Empty username and empty password show correct errors
- [ ] Locked out user cannot login
- [ ] Error banner can be closed
- [ ] Protected pages are not accessible without login

## 2. Product Listing and Details

- [ ] All 6 products are displayed with correct name, price and image
- [ ] Sort by Name (A to Z) and (Z to A) works
- [ ] Sort by Price (low to high) and (high to low) works
- [ ] Product name and product image open the correct detail page
- [ ] Back to products works

## 3. Cart

- [ ] Add to cart from Products page updates button and badge
- [ ] Add to cart from detail page updates button and badge
- [ ] Remove from Products page, detail page and Cart page works
- [ ] Cart page shows correct quantity, name and price
- [ ] Continue Shopping keeps cart items
- [ ] Cart is retained after page refresh

## 4. Checkout

- [ ] First Name, Last Name and Postal Code mandatory validation works
- [ ] Overview page lists the correct items
- [ ] Item total = sum of item prices
- [ ] Total = Item total + Tax
- [ ] Finish places the order and shows the confirmation page
- [ ] Cart is empty after the order
- [ ] Cancel works on both checkout steps

## 5. Navigation

- [ ] All Items, About, Logout and Reset App State work
- [ ] Footer social links open the correct pages
- [ ] Browser Back after logout does not open protected pages

## 6. UI and Compatibility

- [ ] Main flow works on Chrome
- [ ] Main flow works on Firefox
- [ ] Main flow works on Edge
- [ ] Layout is correct on mobile viewport (375 px)
- [ ] No broken images or overlapping elements

## 7. Bug Fix Verification

- [ ] All bugs marked Fixed are retested
- [ ] Related test cases of each fixed bug are re-run
- [ ] No new bug is introduced in the linked modules

| Regression cycle | Date | Tester | Result |
|---|---|---|---|
|  |  |  |  |

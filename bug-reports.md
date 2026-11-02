# Bug Reports: Swag Labs (saucedemo.com)

**Important:** the reports below are **drafts**. Reproduce each one yourself on saucedemo.com first. Keep a report only if you see the same behaviour, then add a screenshot and the date. Delete any you cannot reproduce.

## Template
| Field | Description |
|---|---|
| ID | BUG-001 |
| Title | Short, specific summary |
| Environment | Browser, OS, URL, user |
| Severity / Priority | Critical, High, Medium, Low |
| Steps to reproduce | Numbered steps |
| Expected result | What should happen |
| Actual result | What happened |
| Evidence | Screenshot or video |
| Status | New |

---

## BUG-001: All products show the same image for problem_user (DRAFT, verify)
- **Environment:** Chrome, Windows 11, https://www.saucedemo.com, user `problem_user`
- **Severity:** Medium
- **Steps:**
  1. Open the site and login as `problem_user` / `secret_sauce`
  2. Look at the product images on the Products page
- **Expected:** Each product shows its own image
- **Actual:** Record what you see (reported: the same image for every product)
- **Evidence:** Screenshot
- **Status:** New

## BUG-002: Sorting does not change order for problem_user (DRAFT, verify)
- **Environment:** Chrome, Windows 11, user `problem_user`
- **Severity:** Medium
- **Steps:**
  1. Login as `problem_user`
  2. Choose Price (low to high) in the sort dropdown
- **Expected:** Products sorted by price ascending
- **Actual:** Record what you see
- **Evidence:** Screenshot
- **Status:** New

## BUG-003: Checkout form does not keep entered name for problem_user (DRAFT, verify)
- **Environment:** Chrome, Windows 11, user `problem_user`
- **Severity:** High
- **Steps:**
  1. Login as `problem_user`, add an item, open the cart, click Checkout
  2. Enter first name, last name and postal code
- **Expected:** Each field keeps what was typed and Continue works
- **Actual:** Record what you see, including any error message
- **Evidence:** Screenshot
- **Status:** New

## BUG-004: Checkout allowed with an empty cart (DRAFT, verify)
- **Environment:** Chrome, Windows 11, user `standard_user`
- **Severity:** Low
- **Steps:**
  1. Login as `standard_user` with an empty cart
  2. Open the cart and click Checkout
- **Expected:** Checkout is blocked or a message is shown
- **Actual:** Record what you see
- **Evidence:** Screenshot
- **Status:** New

## BUG-005: Slow login for performance_glitch_user (DRAFT, verify)
- **Environment:** Chrome, Windows 11, user `performance_glitch_user`
- **Severity:** Low
- **Steps:**
  1. Login as `performance_glitch_user`
  2. Note how long it takes to reach the Products page
- **Expected:** Login completes within a normal time (a few seconds)
- **Actual:** Record the time in seconds
- **Evidence:** Screen recording or note
- **Status:** New
